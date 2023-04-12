# Comparing `tmp/vitya-0.12.3.tar.gz` & `tmp/vitya-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.12.3.tar", last modified: Mon Feb 20 14:59:40 2023, max compression
+gzip compressed data, was "dist/vitya-0.13.0.tar", last modified: Wed Apr 12 12:39:07 2023, max compression
```

## Comparing `vitya-0.12.3.tar` & `vitya-0.13.0.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 14:59:40.000000 vitya-0.12.3/
--rw-r--r--   0 runner    (1001) docker     (116)     1065 2023-02-20 14:59:37.000000 vitya-0.12.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2023-02-20 14:59:40.000000 vitya-0.12.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2023-02-20 14:59:37.000000 vitya-0.12.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      128 2023-02-20 14:59:37.000000 vitya-0.12.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-20 14:59:40.000000 vitya-0.12.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      729 2023-02-20 14:59:37.000000 vitya-0.12.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 14:59:40.000000 vitya-0.12.3/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     6734 2023-02-20 14:59:37.000000 vitya-0.12.3/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 14:59:40.000000 vitya-0.12.3/vitya/
--rw-r--r--   0 runner    (1001) docker     (116)      404 2023-02-20 14:59:37.000000 vitya-0.12.3/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-20 14:59:37.000000 vitya-0.12.3/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     2924 2023-02-20 14:59:37.000000 vitya-0.12.3/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     5861 2023-02-20 14:59:37.000000 vitya-0.12.3/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-20 14:59:40.000000 vitya-0.12.3/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2023-02-20 14:59:40.000000 vitya-0.12.3/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      255 2023-02-20 14:59:40.000000 vitya-0.12.3/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-20 14:59:40.000000 vitya-0.12.3/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2023-02-20 14:59:40.000000 vitya-0.12.3/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 12:39:04.000000 vitya-0.13.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 12:39:07.000000 vitya-0.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 12:39:04.000000 vitya-0.13.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 12:39:04.000000 vitya-0.13.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:39:07.000000 vitya-0.13.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-12 12:39:04.000000 vitya-0.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-12 12:39:04.000000 vitya-0.13.0/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.12.3/LICENSE` & `vitya-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.12.3/PKG-INFO` & `vitya-0.13.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.12.3
+Version: 0.13.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 **WARNING**: This library is still in development stage.
 
 Validators for different russian banking values.  
 Values you can validate:
 - ИНН ```validate_inn```
     - ИНН для ИП/Физ.Лица ```validate_inn_ip```
-    - ИНН для Юр.Лица ```validate_inn_jur```
+    - ИНН для Юр.Лица ```validate_inn_le```
 - КПП ```validate_kpp```
 - БИК ```validate_bic```
 - ОГРН ```validate_ogrn```
     - ОГРНИП ```validate_ogrnip```
 - СНИЛС ```validate_snils```
 - ОКТМО ```validate_oktmo```
 
@@ -50,22 +50,22 @@
 validate_ogrn("1027700132195")
 validate_snils("11223344595")
 validate_oktmo("69701000001")
 ```
 
 ```python
 from pydantic import BaseModel, ValidationError
-from vitya.pydantic_fields import Inn
+from vitya.pydantic_fields import INN
 
 
 class InnModel(BaseModel):
-    inn: Inn
+    inn: INN
 
 
 inn_model = InnModel(inn="302502032671")
-assert inn_model.inn == "302502032671"    
+assert inn_model.inn == "302502032671"
 
 try:
     InnModel(inn="3664069398")
 except ValidationError as e:
     print(e.errors())
 ```
```

### Comparing `vitya-0.12.3/README.md` & `vitya-0.13.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 **WARNING**: This library is still in development stage.
 
 Validators for different russian banking values.  
 Values you can validate:
 - ИНН ```validate_inn```
     - ИНН для ИП/Физ.Лица ```validate_inn_ip```
-    - ИНН для Юр.Лица ```validate_inn_jur```
+    - ИНН для Юр.Лица ```validate_inn_le```
 - КПП ```validate_kpp```
 - БИК ```validate_bic```
 - ОГРН ```validate_ogrn```
     - ОГРНИП ```validate_ogrnip```
 - СНИЛС ```validate_snils```
 - ОКТМО ```validate_oktmo```
 
@@ -36,22 +36,22 @@
 validate_ogrn("1027700132195")
 validate_snils("11223344595")
 validate_oktmo("69701000001")
 ```
 
 ```python
 from pydantic import BaseModel, ValidationError
