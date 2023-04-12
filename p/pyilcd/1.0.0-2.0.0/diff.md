# Comparing `tmp/pyilcd-1.0.0.tar.gz` & `tmp/pyilcd-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyilcd-1.0.0.tar", last modified: Tue Apr 11 15:40:38 2023, max compression
+gzip compressed data, was "pyilcd-2.0.0.tar", last modified: Wed Apr 12 13:59:58 2023, max compression
```

## Comparing `pyilcd-1.0.0.tar` & `pyilcd-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:40:38.943256 pyilcd-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-11 15:40:24.000000 pyilcd-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 15:40:24.000000 pyilcd-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-11 15:40:38.943256 pyilcd-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-11 15:40:24.000000 pyilcd-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:40:38.939257 pyilcd-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-11 15:40:24.000000 pyilcd-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:40:38.939257 pyilcd-1.0.0/pyilcd/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58784 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/process_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:40:38.943256 pyilcd-1.0.0/pyilcd/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Categories.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Documentation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_ILCD.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_Locations.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyilcd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:40:38.939257 pyilcd-1.0.0/pyilcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-11 15:40:38.000000 pyilcd-1.0.0/pyilcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-11 15:40:38.000000 pyilcd-1.0.0/pyilcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:40:38.000000 pyilcd-1.0.0/pyilcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:40:38.000000 pyilcd-1.0.0/pyilcd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 15:40:38.000000 pyilcd-1.0.0/pyilcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 15:40:38.000000 pyilcd-1.0.0/pyilcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 15:40:24.000000 pyilcd-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-11 15:40:38.947257 pyilcd-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:40:38.943256 pyilcd-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-11 15:40:24.000000 pyilcd-1.0.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 15:40:24.000000 pyilcd-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-11 15:40:24.000000 pyilcd-1.0.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-11 15:40:24.000000 pyilcd-1.0.0/tests/test_process_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.679233 pyilcd-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-12 13:59:49.000000 pyilcd-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 13:59:49.000000 pyilcd-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-12 13:59:58.679233 pyilcd-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-12 13:59:49.000000 pyilcd-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.671233 pyilcd-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-12 13:59:49.000000 pyilcd-2.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/pyilcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/process_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/pyilcd/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Categories.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Documentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_ILCD.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Locations.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/pyilcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 13:59:58.679233 pyilcd-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_process_dataset.py
```

### Comparing `pyilcd-1.0.0/LICENSE` & `pyilcd-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/PKG-INFO` & `pyilcd-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 1.0.0
+Version: 2.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-1.0.0/README.md` & `pyilcd-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/docs/conf.py` & `pyilcd-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/common.py` & `pyilcd-2.0.0/pyilcd/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -346,7 +346,62 @@
     def referenceToEntitiesWithExclusiveAccess(self) -> List["GlobalReference"]:
         """ "Contact data set" of those entities or persons (or
         groups of these), to which an exclusive access to this
         data set is granted. Mainly intended to be used in
         confidentiality management in projects. [Note: See also
         field "Access and use restrictions".]"""
         return get_element_list(self, "common:referenceToEntitiesWithExclusiveAccess")
