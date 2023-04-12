# Comparing `tmp/pyeph-1.1.7.tar.gz` & `tmp/pyeph-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeph-1.1.7.tar", max compression
+gzip compressed data, was "pyeph-1.2.0.tar", max compression
```

## Comparing `pyeph-1.1.7.tar` & `pyeph-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     4808 2022-06-24 20:40:06.616192 pyeph-1.1.7/README.md
--rw-r--r--   0        0        0    44617 2022-05-22 22:19:34.204872 pyeph-1.1.7/pyeph/.files/EPH_tot_urbano_estructura_bases.xlsx
--rw-r--r--   0        0        0       88 2022-02-20 21:40:02.531228 pyeph-1.1.7/pyeph/__init__.py
--rw-r--r--   0        0        0     1452 2022-03-11 22:09:32.020270 pyeph-1.1.7/pyeph/ads.py
--rw-r--r--   0        0        0      105 2022-02-20 15:36:57.962306 pyeph-1.1.7/pyeph/calc/README.md
--rw-r--r--   0        0        0        0 2022-02-20 15:36:57.962306 pyeph-1.1.7/pyeph/calc/__init__.py
--rw-r--r--   0        0        0      178 2022-02-20 15:36:57.962306 pyeph-1.1.7/pyeph/calc/api.py
--rw-r--r--   0        0        0     1863 2022-02-20 15:56:14.407998 pyeph-1.1.7/pyeph/calc/calculator.py
--rw-r--r--   0        0        0     3527 2022-03-12 22:10:52.096883 pyeph-1.1.7/pyeph/calc/labor_market/__init__.py
--rw-r--r--   0        0        0     6550 2022-04-12 00:45:04.217851 pyeph-1.1.7/pyeph/calc/poverty/__init__.py
--rw-r--r--   0        0        0      808 2022-02-20 15:56:42.705009 pyeph-1.1.7/pyeph/calc/template/__init__.py
--rw-r--r--   0        0        0      459 2022-02-20 15:56:18.416142 pyeph-1.1.7/pyeph/calc/types.py
--rw-r--r--   0        0        0       86 2022-02-21 22:57:31.475203 pyeph-1.1.7/pyeph/config.py
--rw-r--r--   0        0        0      280 2022-03-11 19:25:45.225979 pyeph-1.1.7/pyeph/errors.py
--rw-r--r--   0        0        0        0 2022-02-20 15:36:57.966306 pyeph-1.1.7/pyeph/get/__init__.py
--rw-r--r--   0        0        0       46 2022-03-04 18:03:08.085326 pyeph-1.1.7/pyeph/get/api.py
--rw-r--r--   0        0        0     2032 2022-02-20 15:56:49.141239 pyeph-1.1.7/pyeph/get/basket/__init__.py
--rw-r--r--   0        0        0      135 2022-02-20 15:56:52.185347 pyeph-1.1.7/pyeph/get/basket/constants.py
--rw-r--r--   0        0        0      180 2022-02-20 15:56:55.005448 pyeph-1.1.7/pyeph/get/equivalent_adult/__init__.py
--rw-r--r--   0        0        0     2583 2022-04-11 23:33:30.582511 pyeph-1.1.7/pyeph/get/getter.py
--rw-r--r--   0        0        0      675 2022-03-19 03:21:06.965821 pyeph-1.1.7/pyeph/get/handler.py
--rw-r--r--   0        0        0     1019 2022-04-06 19:54:07.371227 pyeph-1.1.7/pyeph/get/mautic/__init__.py
--rw-r--r--   0        0        0     1033 2022-03-19 03:25:10.143870 pyeph-1.1.7/pyeph/get/mautic/types.py
--rw-r--r--   0        0        0     1346 2022-03-12 22:11:03.864588 pyeph-1.1.7/pyeph/get/microdata/__init__.py
--rw-r--r--   0        0        0     1321 2022-02-20 16:33:36.456612 pyeph-1.1.7/pyeph/get/microdata/types.py
--rw-r--r--   0        0        0     1227 2022-03-11 19:35:46.159143 pyeph-1.1.7/pyeph/get/microdata/validator.py
--rw-r--r--   0        0        0      449 2022-02-20 15:36:57.962306 pyeph-1.1.7/pyeph/tools/.examples/canasta_ejemplo.csv
--rw-r--r--   0        0        0        0 2022-02-20 18:42:53.719410 pyeph-1.1.7/pyeph/tools/__init__.py
--rw-r--r--   0        0        0      138 2022-03-19 04:14:58.805986 pyeph-1.1.7/pyeph/tools/api.py
--rw-r--r--   0        0        0     1136 2022-02-20 15:56:10.163847 pyeph-1.1.7/pyeph/tools/decorators.py
--rw-r--r--   0        0        0     2141 2022-05-30 15:46:50.426916 pyeph-1.1.7/pyeph/tools/labels.py
--rw-r--r--   0        0        0     1036 2022-05-23 23:19:14.725598 pyeph-1.1.7/pyeph/tools/merge.py
--rw-r--r--   0        0        0      829 2022-09-26 22:30:47.801070 pyeph-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     6210 2022-09-26 22:31:22.849123 pyeph-1.1.7/setup.py
--rw-r--r--   0        0        0     5897 2022-09-26 22:31:22.849409 pyeph-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4808 2023-04-12 17:03:54.288054 pyeph-1.2.0/README.md
+-rw-r--r--   0        0        0    44617 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/.files/EPH_tot_urbano_estructura_bases.xlsx
+-rw-r--r--   0        0        0       88 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/__init__.py
+-rw-r--r--   0        0        0     1452 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/ads.py
+-rw-r--r--   0        0        0      105 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/api.py
+-rw-r--r--   0        0        0     1863 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/calculator.py
+-rw-r--r--   0        0        0     3527 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/labor_market/__init__.py
+-rw-r--r--   0        0        0     6550 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/poverty/__init__.py
+-rw-r--r--   0        0        0      808 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/template/__init__.py
+-rw-r--r--   0        0        0      459 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/calc/types.py
+-rw-r--r--   0        0        0       86 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/config.py
+-rw-r--r--   0        0        0      280 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/errors.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:03:54.300055 pyeph-1.2.0/pyeph/get/__init__.py
+-rw-r--r--   0        0        0       46 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/api.py
+-rw-r--r--   0        0        0     2032 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/basket/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/basket/constants.py
+-rw-r--r--   0        0        0      180 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/equivalent_adult/__init__.py
+-rw-r--r--   0        0        0     2575 2023-04-12 17:12:12.364342 pyeph-1.2.0/pyeph/get/getter.py
+-rw-r--r--   0        0        0     2278 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/handler.py
+-rw-r--r--   0        0        0     1019 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/mautic/__init__.py
+-rw-r--r--   0        0        0     1033 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/mautic/types.py
+-rw-r--r--   0        0        0     1346 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/microdata/__init__.py
+-rw-r--r--   0        0        0     1321 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/microdata/types.py
+-rw-r--r--   0        0        0     1227 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/get/microdata/validator.py
+-rw-r--r--   0        0        0      449 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/tools/.examples/canasta_ejemplo.csv
+-rw-r--r--   0        0        0        0 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/tools/__init__.py
+-rw-r--r--   0        0        0      138 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/tools/api.py
+-rw-r--r--   0        0        0     1136 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/tools/decorators.py
+-rw-r--r--   0        0        0     2141 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/tools/labels.py
+-rw-r--r--   0        0        0     1036 2023-04-12 17:03:54.304055 pyeph-1.2.0/pyeph/tools/merge.py
+-rw-r--r--   0        0        0      829 2023-04-12 17:37:13.406102 pyeph-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5948 1970-01-01 00:00:00.000000 pyeph-1.2.0/PKG-INFO
```

### Comparing `pyeph-1.1.7/README.md` & `pyeph-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/.files/EPH_tot_urbano_estructura_bases.xlsx` & `pyeph-1.2.0/pyeph/.files/EPH_tot_urbano_estructura_bases.xlsx`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/ads.py` & `pyeph-1.2.0/pyeph/ads.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/calc/calculator.py` & `pyeph-1.2.0/pyeph/calc/calculator.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/calc/labor_market/__init__.py` & `pyeph-1.2.0/pyeph/calc/labor_market/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/calc/poverty/__init__.py` & `pyeph-1.2.0/pyeph/calc/poverty/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/calc/template/__init__.py` & `pyeph-1.2.0/pyeph/calc/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/get/basket/__init__.py` & `pyeph-1.2.0/pyeph/get/basket/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/get/getter.py` & `pyeph-1.2.0/pyeph/get/getter.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     Retorno en .get_df()
     -------
         df : pandas.DataFrame
 			dataframe del .csv solicitado
 	"""
 
-    BASE_GITHUB_URL = "https://github.com/CocinaDeSoftware/pyeph-data/raw/master/"
+    BASE_GITHUB_URL = "https://github.com/reflejar/pyeph-data/raw/master/"
     URL_INDEC = "https://www.indec.gob.ar/ftp/cuadros/menusuperior/eph"
     DEFAULT_DIR = "pyeph/.db"
 
     @property
     def download_base_folder(self):
         # ruta/completa/db/
         return os.path.join(MODULE_PATH, self.DEFAULT_DIR)
```