-from vitya.pydantic_fields import Inn
+from vitya.pydantic_fields import INN
 
 
 class InnModel(BaseModel):
-    inn: Inn
+    inn: INN
 
 
 inn_model = InnModel(inn="302502032671")
-assert inn_model.inn == "302502032671"    
+assert inn_model.inn == "302502032671"
 
 try:
     InnModel(inn="3664069398")
 except ValidationError as e:
     print(e.errors())
 ```
```

### Comparing `vitya-0.12.3/setup.py` & `vitya-0.13.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.12.3',
+    version='0.13.0',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.12.3/tests/test_vitya.py` & `vitya-0.13.0/tests/test_vitya.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,300 +1,388 @@
+from typing import Optional
+
 import pytest
 from pydantic import BaseModel, ValidationError as PydanticValidationError
+from pydantic.errors import PydanticValueError
 
 from vitya import (
     ValidationError as VityaValidationError,
     validate_bic,
     validate_inn,
     validate_inn_ip,
-    validate_inn_jur,
+    validate_inn_le,
     validate_kpp,
     validate_ogrn,
     validate_ogrnip,
     validate_oktmo,
     validate_snils,
 )
+from vitya.errors import (
+    OKTMOValidationTypeError,
+    OKTMOValidationValueError,
+    OKTMOValidationValueLenError,
+)
 from vitya.pydantic_fields import (
-    Bic,
-    Inn,
-    InnIp,
-    InnJur,
-    Kpp,
-    Ogrn,
-    OgrnIp,
-    Oktmo,
-    Snils,
+    BIC,
+    INN,
+    INNIP,
+    INNLE,
+    KPP,
+    OGRN,
+    OGRNIP,
+    OKTMO,
+    SNILS,
+    FieldMixin,
 )
 
 
-class InnModel(BaseModel):
-    inn: Inn
+class INNModel(BaseModel):
+    inn: INN
 
 
-class InnModelIp(BaseModel):
-    inn: InnIp
+class INNIPModel(BaseModel):
+    inn: INNIP
 
 
-class InnModelJur(BaseModel):
-    inn: InnJur
+class INNLEModel(BaseModel):
+    inn: INNLE
 
 
-class KppModel(BaseModel):
-    kpp: Kpp
+class KPPModel(BaseModel):
+    kpp: KPP
 
 
-class BicModel(BaseModel):
-    bic: Bic
+class BICModel(BaseModel):
+    bic: BIC
 
 
-class OgrnModel(BaseModel):
-    ogrn: Ogrn
+class OGRNModel(BaseModel):
+    ogrn: OGRN
 
 
-class OgrnIpModel(BaseModel):
-    ogrnip: OgrnIp
+class OGRNIPModel(BaseModel):
+    ogrnip: OGRNIP
 
 
-class SnilsModel(BaseModel):
-    snils: Snils
+class SNILSModel(BaseModel):
+    snils: SNILS
 
 
-class OktmoModel(BaseModel):
-    oktmo: Oktmo
+class OKTMOModel(BaseModel):
+    oktmo: OKTMO
 
 
-@pytest.mark.parametrize('inn', [
-    '3664069397', '302502032671', '7707083893', '7703206417', '771002344404'
-])
+@pytest.mark.parametrize(
+    'inn', [
+        '3664069397', '302502032671', '7707083893', '7703206417', '771002344404'
+    ]
+)
 def test_valid_inn(inn):
     """No exception raise"""
-    assert validate_inn(inn) is None
+    validate_inn(inn)
 
-    inn_model = InnModel(inn=inn)
+    inn_model = INNModel(inn=inn)
     assert inn_model.inn == inn
 
 
-@pytest.mark.parametrize('inn', [
-    '469933069430', '368332974449', '298410962506', '686899030369', '097289845404'
-])
+@pytest.mark.parametrize(
+    'inn', [
+        '469933069430', '368332974449', '298410962506', '686899030369', '097289845404'
+    ]
+)
 def test_valid_inn_ip(inn):
-    assert validate_inn_ip(inn) is None
+    validate_inn_ip(inn)
 
-    inn_model_ip = InnModelIp(inn=inn)
+    inn_model_ip = INNIPModel(inn=inn)
     assert inn_model_ip.inn == inn
 
     with pytest.raises(PydanticValidationError):