+
+
+class FlowCategoryInformation(etree.ElementBase):
+    """Hierachical classification of the Flow property foreseen to be used
+    to structure the Flow property content of the database. (Note: This entry
+    is NOT required for the identification of the Flow property data set. It
+    should nevertheless be avoided to use identical names for Flow properties
+    in the same class."""
+
+    @property
+    def elementaryFlowCategorization(self) -> List["FlowCategorization"]:
+        """Identifying category/compartment information exclusively used for
+        elementary flows. E.g. "Emission to air", "Renewable resource", etc."""
+        return get_element_list(self, "common:elementaryFlowCategorization")
+
+    @property
+    def classifications(self) -> List["Classification"]:
+        """Optional statistical or other classification of the data set.
+        Typically also used for structuring LCA databases."""
+        return get_element_list(self, "common:classification")
+
+
+class FlowCategorization(etree.ElementBase):
+    """Identifying category/compartment information exclusively used for
+    elementary flows. E.g. "Emission to air", "Renewable resource", etc."""
+
+    name = create_attribute_process_dataset("name", str)
+    """Name of the categorization system. E.g. "ILCD 1.1" or another
+    elementary flow categorization/compartment scheme applied, as
+    defined e.g. in other LCA database (systems)."""
+
+    categories = create_attribute_process_dataset("categories", str)
+    """URL or file name of a file containing all categories of this
+    categorization system. [Note: The file is to be in form of the
+    "ILCDCategories.xml" format. If a category file is specified, only
+    categories of the referenced categories file should be used.]"""
+
+    @property
+    def categoryList(self) -> List["Category"]:
+        """Name of the category of this elementary flow.."""
+        return get_element_list(self, "common:category")
+
+
+class Category(etree.ElementBase):
+    """Name of the category of this elementary flow."""
+
+    level = create_attribute_process_dataset("level", str)
+    """Hierarchy level (1,2,...), if the categorization system
+    is hierachical, otherwise emtpy or not used."""
+
+    catId = create_attribute_process_dataset("catId", str)
+    """Unique identifier of the category. [Note: May be used by LCA
+    software for it's category system. If used the identifer should
+    be identical to the on defined in the referenced category file.
+    Identifiers can be UUIDs, but also other forms are possible.]"""
```

### Comparing `pyilcd-1.0.0/pyilcd/config.py` & `pyilcd-2.0.0/pyilcd/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,28 @@
 class Defaults:
     """Stores default values for ILCD attributes used when no value exists."""
 
     SCHEMA_DIR: ClassVar[str] = os.path.join(Path(__file__).parent.resolve(), "schemas")
     SCHEMA_PROCESS_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_ProcessDataSet.xsd"
     )
+    SCHEMA_FLOW_DATASET: ClassVar[str] = os.path.join(
+        SCHEMA_DIR, "ILCD_FlowDataSet.xsd"
+    )
 
     DYNAMIC_DEFAULTS: ClassVar[
         Dict[str, Dict[str, Callable[[etree.ElementBase], str]]]
     ] = {}
     STATIC_DEFAULTS: ClassVar[Dict[str, Dict[str, str]]] = {
         "Classification": {
             "name": "ILCD",
         },
+        "FlowCategorization": {
+            "name": "ILCD",
+        },
         "ProcessDataset": {
             "metaDataOnly": "false",
         },
     }
 
     @classmethod
     def config_defaults(cls, config_file: str) -> None:
```

### Comparing `pyilcd-1.0.0/pyilcd/helpers.py` & `pyilcd-2.0.0/pyilcd/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,37 @@
     name: str, attr_type: type, validator: Optional[Callable] = None
 ) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Process Dataset attribute"""
     return create_attribute(name, attr_type, Defaults.SCHEMA_PROCESS_DATASET, validator)
 
 
+def create_attribute_flow_dataset(
+    name: str, attr_type: type, validator: Optional[Callable] = None
+) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Flow Dataset attribute"""
+    return create_attribute(name, attr_type, Defaults.SCHEMA_FLOW_DATASET, validator)
+
+
 def create_element_text_process_dataset(name: str, element_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Process Dataset element text"""
     return create_element_text(name, element_type, Defaults.SCHEMA_PROCESS_DATASET)
 
 
+def create_element_text_flow_dataset(name: str, element_type: type) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Flow Dataset element text"""
+    return create_element_text(name, element_type, Defaults.SCHEMA_FLOW_DATASET)
+
+
 def create_attribute_list_process_dataset(name: str, attr_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Process Dataset element text list"""
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_PROCESS_DATASET)
+
+
+def create_attribute_list_flow_dataset(name: str, attr_type: type) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Flow Dataset element text list"""
+    return create_attribute_list(name, attr_type, Defaults.SCHEMA_FLOW_DATASET)
```

### Comparing `pyilcd-1.0.0/pyilcd/process_dataset.py` & `pyilcd-2.0.0/pyilcd/process_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Custom ILCD Python classes for ProcessDataset of ILCD schema."""
+"""Custom ILCD Python classes for ProcessDataSet of ILCD schema."""
 from typing import List
 
 from lxml import etree
 from lxmlh import get_element, get_element_list
 
 from .common import (
-    ClassificationInformation,
     CommissionerAndGoal,
     ComplianceGroup,
     DataEntryByGroup1,
     DataEntryByGroup2,
+    FlowCategoryInformation,
     GlobalReference,
     PublicationAndOwnershipGroup1,
     PublicationAndOwnershipGroup2,
     PublicationAndOwnershipGroup3,
     ValidationGroup1,
     ValidationGroup3,
 )
@@ -235,19 +235,19 @@
     type of emission source from which the elementary flows of the Inputs and Outputs
     stems (e.g. "incineration-related", "transport-related", etc.). Together with the
     field "Complementing processes" this allows to split up a process data set into a
     number of clearly identified data sets, each carrying only a part of the inventory
     and that together represent the complete inventory. Care has to be taken when
     naming the reference flow, to avoid misinterpretation.."""
 
-    commonSynonyms = create_attribute_list_process_dataset("common:synonyms", str)
+    synonyms = create_attribute_list_process_dataset("common:synonyms", str)
     """Synonyms / alternative names / brands of the good, service, or
     process. Separated by semicolon."""
 
-    commonGeneralComment = create_attribute_list_process_dataset(
+    generalComments = create_attribute_list_process_dataset(
         "common:generalComment", str
     )
     """General information about the data set, including e.g. general
     (internal, not reviewed) quality statements as well as information sources used.
     (Note: Please also check the more specific fields e.g. on "Intended application",
     "Advice on data set use" and the fields in the "Modelling and validation" section
     to avoid overlapping entries.)"""
@@ -262,15 +262,15 @@
         """Process data set(s)" that complement this partial / sub-set of a
         complete process data set, if any and available as separate data set(s). The
         identifying name of this sub-set should be stated in the field "Identifier of
         sub-data set"."""
         return get_element(self, "complementingProcesses")
 
     @property
-    def classificationInformation(self) -> "ClassificationInformation":
+    def classificationInformation(self) -> "FlowCategoryInformation":
         """Hierarchical classification of the good, service, or process.
         (Note: This entry is NOT required for the identification of a Process. It should
         nevertheless be avoided to use identical names for Processes in the same
         category."""
         return get_element(self, "classificationInformation")
 
     @property
```

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Categories.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Categories.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Documentation.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Documentation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_ILCD.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_ILCD.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_Locations.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_Locations.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd` & `pyilcd-2.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/pyilcd.egg-info/PKG-INFO` & `pyilcd-2.0.0/pyilcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 1.0.0
+Version: 2.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-1.0.0/pyilcd.egg-info/SOURCES.txt` & `pyilcd-2.0.0/pyilcd.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 ./docs/conf.py
 ./pyilcd/__init__.py
 ./pyilcd/common.py
 ./pyilcd/config.py
 ./pyilcd/core.py
+./pyilcd/flow_dataset.py
 ./pyilcd/helpers.py
 ./pyilcd/process_dataset.py
 ./pyilcd/utils.py
 pyilcd/VERSION
 pyilcd.egg-info/PKG-INFO
 pyilcd.egg-info/SOURCES.txt
 pyilcd.egg-info/dependency_links.txt
@@ -33,8 +34,9 @@
 pyilcd/schemas/ILCD_Locations.xsd
 pyilcd/schemas/ILCD_ProcessDataSet.xsd
 pyilcd/schemas/ILCD_SourceDataSet.xsd
 pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
 tests/test_common.py
 tests/test_config.py
 tests/test_core.py
+tests/test_flow_dataset.py
 tests/test_process_dataset.py
```

### Comparing `pyilcd-1.0.0/setup.cfg` & `pyilcd-2.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 include_package_data = True
 package_dir = 
 	=.
 python_requires = >=3.8
 install_requires = 
 	lxml==4.9.2
 	lxmlh==1.1.0
+	pycasreg==0.1.0
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `pyilcd-1.0.0/tests/test_common.py` & `pyilcd-2.0.0/tests/test_flow_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-"""Test cases for the __common__ module."""
-from pyilcd.common import Class, DataQualityIndicator, GlobalReference, Method
-from pyilcd.process_dataset import ProcessDataSet
+"""Test cases for the __flow_dataset__ module."""
+from pyilcd.common import GlobalReference
+from pyilcd.flow_dataset import (
+    Compliance,
+    DataEntryBy,
+    FlowCategoryInformation,
+    FlowDataSet,
+    Geography,
+    LCIMethod,
+    Name,
+    QuantitativeReference,
+)
 
 
-def test_process_information(process_dataset: ProcessDataSet) -> None:
+def test_flow_information(flow_dataset: FlowDataSet) -> None:
     """It parses attributes correctly."""
-    dataSetInformation = process_dataset.processInformation.dataSetInformation
-    classificationInformation = dataSetInformation.classificationInformation
+    flowInformation = flow_dataset.flowInformation
+    datasetInformation = flowInformation.dataSetInformation
+    quantitativeReference = flowInformation.quantitativeReference
+    technology = flowInformation.technology
+    geography = flowInformation.geography
 
+    assert isinstance(datasetInformation.name, Name)
     assert isinstance(
-        classificationInformation.classifications[0].classesList[0], Class
+        datasetInformation.classificationInformation, FlowCategoryInformation
     )
+    assert isinstance(quantitativeReference, QuantitativeReference)
+    assert isinstance(geography, Geography)
+    assert isinstance(technology.referenceToTechnicalSpecification[0], GlobalReference)
 
 
-def test_modelling_and_validation(process_dataset: ProcessDataSet) -> None:
+def test_modelling_and_validation(flow_dataset: FlowDataSet) -> None:
     """It parses attributes correctly."""
-    modellingAndValidation = process_dataset.modellingAndValidation
-    review = modellingAndValidation.validation.reviews[0]
-    compliance = modellingAndValidation.complianceDeclarations.compliances[0]
+    modellingAndValidation = flow_dataset.modellingAndValidation
 
-    assert isinstance(review.scope.method[0], Method)
+    assert isinstance(modellingAndValidation.lciMethod, LCIMethod)
     assert isinstance(
-        review.dataQualityIndicators.dataQualityIndicators[0], DataQualityIndicator
+        modellingAndValidation.complianceDeclarations.compliances[0], Compliance
     )
-    assert isinstance(review.referenceToCompleteReviewReport, GlobalReference)
-    assert isinstance(review.referenceToNameOfReviewerAndInstitution, GlobalReference)
-    assert isinstance(compliance.referenceToComplianceSystem, GlobalReference)
 
 
-def test_administrative_information(process_dataset: ProcessDataSet) -> None:
+def test_administrative_information(flow_dataset: FlowDataSet) -> None:
     """It parses attributes correctly."""
-    administrativeInformation = process_dataset.administrativeInformation
-    commissionerAndGoal = administrativeInformation.commissionerAndGoal
-    dataEntryBy = administrativeInformation.dataEntryBy
-    publicationAndOwnership = administrativeInformation.publicationAndOwnership
+    administrativeInformation = flow_dataset.administrativeInformation
 
-    assert isinstance(commissionerAndGoal.referenceToCommissioner[0], GlobalReference)
-    assert isinstance(dataEntryBy.referenceToDataSetFormat[0], GlobalReference)
+    assert isinstance(administrativeInformation.dataEntryBy, DataEntryBy)
     assert isinstance(
-        dataEntryBy.referenceToPersonOrEntityEnteringTheData, GlobalReference
-    )
-    assert isinstance(
-        publicationAndOwnership.referenceToPrecedingDataSetVersion[0], GlobalReference
-    )
-    assert isinstance(
-        publicationAndOwnership.referenceToUnchangedRepublication, GlobalReference
-    )
-    assert isinstance(
-        publicationAndOwnership.referenceToEntitiesWithExclusiveAccess[0],
+        administrativeInformation.publicationAndOwnership.referenceToOwnershipOfDataSet,
         GlobalReference,
     )
+
+
+def test_flow_properties(flow_dataset: FlowDataSet) -> None:
+    """It parses attributes correctly."""
+    flowProperty = flow_dataset.flowProperties.flowProperties[0]
+
+    assert isinstance(flowProperty.referenceToFlowPropertyDataSet, GlobalReference)
```

### Comparing `pyilcd-1.0.0/tests/test_config.py` & `pyilcd-2.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyilcd-1.0.0/tests/test_core.py` & `pyilcd-2.0.0/tests/test_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,44 +2,62 @@
 import os
 import tempfile
 from io import StringIO
 
 import pytest
 
 from pyilcd.core import (
-    ProcessDatasetLookup,
+    _check_common_lookup,
     parse_file_process_dataset,
     save_ilcd_file,
+    validate_file_flow_dataset,
     validate_file_process_dataset,
 )
 
 
-def test_parse_file_process_dataset_key_error() -> None:
+def test_check_common_lookup() -> None:
     """It validates file successfully."""
     with pytest.raises(KeyError):
-        ProcessDatasetLookup().lookup("", "", "", "undefined")
+        _check_common_lookup("undefined")
 
 
 def test_validate_file_process_dataset_success() -> None:
     """It validates file successfully."""
     assert validate_file_process_dataset("data/sample_process.xml") is None
 
 
+def test_validate_file_flow_dataset_success() -> None:
+    """It validates file successfully."""
+    assert validate_file_flow_dataset("data/sample_flow.xml") is None
+
+
 def test_validate_file_process_dataset_fail() -> None:
     """It validates file successfully."""
     xml = StringIO("<ilcd></ilcd>")
     errorExpected = (
         "<string>:1:0:ERROR:SCHEMASV:SCHEMAV_CVC_ELT_1: Element 'ilcd': "
         "No matching global declaration available for the validation root."
     )
     errorActual = validate_file_process_dataset(xml)
     assert errorActual is not None
     assert str(errorActual[0]) == errorExpected
 
 
+def test_validate_file_flow_dataset_fail() -> None:
+    """It validates file successfully."""
+    xml = StringIO("<ilcd></ilcd>")
+    errorExpected = (
+        "<string>:1:0:ERROR:SCHEMASV:SCHEMAV_CVC_ELT_1: Element 'ilcd': "
+        "No matching global declaration available for the validation root."
+    )
+    errorActual = validate_file_flow_dataset(xml)
+    assert errorActual is not None
+    assert str(errorActual[0]) == errorExpected
+
+
 def test_save_ilcd_file() -> None:
     """It saves read file correctly."""
     inputPath = "data/sample_process.xml"
     processDataset = parse_file_process_dataset(inputPath)
     outputPath = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
     save_ilcd_file(processDataset, outputPath, fill_defaults=False)
```

### Comparing `pyilcd-1.0.0/tests/test_process_dataset.py` & `pyilcd-2.0.0/tests/test_process_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Test cases for the __process_dataset__ module."""
-from pyilcd.common import GlobalReference
+from pyilcd.common import ClassificationInformation, GlobalReference
 from pyilcd.process_dataset import (
     Allocation,
-    ClassificationInformation,
     CommissionerAndGoal,
     CompletenessElementaryFlows,
     Compliance,
     LocationOfOperationSupplyOrProduction,
     Name,
     ProcessDataSet,
     QuantitativeReference,
```