### Comparing `pyeph-1.1.7/pyeph/get/mautic/__init__.py` & `pyeph-1.2.0/pyeph/get/mautic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/get/mautic/types.py` & `pyeph-1.2.0/pyeph/get/mautic/types.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/get/microdata/__init__.py` & `pyeph-1.2.0/pyeph/get/microdata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/get/microdata/types.py` & `pyeph-1.2.0/pyeph/get/microdata/types.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/get/microdata/validator.py` & `pyeph-1.2.0/pyeph/get/microdata/validator.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/tools/decorators.py` & `pyeph-1.2.0/pyeph/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/tools/labels.py` & `pyeph-1.2.0/pyeph/tools/labels.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyeph/tools/merge.py` & `pyeph-1.2.0/pyeph/tools/merge.py`

 * *Files identical despite different names*

### Comparing `pyeph-1.1.7/pyproject.toml` & `pyeph-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyeph"
-version = "v1.1.7"
+version = "v1.2.0"
 description = "PyEPH es una librería para el procesamiento de la Encuesta Permanente de Hogares (eph) en Python. Permite la descarga de archivos de EPH's y otros como la canasta basica y adulto equivalente , como asi también algunos calculos rápidos relacionados con las mismas"
 authors = ["Maria Carolina Trogliero, Mariano Valdez Anopa, Maria Gaska"]
 license = "MIT"
 homepage = "https://github.com/institutohumai/pyeph/"
 readme = "README.md"
 documentation = "https://pyeph.readthedocs.io/es/latest/"