-        InnModelJur(inn=inn)
+        INNLEModel(inn=inn)
+
+
+@pytest.mark.parametrize(
+    'inn', [
+        '9267145148', '5302008630', '6524062615', '0207895252', '0990471741'
+    ]
+)
+def test_valid_inn_le(inn):
+    validate_inn_le(inn)
+
+    inn_model_le = INNLEModel(inn=inn)
+    assert inn_model_le.inn == inn
+
+    with pytest.raises(PydanticValidationError):
+        INNIPModel(inn=inn)
 
 
-@pytest.mark.parametrize('inn', [
-    '9267145148', '5302008630', '6524062615', '0207895252', '0990471741'
-])
-def test_valid_inn_jur(inn):
-    assert validate_inn_jur(inn) is None
-
-    inn_model_jur = InnModelJur(inn=inn)
-    assert inn_model_jur.inn == inn
-
-    with pytest.raises(PydanticValidationError):
-        InnModelIp(inn=inn)
-
-
-@pytest.mark.parametrize('inn', [
-    None,           # can't be None
-    '',
-    3664069397,     # can't be nothing than str
-    302502032671,
-    '770708389',    # should be size of 10 or 12 chars
-    '77100234440',
-    '3664069398',   # wrong checksums
-    '302502032672',
-    '302502032681'
-    '36640A9397'    # don't match regexp
-])
+@pytest.mark.parametrize(
+    'inn', [
+        None,  # can't be None
+        '',
+        3664069397,  # can't be nothing than str
+        302502032671,
+        '770708389',  # should be size of 10 or 12 chars
+        '77100234440',
+        '3664069398',  # wrong checksums
+        '302502032672',
+        '302502032681'
+        '36640A9397'  # don't match regexp
+    ]
+)
 def test_wrong_inn(inn):
-    with pytest.raises(VityaValidationError):
+    with pytest.raises(PydanticValueError):
         validate_inn(inn)
 
     with pytest.raises(PydanticValidationError):
-        InnModel(inn=inn)
+        INNModel(inn=inn)
 
     with pytest.raises(PydanticValidationError):
-        InnModelIp(inn=inn)
+        INNIPModel(inn=inn)
 
     with pytest.raises(PydanticValidationError):
-        InnModelJur(inn=inn)
+        INNLEModel(inn=inn)
 
 
-@pytest.mark.parametrize('kpp', [
-    '616401001', '770943002', '7709AB002', '320143522', '704601307', '0'
-])
+@pytest.mark.parametrize(
+    'kpp', [
+        '616401001', '770943002', '7709AB002', '320143522', '704601307',
+    ]
+)
 def test_valid_kpp(kpp):
     """No exception raise"""
-    assert validate_kpp(kpp) is None
+    validate_kpp(kpp)
 
-    kpp_model = KppModel(kpp=kpp)
+    kpp_model = KPPModel(kpp=kpp)
     assert kpp_model.kpp == kpp
 
 
-@pytest.mark.parametrize('kpp', [
-    None,          # can't be None
-    '',
-    616401001,     # can't be nothing than str
-    770943002,
-    '77070838',    # should be size of 9 chars
-    '77100234440',
-    '7709ABС02'    # don't match regexp
-])
+@pytest.mark.parametrize(
+    'kpp', [
+        None,  # can't be None
+        616401001,  # can't be nothing than str
+        770943002,
+        '77070838',  # should be size of 9 chars
+        '77100234440',
+        '7709ABС02'  # don't match regexp
+    ]
+)
 def test_wrong_kpp(kpp):
-    with pytest.raises(VityaValidationError):
+    with pytest.raises(PydanticValueError):
         validate_kpp(kpp)
 
     with pytest.raises(PydanticValidationError):
-        KppModel(kpp=kpp)
+        KPPModel(kpp=kpp)
 
 
-@pytest.mark.parametrize('bic', [
-    '044525901', '043002717', '046577964', '040349758', '041806647'
-])
+@pytest.mark.parametrize(
+    'bic', [
+        '044525901', '043002717', '046577964', '040349758', '041806647'
+    ]
+)
 def test_valid_bic(bic):
     """No exception raise"""
-    assert validate_bic(bic) is None
+    validate_bic(bic)
 
-    bic_model = BicModel(bic=bic)
+    bic_model = BICModel(bic=bic)
     assert bic_model.bic == bic
 
 
