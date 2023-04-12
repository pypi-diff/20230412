# Comparing `tmp/feynml-0.1.2.tar.gz` & `tmp/feynml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynml-0.1.2.tar", max compression
+gzip compressed data, was "feynml-0.1.3.tar", max compression
```

## Comparing `feynml-0.1.2.tar` & `feynml-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-03-22 21:30:32.607900 feynml-0.1.2/LICENSE
--rw-r--r--   0        0        0     2359 2023-03-22 21:30:32.607900 feynml-0.1.2/README.md
--rw-r--r--   0        0        0      179 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/__init__.py
--rw-r--r--   0        0        0      960 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/connector.py
--rw-r--r--   0        0        0     6455 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/feynmandiagram.py
--rw-r--r--   0        0        0     2716 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/feynml.py
--rw-r--r--   0        0        0      651 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/id.py
--rw-r--r--   0        0        0        0 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/interface/__init__.py
--rw-r--r--   0        0        0     1563 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/interface/hepmc.py
--rw-r--r--   0        0        0     1569 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/interface/qgraf.py
--rw-r--r--   0        0        0     1035 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/leg.py
--rw-r--r--   0        0        0      303 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/line.py
--rw-r--r--   0        0        0      563 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/momentum.py
--rw-r--r--   0        0        0     1385 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/particles.py
--rw-r--r--   0        0        0     3115 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/pdgid.py
--rw-r--r--   0        0        0      846 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/point.py
--rw-r--r--   0        0        0      207 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/propagator.py
--rw-r--r--   0        0        0      363 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/sourcing.py
--rw-r--r--   0        0        0     2932 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/style.py
--rw-r--r--   0        0        0      364 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/targeting.py
--rw-r--r--   0        0        0     4181 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/types.py
--rw-r--r--   0        0        0      398 2023-03-22 21:30:32.607900 feynml-0.1.2/feynml/vertex.py
--rw-r--r--   0        0        0     1641 2023-03-22 21:30:34.379922 feynml-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 feynml-0.1.2/setup.py
--rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 feynml-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 05:50:36.884966 feynml-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2359 2023-04-12 05:50:36.884966 feynml-0.1.3/README.md
+-rw-r--r--   0        0        0      179 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/__init__.py
+-rw-r--r--   0        0        0      986 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/connector.py
+-rw-r--r--   0        0        0     6456 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/feynmandiagram.py
+-rw-r--r--   0        0        0     2716 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/feynml.py
+-rw-r--r--   0        0        0      651 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/id.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/interface/__init__.py
+-rw-r--r--   0        0        0     1563 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/interface/hepmc.py
+-rw-r--r--   0        0        0     1569 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/interface/qgraf.py
+-rw-r--r--   0        0        0      385 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/labeled.py
+-rw-r--r--   0        0        0     1035 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/leg.py
+-rw-r--r--   0        0        0      303 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/line.py
+-rw-r--r--   0        0        0      563 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/momentum.py
+-rw-r--r--   0        0        0     1385 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/particles.py
+-rw-r--r--   0        0        0     3115 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/pdgid.py
+-rw-r--r--   0        0        0      846 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/point.py
+-rw-r--r--   0        0        0      207 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/propagator.py
+-rw-r--r--   0        0        0      363 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/sourcing.py
+-rw-r--r--   0        0        0     2749 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/styled.py
+-rw-r--r--   0        0        0      364 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/targeting.py
+-rw-r--r--   0        0        0     4181 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/types.py
+-rw-r--r--   0        0        0      425 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/vertex.py
+-rw-r--r--   0        0        0     1641 2023-04-12 05:50:39.340987 feynml-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 feynml-0.1.3/setup.py
+-rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 feynml-0.1.3/PKG-INFO
```

### Comparing `feynml-0.1.2/LICENSE` & `feynml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/README.md` & `feynml-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/connector.py` & `feynml-0.1.3/feynml/connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 from smpl_util.util import withify
 
+from feynml.labeled import Labeled
 from feynml.momentum import Momentum
 from feynml.pdgid import PDG