```

### Comparing `pyeph-1.1.7/setup.py` & `pyeph-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,132 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyeph
+Version: 1.2.0
+Summary: PyEPH es una librería para el procesamiento de la Encuesta Permanente de Hogares (eph) en Python. Permite la descarga de archivos de EPH's y otros como la canasta basica y adulto equivalente , como asi también algunos calculos rápidos relacionados con las mismas
+Home-page: https://github.com/institutohumai/pyeph/
+License: MIT
+Author: Maria Carolina Trogliero, Mariano Valdez Anopa, Maria Gaska
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ipykernel (>=6.13.0,<7.0.0)
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: pandas (>=1.1.5,<2.0.0)
+Requires-Dist: wget (>=3.2,<4.0)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
+Project-URL: Documentation, https://pyeph.readthedocs.io/es/latest/
+Description-Content-Type: text/markdown
 
-packages = \
-['pyeph',
- 'pyeph.calc',
- 'pyeph.calc.labor_market',
- 'pyeph.calc.poverty',
- 'pyeph.calc.template',
- 'pyeph.get',
- 'pyeph.get.basket',
- 'pyeph.get.equivalent_adult',
- 'pyeph.get.mautic',
- 'pyeph.get.microdata',
- 'pyeph.tools']
-
-package_data = \
-{'': ['*'], 'pyeph': ['.files/*'], 'pyeph.tools': ['.examples/*']}
-
-install_requires = \
-['ipykernel>=6.13.0,<7.0.0',
- 'openpyxl>=3.0.10,<4.0.0',
- 'pandas>=1.1.5,<2.0.0',
- 'wget>=3.2,<4.0',
- 'xlrd>=2.0.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pyeph',
-    'version': '1.1.7',
-    'description': "PyEPH es una librería para el procesamiento de la Encuesta Permanente de Hogares (eph) en Python. Permite la descarga de archivos de EPH's y otros como la canasta basica y adulto equivalente , como asi también algunos calculos rápidos relacionados con las mismas",
-    'long_description': '# PyEPH - Libreria para el procesamiento de la Encuesta Permanente de Hogares en Python \n<a><img src=\'docs/_static/logo.png\' align="right" height="250" /></a>\n\n![PyPI](https://img.shields.io/pypi/v/pyeph?color=orange&)\n![PyPI - License](https://img.shields.io/pypi/l/pyeph?color=purple&)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyeph?)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/pyeph?)\n[![Downloads](https://static.pepy.tech/personalized-badge/pyeph?period=total&units=none&left_color=grey&right_color=yellowgreen&left_text=downloads)](https://pepy.tech/project/pyeph)\n[![Documentation Status](https://readthedocs.org/projects/pyeph/badge/?version=latest)](https://pyeph.readthedocs.io/es/latest/?badge=latest)\n[![DOI](https://zenodo.org/badge/461306367.svg)](https://zenodo.org/badge/latestdoi/461306367)\n\nLa librería Pyeph tiene como objetivo facilitar el procesamiento en Python de las [Encuesta Permanente de Hogares (eph)](https://www.indec.gob.ar/indec/web/Institucional-Indec-BasesDeDatos) publicadas por INDEC de forma periódica. Está pensada como un espacio donde se nuclean y centralizan los cálculos vinculados a las mismas para posteriormente ser utilizadas en investigaciones, artículos, publicaciones, etc.\nEs una librería que hace principal hincapié en la transparencia metodológica utilizando licencias de código abierto y que promueve la colaboración de las comunidades de cientístas de datos, sociales, investigadorxs, desarrolladorxs, periodistas y demás curiosxs.\n\nPermite la descarga de archivos de `EPH\'s` y otros como la `canasta basica` y `adulto equivalente` , como asi también algunos calculos rápidos relacionados con las mismas\n\n## Cómo citar la librería\n\n```\nCarolina Trogliero, Mariano Valdez y Maria Frances Gaska (2022). PyEPH: Librería para la obtención y el procesamiento de la Encuesta Permanente de Hogares (EPH-INDEC). PyEPH version https://doi.org/10.5281/zenodo.6727908\n```\n\n\n## Instalación\n\nPueden probar nuestra notebook de ejemplo en Google Colab\n\n<a href="https://colab.research.google.com/github/institutohumai/pyeph/blob/main/examples.ipynb" target="_blank"> <img src=\'https://colab.research.google.com/assets/colab-badge.svg\' /> </a>\n\nRecordá abrir en una nueva pestaña\n\n### Prerequisitos\n- [Python 3](https://www.python.org/)\n- [pip](https://www.pypi.org/)\n### Instalando PyEPH\n\n- Abra una terminal del sistema y escriba \n\n```bash\n$ pip install pyeph\n```\n\n## Uso básico\n\nLos siguientes son algunos ejemplos de uso. Para ver todos los cálculos podés ir para la documentación\n\nEn inglés\n\n```python\nimport pyeph\n\n# Obtención\neph = pyeph.get(data="eph", year=2021, period=2, base_type=\'individual\') # EPH individual\nbasket = pyeph.get(data="canastas") # canasta basica total y alimentaria\nadequi = pyeph.get(data="adulto-equivalente") # adulto equivalente\n\n# Cálculos de ejemplo de pobreza \npoverty = pyeph.Poverty(eph, basket)\npopulation_poverty = poverty.population(group_by=\'CH04\') # Población pobre por sexo \nlabeled_poverty = pyeph.map_labels(population_poverty) # Etiquetado de las variables\n\n# Cálculos de Mercado Laboral\nlabor_market = pyeph.LaborMarket(eph)\nunemployment = labor_market.unemployment(group_by="REGION", div_by="PT") # Desempleo agrupado por region y dividiendo por Población Total\nlabeled_unemployment = pyeph.map_labels(unemployment) # Etiquetado de las variables\n```\n\nEn español\n\n```python\nimport pyeph\n\n# Obtención\neph = pyeph.obtener(data="eph", ano=2021, periodo=2, tipo_base=\'individual\') # EPH individual\ncanastas = pyeph.obtener(data="canastas") # canasta basica total y alimentaria\nadequi = pyeph.obtener(data="adulto-equivalente") # adulto equivalente\n\n# Cálculos de ejemplo de pobreza \npobreza = pyeph.Pobreza(eph, canastas)\npoblacion_pobre = pobreza.poblacion(agrupar_por=\'CH04\') # Población pobre por sexo \npoblacion_pobre_etiquetado = pyeph.etiquetar(poblacion_pobre) # Etiquetado de las variables\n\n# Cálculos de Mercado Laboral\nmercado_laboral = pyeph.MercadoLaboral(eph)\ndesempleo = mercado_laboral.desempleo(agrupar_por="REGION", div_por="PT") # Desempleo agrupado por region y dividiendo por Población Total\ndesempleo_etiquetado = pyeph.etiquetar(desempleo) # Etiquetado de las variables\n```\n\n## Documentación\n\n[Link del sitio de la documentación](https://pyeph.readthedocs.io/es/latest/) \n\n---\n\n### Tenga en cuenta\n\nEsta librería se encuentra en estado permanente de desarrollo.\n\n> Cualquier colaboración es bienvenida\n\n\n## Agradecimientos\n\nDejamos aquí un especial agradecimiento al equipo de desarrollo de la librería [EPH en R](https://holatam.github.io/eph/authors.html). Todo el amor para elles ❤️ y a  [Rami Argañaraz](https://www.linkedin.com/in/ramiro-arga%C3%B1araz-57764a16b/) por armarnos el loguito 😻 \n\n---\n⌨️ con ❤️\n\n',
-    'author': 'Maria Carolina Trogliero, Mariano Valdez Anopa, Maria Gaska',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/institutohumai/pyeph/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+# PyEPH - Libreria para el procesamiento de la Encuesta Permanente de Hogares en Python 
+<a><img src='docs/_static/logo.png' align="right" height="250" /></a>
+
+![PyPI](https://img.shields.io/pypi/v/pyeph?color=orange&)
+![PyPI - License](https://img.shields.io/pypi/l/pyeph?color=purple&)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyeph?)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyeph?)
+[![Downloads](https://static.pepy.tech/personalized-badge/pyeph?period=total&units=none&left_color=grey&right_color=yellowgreen&left_text=downloads)](https://pepy.tech/project/pyeph)
+[![Documentation Status](https://readthedocs.org/projects/pyeph/badge/?version=latest)](https://pyeph.readthedocs.io/es/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/461306367.svg)](https://zenodo.org/badge/latestdoi/461306367)
+
+La librería Pyeph tiene como objetivo facilitar el procesamiento en Python de las [Encuesta Permanente de Hogares (eph)](https://www.indec.gob.ar/indec/web/Institucional-Indec-BasesDeDatos) publicadas por INDEC de forma periódica. Está pensada como un espacio donde se nuclean y centralizan los cálculos vinculados a las mismas para posteriormente ser utilizadas en investigaciones, artículos, publicaciones, etc.
+Es una librería que hace principal hincapié en la transparencia metodológica utilizando licencias de código abierto y que promueve la colaboración de las comunidades de cientístas de datos, sociales, investigadorxs, desarrolladorxs, periodistas y demás curiosxs.
+
+Permite la descarga de archivos de `EPH's` y otros como la `canasta basica` y `adulto equivalente` , como asi también algunos calculos rápidos relacionados con las mismas
+
+## Cómo citar la librería
+
+```
+Carolina Trogliero, Mariano Valdez y Maria Frances Gaska (2022). PyEPH: Librería para la obtención y el procesamiento de la Encuesta Permanente de Hogares (EPH-INDEC). PyEPH version https://doi.org/10.5281/zenodo.6727908
+```
+
+
+## Instalación
+
+Pueden probar nuestra notebook de ejemplo en Google Colab
+
+<a href="https://colab.research.google.com/github/institutohumai/pyeph/blob/main/examples.ipynb" target="_blank"> <img src='https://colab.research.google.com/assets/colab-badge.svg' /> </a>
+
+Recordá abrir en una nueva pestaña
+
+### Prerequisitos
+- [Python 3](https://www.python.org/)
+- [pip](https://www.pypi.org/)
+### Instalando PyEPH
+
+- Abra una terminal del sistema y escriba 
+
+```bash
+$ pip install pyeph
+```
+
+## Uso básico
+
+Los siguientes son algunos ejemplos de uso. Para ver todos los cálculos podés ir para la documentación
+
+En inglés
+
+```python
+import pyeph
+
+# Obtención
+eph = pyeph.get(data="eph", year=2021, period=2, base_type='individual') # EPH individual
+basket = pyeph.get(data="canastas") # canasta basica total y alimentaria
+adequi = pyeph.get(data="adulto-equivalente") # adulto equivalente
+
+# Cálculos de ejemplo de pobreza 
+poverty = pyeph.Poverty(eph, basket)
+population_poverty = poverty.population(group_by='CH04') # Población pobre por sexo 
+labeled_poverty = pyeph.map_labels(population_poverty) # Etiquetado de las variables
+
+# Cálculos de Mercado Laboral
+labor_market = pyeph.LaborMarket(eph)
+unemployment = labor_market.unemployment(group_by="REGION", div_by="PT") # Desempleo agrupado por region y dividiendo por Población Total
+labeled_unemployment = pyeph.map_labels(unemployment) # Etiquetado de las variables
+```
+
+En español
+
+```python
+import pyeph
+
+# Obtención
+eph = pyeph.obtener(data="eph", ano=2021, periodo=2, tipo_base='individual') # EPH individual
+canastas = pyeph.obtener(data="canastas") # canasta basica total y alimentaria
+adequi = pyeph.obtener(data="adulto-equivalente") # adulto equivalente
+
+# Cálculos de ejemplo de pobreza 
+pobreza = pyeph.Pobreza(eph, canastas)
+poblacion_pobre = pobreza.poblacion(agrupar_por='CH04') # Población pobre por sexo 
+poblacion_pobre_etiquetado = pyeph.etiquetar(poblacion_pobre) # Etiquetado de las variables
+
+# Cálculos de Mercado Laboral
+mercado_laboral = pyeph.MercadoLaboral(eph)
+desempleo = mercado_laboral.desempleo(agrupar_por="REGION", div_por="PT") # Desempleo agrupado por region y dividiendo por Población Total
+desempleo_etiquetado = pyeph.etiquetar(desempleo) # Etiquetado de las variables
+```
+
+## Documentación
+
+[Link del sitio de la documentación](https://pyeph.readthedocs.io/es/latest/) 
+
+---
+
+### Tenga en cuenta
+
+Esta librería se encuentra en estado permanente de desarrollo.
+
+> Cualquier colaboración es bienvenida
+
+
+## Agradecimientos
+
+Dejamos aquí un especial agradecimiento al equipo de desarrollo de la librería [EPH en R](https://holatam.github.io/eph/authors.html). Todo el amor para elles ❤️ y a  [Rami Argañaraz](https://www.linkedin.com/in/ramiro-arga%C3%B1araz-57764a16b/) por armarnos el loguito 😻 
+
+---
+⌨️ con ❤️
 
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,82 +1,77 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['pyeph',
-'pyeph.calc', 'pyeph.calc.labor_market', 'pyeph.calc.poverty',
-'pyeph.calc.template', 'pyeph.get', 'pyeph.get.basket',
-'pyeph.get.equivalent_adult', 'pyeph.get.mautic', 'pyeph.get.microdata',
-'pyeph.tools'] package_data = \ {'': ['*'], 'pyeph': ['.files/*'],
-'pyeph.tools': ['.examples/*']} install_requires = \
-['ipykernel>=6.13.0,<7.0.0', 'openpyxl>=3.0.10,<4.0.0', 'pandas>=1.1.5,<2.0.0',
-'wget>=3.2,<4.0', 'xlrd>=2.0.1,<3.0.0'] setup_kwargs = { 'name': 'pyeph',
-'version': '1.1.7', 'description': "PyEPH es una librerÃ­a para el
-procesamiento de la Encuesta Permanente de Hogares (eph) en Python. Permite la
-descarga de archivos de EPH's y otros como la canasta basica y adulto
-equivalente , como asi tambiÃ©n algunos calculos rÃ¡pidos relacionados con las
-mismas", 'long_description': '# PyEPH - Libreria para el procesamiento de la
-Encuesta Permanente de Hogares en Python \n[\'docs/_static/logo.png\']\n\n!
-[PyPI](https://img.shields.io/pypi/v/pyeph?color=orange&)\n![PyPI - License]
-(https://img.shields.io/pypi/l/pyeph?color=purple&)\n![PyPI - Python Version]
-(https://img.shields.io/pypi/pyversions/pyeph?)\n![PyPI - Downloads](https://
-img.shields.io/pypi/dm/pyeph?)\n[![Downloads](https://static.pepy.tech/
-personalized-badge/
+Metadata-Version: 2.1 Name: pyeph Version: 1.2.0 Summary: PyEPH es una
+librerÃ­a para el procesamiento de la Encuesta Permanente de Hogares (eph) en
+Python. Permite la descarga de archivos de EPH's y otros como la canasta basica
+y adulto equivalente , como asi tambiÃ©n algunos calculos rÃ¡pidos relacionados
+con las mismas Home-page: https://github.com/institutohumai/pyeph/ License: MIT
+Author: Maria Carolina Trogliero, Mariano Valdez Anopa, Maria Gaska Requires-
+Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ipykernel (>=6.13.0,<7.0.0) Requires-Dist: openpyxl
+(>=3.0.10,<4.0.0) Requires-Dist: pandas (>=1.1.5,<2.0.0) Requires-Dist: wget
+(>=3.2,<4.0) Requires-Dist: xlrd (>=2.0.1,<3.0.0) Project-URL: Documentation,
+https://pyeph.readthedocs.io/es/latest/ Description-Content-Type: text/markdown
+# PyEPH - Libreria para el procesamiento de la Encuesta Permanente de Hogares
+en Python [docs/_static/logo.png] ![PyPI](https://img.shields.io/pypi/v/
+pyeph?color=orange&) ![PyPI - License](https://img.shields.io/pypi/l/
+pyeph?color=purple&) ![PyPI - Python Version](https://img.shields.io/pypi/
+pyversions/pyeph?) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyeph?)
+[![Downloads](https://static.pepy.tech/personalized-badge/
 pyeph?period=total&units=none&left_color=grey&right_color=yellowgreen&left_text=downloads)]
-(https://pepy.tech/project/pyeph)\n[![Documentation Status](https://
+(https://pepy.tech/project/pyeph) [![Documentation Status](https://
 readthedocs.org/projects/pyeph/badge/?version=latest)](https://
-pyeph.readthedocs.io/es/latest/?badge=latest)\n[![DOI](https://zenodo.org/
-badge/461306367.svg)](https://zenodo.org/badge/latestdoi/461306367)\n\nLa
-librerÃ­a Pyeph tiene como objetivo facilitar el procesamiento en Python de las
-[Encuesta Permanente de Hogares (eph)](https://www.indec.gob.ar/indec/web/
-Institucional-Indec-BasesDeDatos) publicadas por INDEC de forma periÃ³dica.
-EstÃ¡ pensada como un espacio donde se nuclean y centralizan los cÃ¡lculos
-vinculados a las mismas para posteriormente ser utilizadas en investigaciones,
-artÃ­culos, publicaciones, etc.\nEs una librerÃ­a que hace principal hincapiÃ©
-en la transparencia metodolÃ³gica utilizando licencias de cÃ³digo abierto y que
+pyeph.readthedocs.io/es/latest/?badge=latest) [![DOI](https://zenodo.org/badge/
+461306367.svg)](https://zenodo.org/badge/latestdoi/461306367) La librerÃ­a
+Pyeph tiene como objetivo facilitar el procesamiento en Python de las [Encuesta
+Permanente de Hogares (eph)](https://www.indec.gob.ar/indec/web/Institucional-
+Indec-BasesDeDatos) publicadas por INDEC de forma periÃ³dica. EstÃ¡ pensada
+como un espacio donde se nuclean y centralizan los cÃ¡lculos vinculados a las
+mismas para posteriormente ser utilizadas en investigaciones, artÃ­culos,
+publicaciones, etc. Es una librerÃ­a que hace principal hincapiÃ© en la
+transparencia metodolÃ³gica utilizando licencias de cÃ³digo abierto y que
 promueve la colaboraciÃ³n de las comunidades de cientÃ­stas de datos, sociales,
-investigadorxs, desarrolladorxs, periodistas y demÃ¡s curiosxs.\n\nPermite la
-descarga de archivos de `EPH\'s` y otros como la `canasta basica` y `adulto
+investigadorxs, desarrolladorxs, periodistas y demÃ¡s curiosxs. Permite la
+descarga de archivos de `EPH's` y otros como la `canasta basica` y `adulto
 equivalente` , como asi tambiÃ©n algunos calculos rÃ¡pidos relacionados con las
-mismas\n\n## CÃ³mo citar la librerÃ­a\n\n```\nCarolina Trogliero, Mariano
-Valdez y Maria Frances Gaska (2022). PyEPH: LibrerÃ­a para la obtenciÃ³n y el
+mismas ## CÃ³mo citar la librerÃ­a ``` Carolina Trogliero, Mariano Valdez y
+Maria Frances Gaska (2022). PyEPH: LibrerÃ­a para la obtenciÃ³n y el
 procesamiento de la Encuesta Permanente de Hogares (EPH-INDEC). PyEPH version
-https://doi.org/10.5281/zenodo.6727908\n```\n\n\n## InstalaciÃ³n\n\nPueden
-probar nuestra notebook de ejemplo en Google Colab\n\n[\'https://
-colab.research.google.com/assets/colab-badge.svg\']\n\nRecordÃ¡ abrir en una
-nueva pestaÃ±a\n\n### Prerequisitos\n- [Python 3](https://www.python.org/)\n-
-[pip](https://www.pypi.org/)\n### Instalando PyEPH\n\n- Abra una terminal del
-sistema y escriba \n\n```bash\n$ pip install pyeph\n```\n\n## Uso
-bÃ¡sico\n\nLos siguientes son algunos ejemplos de uso. Para ver todos los
-cÃ¡lculos podÃ©s ir para la documentaciÃ³n\n\nEn inglÃ©s\n\n```python\nimport
-pyeph\n\n# ObtenciÃ³n\neph = pyeph.get(data="eph", year=2021, period=2,
-base_type=\'individual\') # EPH individual\nbasket = pyeph.get(data="canastas")
-# canasta basica total y alimentaria\nadequi = pyeph.get(data="adulto-
-equivalente") # adulto equivalente\n\n# CÃ¡lculos de ejemplo de pobreza
-\npoverty = pyeph.Poverty(eph, basket)\npopulation_poverty = poverty.population
-(group_by=\'CH04\') # PoblaciÃ³n pobre por sexo \nlabeled_poverty =
-pyeph.map_labels(population_poverty) # Etiquetado de las variables\n\n#
-CÃ¡lculos de Mercado Laboral\nlabor_market = pyeph.LaborMarket
-(eph)\nunemployment = labor_market.unemployment(group_by="REGION", div_by="PT")
-# Desempleo agrupado por region y dividiendo por PoblaciÃ³n
-Total\nlabeled_unemployment = pyeph.map_labels(unemployment) # Etiquetado de
-las variables\n```\n\nEn espaÃ±ol\n\n```python\nimport pyeph\n\n#
-ObtenciÃ³n\neph = pyeph.obtener(data="eph", ano=2021, periodo=2,
-tipo_base=\'individual\') # EPH individual\ncanastas = pyeph.obtener
-(data="canastas") # canasta basica total y alimentaria\nadequi = pyeph.obtener
-(data="adulto-equivalente") # adulto equivalente\n\n# CÃ¡lculos de ejemplo de
-pobreza \npobreza = pyeph.Pobreza(eph, canastas)\npoblacion_pobre =
-pobreza.poblacion(agrupar_por=\'CH04\') # PoblaciÃ³n pobre por sexo
-\npoblacion_pobre_etiquetado = pyeph.etiquetar(poblacion_pobre) # Etiquetado de
-las variables\n\n# CÃ¡lculos de Mercado Laboral\nmercado_laboral =
-pyeph.MercadoLaboral(eph)\ndesempleo = mercado_laboral.desempleo
+https://doi.org/10.5281/zenodo.6727908 ``` ## InstalaciÃ³n Pueden probar
+nuestra notebook de ejemplo en Google Colab [https://colab.research.google.com/
+assets/colab-badge.svg] RecordÃ¡ abrir en una nueva pestaÃ±a ### Prerequisitos
+- [Python 3](https://www.python.org/) - [pip](https://www.pypi.org/) ###
+Instalando PyEPH - Abra una terminal del sistema y escriba ```bash $ pip
+install pyeph ``` ## Uso bÃ¡sico Los siguientes son algunos ejemplos de uso.
+Para ver todos los cÃ¡lculos podÃ©s ir para la documentaciÃ³n En inglÃ©s
+```python import pyeph # ObtenciÃ³n eph = pyeph.get(data="eph", year=2021,
+period=2, base_type='individual') # EPH individual basket = pyeph.get
+(data="canastas") # canasta basica total y alimentaria adequi = pyeph.get
+(data="adulto-equivalente") # adulto equivalente # CÃ¡lculos de ejemplo de
+pobreza poverty = pyeph.Poverty(eph, basket) population_poverty =
+poverty.population(group_by='CH04') # PoblaciÃ³n pobre por sexo labeled_poverty
+= pyeph.map_labels(population_poverty) # Etiquetado de las variables #
+CÃ¡lculos de Mercado Laboral labor_market = pyeph.LaborMarket(eph) unemployment
+= labor_market.unemployment(group_by="REGION", div_by="PT") # Desempleo
+agrupado por region y dividiendo por PoblaciÃ³n Total labeled_unemployment =
+pyeph.map_labels(unemployment) # Etiquetado de las variables ``` En espaÃ±ol
+```python import pyeph # ObtenciÃ³n eph = pyeph.obtener(data="eph", ano=2021,
+periodo=2, tipo_base='individual') # EPH individual canastas = pyeph.obtener
+(data="canastas") # canasta basica total y alimentaria adequi = pyeph.obtener
+(data="adulto-equivalente") # adulto equivalente # CÃ¡lculos de ejemplo de
+pobreza pobreza = pyeph.Pobreza(eph, canastas) poblacion_pobre =
+pobreza.poblacion(agrupar_por='CH04') # PoblaciÃ³n pobre por sexo
+poblacion_pobre_etiquetado = pyeph.etiquetar(poblacion_pobre) # Etiquetado de
+las variables # CÃ¡lculos de Mercado Laboral mercado_laboral =
+pyeph.MercadoLaboral(eph) desempleo = mercado_laboral.desempleo
 (agrupar_por="REGION", div_por="PT") # Desempleo agrupado por region y
-dividiendo por PoblaciÃ³n Total\ndesempleo_etiquetado = pyeph.etiquetar
-(desempleo) # Etiquetado de las variables\n```\n\n## DocumentaciÃ³n\n\n[Link
-del sitio de la documentaciÃ³n](https://pyeph.readthedocs.io/es/latest/) \n\n--
--\n\n### Tenga en cuenta\n\nEsta librerÃ­a se encuentra en estado permanente de
-desarrollo.\n\n> Cualquier colaboraciÃ³n es bienvenida\n\n\n##
-Agradecimientos\n\nDejamos aquÃ­ un especial agradecimiento al equipo de
-desarrollo de la librerÃ­a [EPH en R](https://holatam.github.io/eph/
-authors.html). Todo el amor para elles â¤ï¸ y a [Rami ArgaÃ±araz](https://
-www.linkedin.com/in/ramiro-arga%C3%B1araz-57764a16b/) por armarnos el loguito
-ð» \n\n---\nâ¨ï¸ con â¤ï¸\n\n', 'author': 'Maria Carolina Trogliero,
-Mariano Valdez Anopa, Maria Gaska', 'author_email': None, 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/institutohumai/pyeph/',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+dividiendo por PoblaciÃ³n Total desempleo_etiquetado = pyeph.etiquetar
+(desempleo) # Etiquetado de las variables ``` ## DocumentaciÃ³n [Link del sitio
+de la documentaciÃ³n](https://pyeph.readthedocs.io/es/latest/) --- ### Tenga en
+cuenta Esta librerÃ­a se encuentra en estado permanente de desarrollo. >
+Cualquier colaboraciÃ³n es bienvenida ## Agradecimientos Dejamos aquÃ­ un
+especial agradecimiento al equipo de desarrollo de la librerÃ­a [EPH en R]
+(https://holatam.github.io/eph/authors.html). Todo el amor para elles â¤ï¸ y
+a [Rami ArgaÃ±araz](https://www.linkedin.com/in/ramiro-arga%C3%B1araz-
+57764a16b/) por armarnos el loguito ð» --- â¨ï¸ con â¤ï¸
```