-@pytest.mark.parametrize('bic', [
-    None,          # can't be None
-    '',
-    770943002,     # can't be nothing than str
-    '04452590',    # should be size of 9 chars
-    '0445259011',
-    '034525901'    # don't match regexp
-    '04452A901'
-])
+@pytest.mark.parametrize(
+    'bic', [
+        None,  # can't be None
+        '',
+        770943002,  # can't be nothing than str
+        '04452590',  # should be size of 9 chars
+        '0445259011',
+        '034525901'  # don't match regexp
+        '04452A901'
+    ]
+)
 def test_wrong_bic(bic):
-    with pytest.raises(VityaValidationError):
+    with pytest.raises(PydanticValueError):
         validate_bic(bic)
 
     with pytest.raises(PydanticValidationError):
-        BicModel(bic=bic)
+        BICModel(bic=bic)
 
 
-@pytest.mark.parametrize('ogrn', [
-    '1027700132195', '1037700013020', '316784700262702', '304500116000157', '1076935620520'
-])
+@pytest.mark.parametrize(
+    'ogrn', [
+        '1027700132195', '1037700013020', '316784700262702', '304500116000157', '1076935620520'
+    ]
+)
 def test_valid_ogrn(ogrn):
     """No exception raise"""
     assert validate_ogrn(ogrn) is None
 
-    ogrn_model = OgrnModel(ogrn=ogrn)
+    ogrn_model = OGRNModel(ogrn=ogrn)
     assert ogrn_model.ogrn == ogrn
 
 
-@pytest.mark.parametrize('ogrnip', [
-    '304051927964808', '314057243354856', '307870729546242', '312550098407541', '308633624812989'
-])
+@pytest.mark.parametrize(
+    'ogrnip', [
+        '304051927964808', '314057243354856', '307870729546242', '312550098407541', '308633624812989'
+    ]
+)
 def test_valid_ogrnip(ogrnip):
     """No exception raise"""
     assert validate_ogrnip(ogrnip) is None
 
-    ogrnip_model = OgrnIpModel(ogrnip=ogrnip)
+    ogrnip_model = OGRNIPModel(ogrnip=ogrnip)
     assert ogrnip_model.ogrnip == ogrnip
 
 
-@pytest.mark.parametrize('ogrnip', [
-    '1076935620520', '5122703513136', '5081268440446', '5063675362394'
-])
+@pytest.mark.parametrize(
+    'ogrnip', [
+        '1076935620520', '5122703513136', '5081268440446', '5063675362394'
+    ]
+)
 def test_wrong_ogrnip(ogrnip):
     with pytest.raises(PydanticValidationError):
-        OgrnIpModel(ogrnip=ogrnip)
+        OGRNIPModel(ogrnip=ogrnip)
 
 
-@pytest.mark.parametrize('ogrn', [
-    None,          # can't be None
-    '',
-    1027700132195,     # can't be nothing than str
-    '102770013219',    # should be size of 13 or 15 chars
-    '10377000130200',
-    '10277001321955',
-    '1027A00132195'    # don't match regexp
-    '0027700132195',
-    '1027700132196',    # wrong last digit
-    '1037700013021'
-    '304500116000158',
-    '316784700262701'
-])
+@pytest.mark.parametrize(
+    'ogrn', [
+        None,  # can't be None
+        '',
+        1027700132195,  # can't be nothing than str
+        '102770013219',  # should be size of 13 or 15 chars
+        '10377000130200',
+        '10277001321955',
+        '1027A00132195'  # don't match regexp
+        '0027700132195',
+        '1027700132196',  # wrong last digit
+        '1037700013021'
+        '304500116000158',
+        '316784700262701'
+    ]
+)
 def test_wrong_ogrn(ogrn):
     with pytest.raises(VityaValidationError):
         validate_ogrn(ogrn)
 
     with pytest.raises(PydanticValidationError):
-        OgrnModel(ogrn=ogrn)
+        OGRNModel(ogrn=ogrn)
 
     with pytest.raises(PydanticValidationError):
-        OgrnIpModel(ogrnip=ogrn)
+        OGRNIPModel(ogrnip=ogrn)
 
 
-@pytest.mark.parametrize('snils', [
-    '11223344595',
-    '21647164763',
-    '47789365577',
-    '93149947849',
-    '58966302961'
-])
+@pytest.mark.parametrize(
+    'snils', [
+        '11223344595',
+        '21647164763',
+        '47789365577',
+        '93149947849',
+        '58966302961'
+    ]
+)
 def test_valid_snils(snils):
     """No exception raise"""
     assert validate_snils(snils) is None
 