-from feynml.style import Labeled, Styled
+from feynml.styled import Styled
 
 
 @withify()
 @dataclass
 class Connector(Labeled, Styled, PDG):
     momentum: Optional[Momentum] = field(
         default=None, metadata={"name": "momentum", "type": "Element"}
@@ -22,12 +23,12 @@
 
     def get_tension(self):
         """Get tension of the connector"""
         return self.get_style_property("tension")
 
     def with_length(self, length: float):
         """Add length to the connector"""
-        return self.with_styles_properties(length=length)
+        return self.with_style_properties(length=length)
 
     def get_length(self):
         """Get length of the connector"""
         return self.get_style_property("length")
```

### Comparing `feynml-0.1.2/feynml/feynmandiagram.py` & `feynml-0.1.3/feynml/feynmandiagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from feynml.id import Identifiable
 from feynml.leg import Leg
 from feynml.propagator import Propagator
-from feynml.style import CSSSheet, Styled
+from feynml.styled import CSSSheet, Styled
 from feynml.vertex import Vertex
 
 from .types import get_default_sheet
 
 # We don't want to see the cssutils warnings, since we have custom properties
 cssutils.log.setLevel(logging.CRITICAL)
```

### Comparing `feynml-0.1.2/feynml/feynml.py` & `feynml-0.1.3/feynml/feynml.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/id.py` & `feynml-0.1.3/feynml/id.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/interface/hepmc.py` & `feynml-0.1.3/feynml/interface/hepmc.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/interface/qgraf.py` & `feynml-0.1.3/feynml/interface/qgraf.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/leg.py` & `feynml-0.1.3/feynml/leg.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/momentum.py` & `feynml-0.1.3/feynml/momentum.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/particles.py` & `feynml-0.1.3/feynml/particles.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/pdgid.py` & `feynml-0.1.3/feynml/pdgid.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/point.py` & `feynml-0.1.3/feynml/point.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/feynml/style.py` & `feynml-0.1.3/feynml/styled.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,14 @@
 from smpl_doc.doc import deprecated
 from smpl_util.util import withify
 from xsdata.formats.converter import Converter, converter
 
 # We don't want to see the cssutils warnings, since we have custom properties
 cssutils.log.setLevel(logging.CRITICAL)
 
-
-@withify()
-@dataclass
-class Labeled:
-    label: Optional[str] = field(
-        default=None, metadata={"xml_attribute": True, "type": "Attribute"}
-    )
-    """Label the object"""
-
-
 CSSString = cssutils.css.CSSStyleDeclaration
 CSSSheet = cssutils.css.CSSStyleSheet
 
 
 class CSSStringConverter(Converter):
     @staticmethod
     def deserialize(value: str, **kwargs) -> CSSString:
```

### Comparing `feynml-0.1.2/feynml/types.py` & `feynml-0.1.3/feynml/types.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.2/pyproject.toml` & `feynml-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynml"
-version = "0.1.2"
+version = "0.1.3"
 description = "Feynman diagram markup language"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynml"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `feynml-0.1.2/setup.py` & `feynml-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'xsdata[cli,lxml,soap]']
 
 extras_require = \
 {'interface': ['pyqgraf>=0.0.3', 'pyhepmc']}
 
 setup_kwargs = {
     'name': 'feynml',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Feynman diagram markup language',
     'long_description': '# FeynML\n\nFeynML from <https://feynml.hepforge.org/>\n\nFeynML is a project to develop an XML dialect for describing Feynman diagrams as used in quantum field theory calculations. The primary aim is to unambiguously describe the structure of a diagram in XML, giving a de facto representation for diagram structure which can be easily translated into another representation.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n\n[pypi image]: https://badge.fury.io/py/feynml.svg\n[pypi link]: https://pypi.org/project/feynml/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynml.svg\n\n[a t link]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynml&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynml&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynml?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynml/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynml',
```

### Comparing `feynml-0.1.2/PKG-INFO` & `feynml-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Feynman diagram markup language
 Home-page: https://github.com/APN-Pucky/feynml
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