-    snils_model = SnilsModel(snils=snils)
+    snils_model = SNILSModel(snils=snils)
     assert snils_model.snils == snils
 
 
-@pytest.mark.parametrize('snils', [
-    None,
-    '',
-    11223344595,
-    '12-233-445 955',
-    '12-233-445 9',
-    '12-233-445-95',
-    '12-233-44595',
-    '12-233-445 96',
-    '216-471-647 60',
-    '00000000000'
-])
+@pytest.mark.parametrize(
+    'snils', [
+        None,
+        '',
+        11223344595,
+        '12-233-445 955',
+        '12-233-445 9',
+        '12-233-445-95',
+        '12-233-44595',
+        '12-233-445 96',
+        '216-471-647 60',
+        '00000000000'
+    ]
+)
 def test_wrong_snils(snils):
     with pytest.raises(VityaValidationError):
         validate_snils(snils)
 
     with pytest.raises(PydanticValidationError):
-        SnilsModel(snils=snils)
+        SNILSModel(snils=snils)
 
 
-@pytest.mark.parametrize('oktmo', [
-    '69654000',
-    '69701000001',
-    '98603170051',
-    '78623427116',
-    '66614465117'
-])
+@pytest.mark.parametrize(
+    'oktmo', [
+        '69654000',
+        '69701000001',
+        '98603170051',
+        '78623427116',
+        '66614465117',
+    ]
+)
 def test_valid_oktmo(oktmo):
     """No exception raise"""
-    assert validate_oktmo(oktmo) is None
+    assert validate_oktmo(oktmo) == oktmo
 
-    oktmo_model = OktmoModel(oktmo=oktmo)
+    oktmo_model = OKTMOModel(oktmo=oktmo)
     assert oktmo_model.oktmo == oktmo
 
 
-@pytest.mark.parametrize('oktmo', [
-    None,
-    '',
-    69654000,
-    '69 701 000 001'
-])
-def test_wrong_oktmo(oktmo):
-    with pytest.raises(VityaValidationError):
+@pytest.mark.parametrize(
+    'oktmo, error',
+    [
+        (None, OKTMOValidationTypeError),
+        (69654000, OKTMOValidationTypeError),
+        ('6965400', OKTMOValidationValueLenError),
+        ('69b01000001', OKTMOValidationValueError),
+    ]
+)
+def test_wrong_oktmo(oktmo, error):
+    with pytest.raises(error):
         validate_oktmo(oktmo)
 
     with pytest.raises(PydanticValidationError):
-        OktmoModel(oktmo=oktmo)
+        OKTMOModel(oktmo=oktmo)
+
+
+class Field(FieldMixin, str):
+    @classmethod
+    def _validate(cls, value):
+        return value if value not in {'', '0'} else None
+
+
+class TestFieldMixin(BaseModel):
+    field: Field
+
+
+@pytest.mark.parametrize(
+    'value',
+    ('', '0', None)
+)
+def test_field_mixin(value: Optional[str]) -> None:
+    with pytest.raises(PydanticValidationError):
+        TestFieldMixin(field=value)
+
+
+class TestFieldMixinOptional(BaseModel):
+    field: Optional[Field]
+
+
+@pytest.mark.parametrize(
+    'value',
+    ('', '0', None)
+)
+def test_field_mixin_optional(value: Optional[str]) -> None:
+    assert TestFieldMixinOptional(field=value).field is None
+
+
+class TestFieldMixinOptionalWithDefault(BaseModel):
+    field: Optional[Field] = '5'
+
+
+def test_field_mixin_optional_with_default() -> None:
+    assert TestFieldMixinOptionalWithDefault().field == '5'
+
+
+@pytest.mark.parametrize(
+    'value',
+    ('', '0', None),
+)
+def test_field_mixin_optional_with_default_with_value(value: Optional[str]) -> None:
+    assert TestFieldMixinOptionalWithDefault(field=value).field is None
```

### Comparing `vitya-0.12.3/vitya/pydantic_fields.py` & `vitya-0.13.0/vitya/pydantic_fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,119 @@
-from typing import Any, Callable, Generator
+from abc import ABC, abstractmethod
+from typing import Any, Callable, Generator, Optional
+
+from pydantic.fields import ModelField
 
 from .validators import (
     ValidationError,
     validate_bic,
     validate_inn,
     validate_inn_ip,
-    validate_inn_jur,
+    validate_inn_le,
     validate_kpp,
     validate_ogrn,
     validate_ogrnip,
     validate_oktmo,
     validate_snils,
 )
 
 try:
-    from pydantic.errors import PydanticValueError
-except ImportError:
+    from pydantic.errors import MissingError, PydanticValueError
+except ImportError:  # pragma: no cover
     pass
 
 CallableGenerator = Generator[Callable[..., Any], None, None]
 
 
 class PydanticValidationError(PydanticValueError):
     msg_template = 'invalid {name}: {reason}'
 
 
+class EmptyError(Exception):
+    pass
+
+
 def _validate_wrapper(func: Callable[[str], None], name: str, value: str) -> str:
     try:
         func(value)
     except ValidationError as e:
         raise PydanticValidationError(name=name, reason=str(e))
 
     return value
 
 
-class Inn(str):
-    @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
+class FieldMixin(ABC):
+    def __new__(cls, value: Any) -> 'FieldMixin':
+        value = cls._validate(value)
+        if value is None:
+            raise EmptyError
+        return super().__new__(cls, value)  # type: ignore
 
     @classmethod
-    def validate(cls, value: str) -> str:
-        return _validate_wrapper(validate_inn, "inn", value)
-
+    @abstractmethod
+    def _validate(cls, value: Any) -> Any:
+        pass
 
-class InnIp(str):
     @classmethod
     def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, value: str) -> str:
-        return _validate_wrapper(validate_inn_ip, "inn_ip", value)
+        def validator(value: Any, field: ModelField) -> Any:
+            try:
+                return cls(value)
+            except EmptyError:
+                if field.allow_none:
+                    return None
+                raise MissingError
+        yield validator
 
 
-class InnJur(str):
+class INN(FieldMixin, str):
     @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
+    def _validate(cls, value: str) -> str:
+        return validate_inn(value)
 
-    @classmethod
-    def validate(cls, value: str) -> str:
-        return _validate_wrapper(validate_inn_jur, "inn_jur", value)
-
-
-class Kpp(str):
-    @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
 
+class INNIP(FieldMixin, str):
     @classmethod
-    def validate(cls, value: str) -> str:
-        return _validate_wrapper(validate_kpp, "kpp", value)
+    def _validate(cls, value: str) -> str:
+        return validate_inn_ip(value)
 
 
-class Bic(str):
+class INNLE(FieldMixin, str):
     @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
+    def _validate(cls, value: str) -> str:
+        return validate_inn_le(value)
 
+
+class KPP(FieldMixin, str):
     @classmethod
-    def validate(cls, value: str) -> str:
-        return _validate_wrapper(validate_bic, "bic", value)
+    def _validate(cls, value: str) -> Optional[str]:
+        return validate_kpp(value)
 
 
-class Ogrn(str):
+class BIC(FieldMixin, str):
     @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
+    def _validate(cls, value: str) -> str:
+        return validate_bic(value)
 
+
+class OGRN(FieldMixin, str):
     @classmethod
-    def validate(cls, value: str) -> str:
+    def _validate(cls, value: str) -> str:
         return _validate_wrapper(validate_ogrn, "ogrn", value)
 
 
-class OgrnIp(str):
-    @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
-
+class OGRNIP(FieldMixin, str):
     @classmethod
-    def validate(cls, value: str) -> str:
+    def _validate(cls, value: str) -> str:
         return _validate_wrapper(validate_ogrnip, "ogrn_ip", value)
 
 
-class Snils(str):
-    @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
-
+class SNILS(FieldMixin, str):
     @classmethod
-    def validate(cls, value: str) -> str:
+    def _validate(cls, value: str) -> str:
         return _validate_wrapper(validate_snils, "snils", value)
 
 
-class Oktmo(str):
-    @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate
-
+class OKTMO(FieldMixin, str):
     @classmethod
-    def validate(cls, value: str) -> str:
-        return _validate_wrapper(validate_oktmo, "oktmo", value)
+    def _validate(cls, value: str) -> Optional[str]:
+        return validate_oktmo(value)
```

### Comparing `vitya-0.12.3/vitya/validators.py` & `vitya-0.13.0/vitya/validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,120 @@
 import re
 from typing import List, Optional
 
+from .errors import (
+    BICValidationLenError,
+    BICValidationTypeError,
+    BICValidationValueDigitsOnlyError,
+    INNValidationControlSumError,
+    INNValidationDigitsOnlyError,
+    INNValidationLenError,
+    INNValidationStartsWithZerosError,
+    INNValidationTypeError,
+    KPPValidationTypeError,
+    KPPValidationValueError,
+    KPPValidationValueLenError,
+    OKTMOValidationTypeError,
+    OKTMOValidationValueError,
+    OKTMOValidationValueLenError,
+)
+
 
 class ValidationError(ValueError):
     """
     Exception that raises if passed data is invalid
     """
     pass
 
 
 def _count_inn_checksum(inn: str, coefficients: List[int]) -> int:
     assert len(inn) == len(coefficients)
     n = sum([int(digit) * coef for digit, coef in zip(inn, coefficients)])
     return n % 11 % 10
 
 
-def validate_inn(inn: str, is_ip: Optional[bool] = None) -> None:
+def validate_inn(inn: str, is_ip: Optional[bool] = None) -> str:
     """
     Source:
     https://www.consultant.ru/document/cons_doc_LAW_134082/947eeb5630c9f58cbc6103f0910440cef8eaccac/
     https://ru.wikipedia.org/wiki/%D0%98%D0%B4%D0%B5%D0%BD%D1%82%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9_%D0%BD%D0%BE%D0%BC%D0%B5%D1%80_%D0%BD%D0%B0%D0%BB%D0%BE%D0%B3%D0%BE%D0%BF%D0%BB%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D1%89%D0%B8%D0%BA%D0%B0
     """
     if not isinstance(inn, str):
-        raise ValidationError('inn should be passed as string')
+        raise INNValidationTypeError
 
     if not re.fullmatch(r'[0-9]+', inn):
-        raise ValidationError('inn can contain only numbers')
+        raise INNValidationDigitsOnlyError
+
+    if inn.startswith('00'):
+        raise INNValidationStartsWithZerosError
 
     coefs10 = [2, 4, 10, 3, 5, 9, 4, 6, 8]
     coefs11 = [7] + coefs10
     coefs12 = [3] + coefs11
 
     if len(inn) == 10 and is_ip is not True:
         n10 = _count_inn_checksum(inn[:9], coefs10)
         if n10 != int(inn[9]):
-            raise ValidationError(f'wrong checksum on last digit: {inn[9]}; expected: {n10}')
-        return
-
-    if len(inn) == 12 and is_ip is not False:
+            raise INNValidationControlSumError
+        return inn
+    elif len(inn) == 12 and is_ip is not False:
         n11 = _count_inn_checksum(inn[:10], coefs11)
         if n11 != int(inn[10]):
-            raise ValidationError(f'wrong checksum on pre-last digit: {inn[10]}; expected: {n11}')
+            raise INNValidationControlSumError
 
         n12 = _count_inn_checksum(inn[:11], coefs12)
         if n12 != int(inn[11]):
-            raise ValidationError(f'wrong checksum on last digit: {inn[11]}; expected: {n12}')
-        return
+            raise INNValidationControlSumError
+        return inn
+    elif len(inn) == 5:
+        return inn
 
-    raise ValidationError('wrong size of inn, it can be 10 or 12 chars only')
+    raise INNValidationLenError
 
 
-def validate_inn_ip(inn: str) -> None:
+def validate_inn_ip(inn: str) -> str:
     return validate_inn(inn, is_ip=True)
 
 
-def validate_inn_jur(inn: str) -> None:
+def validate_inn_le(inn: str) -> str:
     return validate_inn(inn, is_ip=False)
 
 
-def validate_kpp(kpp: str) -> None:
+def validate_kpp(kpp: str) -> Optional[str]:
     """
     Source: https://kontur.ru/bk/spravka/491-chtotakoe_kpp
     """
     if not isinstance(kpp, str):
-        raise ValidationError('kpp should be passed as string')
-
-    if kpp == '0':
-        # '0' allowed as kpp value
-        return
+        raise KPPValidationTypeError
+    elif kpp in {'0', ''}:
+        return None
 
     if len(kpp) != 9:
-        raise ValidationError('wrong size of kpp, it can be 9 chars only')
+        raise KPPValidationValueLenError
 
     if not re.fullmatch(r'[0-9]{4}[0-9A-Z]{2}[0-9]{3}', kpp):
-        raise ValidationError('wrong kpp')
+        raise KPPValidationValueError
+    return kpp
 
 
-def validate_bic(bic: str) -> None:
+def validate_bic(bic: str) -> str:
     """
     Source:
     https://ru.wikipedia.org/wiki/%D0%91%D0%B0%D0%BD%D0%BA%D0%BE%D0%B2%D1%81%D0%BA%D0%B8%D0%B9_%D0%B8%D0%B4%D0%B5%D0%BD%D1%82%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9_%D0%BA%D0%BE%D0%B4
     https://bik-info.ru/
     """
     if not isinstance(bic, str):
-        raise ValidationError('bic should be passed as string')
+        raise BICValidationTypeError
 
     if len(bic) != 9:
-        raise ValidationError('wrong size of bic, it can be 9 chars only')
+        raise BICValidationLenError
 
     if not re.fullmatch(r'[0-9]+', bic):
-        raise ValidationError('wrong bic')
+        raise BICValidationValueDigitsOnlyError
+    return bic
 
 
 def validate_ogrn(ogrn: str, is_ip: Optional[bool] = None) -> None:
     """
     Source:
     https://ru.wikipedia.org/wiki/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D0%BD%D0%BE%D0%B9_%D0%B3%D0%BE%D1%81%D1%83%D0%B4%D0%B0%D1%80%D1%81%D1%82%D0%B2%D0%B5%D0%BD%D0%BD%D1%8B%D0%B9_%D1%80%D0%B5%D0%B3%D0%B8%D1%81%D1%82%D1%80%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9_%D0%BD%D0%BE%D0%BC%D0%B5%D1%80
     """
@@ -132,15 +153,15 @@
     """
     if not isinstance(snils, str):
         raise ValidationError('snils should be passed as string')
 
     if not re.fullmatch(r'[0-9]{11}', snils):
         raise ValidationError('wrong snils')
 
-    if int(snils[:9]) < 1001998:     # less than 001-001-998
+    if int(snils[:9]) < 1001998:  # less than 001-001-998
         raise ValidationError('snils must be more than "001-001-998" ')
 
     numbers = []
     parts = [snils[0:3], snils[3:6], snils[6:9]]
     for part in parts:
         numbers.extend([int(num) for num in part])
 
@@ -155,17 +176,21 @@
     else:
         checksum_str = str(checksum)
 
     if checksum_str != snils[-2:]:
         raise ValidationError(f'wrong checksum: {snils[-2:]}; expected: {checksum_str}')
 
 
-def validate_oktmo(oktmo: str) -> None:
+def validate_oktmo(oktmo: str) -> Optional[str]:
     """
     Source:
     https://www.consultant.ru/cons/CGI/online.cgi?req=doc;base=LAW;n=149911#fUpVRbSdflobnNc4
     """
     if not isinstance(oktmo, str):
-        raise ValidationError('oktmo should be passed as string')
-
+        raise OKTMOValidationTypeError
+    elif oktmo in {'', '0'}:
+        return None
+    elif len(oktmo) not in {8, 11}:
+        raise OKTMOValidationValueLenError
     if not re.fullmatch(r'([0-9]{11}|[0-9]{8})', oktmo):
-        raise ValidationError('wrong oktmo')
+        raise OKTMOValidationValueError
+    return oktmo
```

### Comparing `vitya-0.12.3/vitya.egg-info/PKG-INFO` & `vitya-0.13.0/vitya.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.12.3
+Version: 0.13.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 **WARNING**: This library is still in development stage.
 
 Validators for different russian banking values.  
 Values you can validate:
 - ИНН ```validate_inn```
     - ИНН для ИП/Физ.Лица ```validate_inn_ip```
-    - ИНН для Юр.Лица ```validate_inn_jur```
+    - ИНН для Юр.Лица ```validate_inn_le```
 - КПП ```validate_kpp```
 - БИК ```validate_bic```
 - ОГРН ```validate_ogrn```
     - ОГРНИП ```validate_ogrnip```
 - СНИЛС ```validate_snils```
 - ОКТМО ```validate_oktmo```
 
@@ -50,22 +50,22 @@
 validate_ogrn("1027700132195")
 validate_snils("11223344595")
 validate_oktmo("69701000001")
 ```
 
 ```python
 from pydantic import BaseModel, ValidationError
-from vitya.pydantic_fields import Inn
+from vitya.pydantic_fields import INN
 
 
 class InnModel(BaseModel):
-    inn: Inn
+    inn: INN
 
 
 inn_model = InnModel(inn="302502032671")
-assert inn_model.inn == "302502032671"    
+assert inn_model.inn == "302502032671"
 
 try:
     InnModel(inn="3664069398")
 except ValidationError as e:
     print(e.errors())
 ```
```

