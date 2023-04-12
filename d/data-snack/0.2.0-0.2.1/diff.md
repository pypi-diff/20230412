# Comparing `tmp/data_snack-0.2.0.tar.gz` & `tmp/data_snack-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack-0.2.0.tar", last modified: Thu Apr  6 13:17:22 2023, max compression
+gzip compressed data, was "data_snack-0.2.1.tar", last modified: Wed Apr 12 13:26:00 2023, max compression
```

## Comparing `data_snack-0.2.0.tar` & `data_snack-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.422586 data_snack-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-06 13:17:09.000000 data_snack-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 13:17:09.000000 data_snack-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-06 13:17:22.422586 data_snack-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-06 13:17:09.000000 data_snack-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 13:17:09.000000 data_snack-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 13:17:09.000000 data_snack-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-06 13:17:22.422586 data_snack-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-06 13:17:09.000000 data_snack-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.410586 data_snack-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.414586 data_snack-0.2.0/src/data_snack/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.418586 data_snack-0.2.0/src/data_snack/connections/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/connections/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/connections/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/connections/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.418586 data_snack-0.2.0/src/data_snack/entities/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/entities/entity_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/entities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/entities/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/entities/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/key_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.418586 data_snack-0.2.0/src/data_snack/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/serializers/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/snack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.422586 data_snack-0.2.0/src/data_snack/wrap/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/wrap/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/wrap/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/wrap/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 13:17:09.000000 data_snack-0.2.0/src/data_snack/wrap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:17:22.418586 data_snack-0.2.0/src/data_snack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-06 13:17:22.000000 data_snack-0.2.0/src/data_snack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-06 13:17:22.000000 data_snack-0.2.0/src/data_snack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:17:22.000000 data_snack-0.2.0/src/data_snack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-06 13:17:22.000000 data_snack-0.2.0/src/data_snack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 13:17:22.000000 data_snack-0.2.0/src/data_snack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.068088 data_snack-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 13:25:50.000000 data_snack-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 13:25:50.000000 data_snack-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-12 13:26:00.068088 data_snack-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-12 13:25:50.000000 data_snack-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 13:25:50.000000 data_snack-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 13:25:50.000000 data_snack-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-12 13:26:00.068088 data_snack-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 13:25:50.000000 data_snack-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.056088 data_snack-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.060088 data_snack-0.2.1/src/data_snack/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.064088 data_snack-0.2.1/src/data_snack/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/connections/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/connections/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/connections/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.064088 data_snack-0.2.1/src/data_snack/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/entities/entity_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/entities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/entities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/entities/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.068088 data_snack-0.2.1/src/data_snack/key_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/key_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/key_factories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/key_factories/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/key_factories/non_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.068088 data_snack-0.2.1/src/data_snack/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/serializers/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/snack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.068088 data_snack-0.2.1/src/data_snack/wrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/wrap/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/wrap/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/wrap/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 13:25:50.000000 data_snack-0.2.1/src/data_snack/wrap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:26:00.064088 data_snack-0.2.1/src/data_snack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-12 13:26:00.000000 data_snack-0.2.1/src/data_snack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 13:26:00.000000 data_snack-0.2.1/src/data_snack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:26:00.000000 data_snack-0.2.1/src/data_snack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 13:26:00.000000 data_snack-0.2.1/src/data_snack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 13:26:00.000000 data_snack-0.2.1/src/data_snack.egg-info/top_level.txt
```

### Comparing `data_snack-0.2.0/LICENSE` & `data_snack-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack-0.2.0/PKG-INFO` & `data_snack-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-0.2.0/README.md` & `data_snack-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `data_snack-0.2.0/setup.cfg` & `data_snack-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack
-version = 0.2.0
+version = 0.2.1
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack
 project_urls =
```

### Comparing `data_snack-0.2.0/setup.py` & `data_snack-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.2.0/src/data_snack/connections/base.py` & `data_snack-0.2.1/src/data_snack/connections/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Protocol, Text, Union, Optional
+from typing import Any, Dict, List, Optional, Protocol, Text, Union
 
 
 class Connection(Protocol):
     """
     An interface used for by `Snack` to access db.
     If you want to create a custom connection to a db for your choosing,
     create a new class that follows this protocol.
```

### Comparing `data_snack-0.2.0/src/data_snack/connections/memcached.py` & `data_snack-0.2.1/src/data_snack/connections/memcached.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Dict, List, Text, Optional
+from typing import Dict, List, Optional, Text
 
 from .base import Connection
 
 
 @dataclass
 class MemcachedConnection(Connection):
     connection: "Client"
```

### Comparing `data_snack-0.2.0/src/data_snack/connections/redis.py` & `data_snack-0.2.1/src/data_snack/connections/redis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Dict, List, Text, Optional
+from typing import Dict, List, Optional, Text
 
 from .base import Connection
 
 
 @dataclass
 class RedisConnection(Connection):
     connection: "Redis"
```

### Comparing `data_snack-0.2.0/src/data_snack/entities/entity.py` & `data_snack-0.2.1/src/data_snack/entities/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.2.0/src/data_snack/entities/entity_meta.py` & `data_snack-0.2.1/src/data_snack/entities/entity_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from abc import ABCMeta, ABC
+from abc import ABC, ABCMeta
 
 from .exceptions import (
-    MetaFieldsException,
     MetaEmptyKeysException,
+    MetaFieldsException,
     NonExistingMetaError,
 )
 
 
 class EntityMetaClass(ABCMeta):
 
     meta_fields = ["keys", "excluded_fields"]
```

### Comparing `data_snack-0.2.0/src/data_snack/entities/schema.py` & `data_snack-0.2.1/src/data_snack/entities/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Dict, Any, Callable, Type, get_type_hints
+from typing import Any, Callable, Dict, Type, get_type_hints
 
 from data_snack.entities import Entity
 
-
 EntitySchemaGetter = Callable[[Type[Entity], bool], Dict[str, Any]]
 
 
 def get_entity_schema(
     entity_type: Type[Entity], exclude_fields: bool = False
 ) -> Dict[str, Any]:
     """
```

### Comparing `data_snack-0.2.0/src/data_snack/serializers/base.py` & `data_snack-0.2.1/src/data_snack/serializers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import List, Type, Union, Optional
+from typing import List, Optional, Type, Union
 
 from ..entities import Entity
 
 
 @dataclass
 class Serializer(ABC):
     entity_type: Type[Entity]
```

### Comparing `data_snack-0.2.0/src/data_snack/serializers/dataclass.py` & `data_snack-0.2.1/src/data_snack/serializers/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 import zlib
 from dataclasses import dataclass
-from typing import List, Union, get_type_hints, Optional
+from typing import List, Optional, Union, get_type_hints
 
 import pandas as pd
 
 from data_snack.entities import Entity
 from data_snack.serializers.base import Serializer
```

### Comparing `data_snack-0.2.0/src/data_snack/snack.py` & `data_snack-0.2.1/src/data_snack/snack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Text, Type, Any
+from typing import Any, Dict, List, Optional, Text, Type
 
 from .connections import Connection
 from .entities import Entity, EntityRegistry
-from .exceptions import EntityAlreadyRegistered, WrongKeyValue
-from .key_factory import KeyFactory, key_factory
+from .exceptions import EntityAlreadyRegistered
+from .key_factories import KeyFactory
+from .key_factories.non_cluster import NonClusterKeyFactory
 from .serializers import DataclassSerializer, Serializer
 from .wrap import EntityWrap
 
 
 @dataclass
 class Snack:
     """
     A core interface handling saving and reading Entities from db.
     """
 
     connection: Connection
     registry: Dict[Text, EntityRegistry] = field(default_factory=dict)
-    key_factory: KeyFactory = field(default=key_factory)
+    key_factory: KeyFactory = field(default=NonClusterKeyFactory())
 
     def register_entity(
         self,
         entity_type: Type[Entity],
         serializer: Serializer = None,
     ) -> None:
         """
@@ -58,15 +59,15 @@
         return self.registry[type_name].serializer
 
     def _build_record_key(self, type_name: Text, entity: Entity) -> Text:
         key_values = [
             getattr(entity, key)
             for key in self.registry[type_name].entity_type.get_keys()
         ]
-        return self.key_factory(type_name, *key_values)
+        return self.key_factory.get_key(type_name, *key_values)
 
     def set(self, entity: Entity, expire: int = 0) -> Optional[Text]:
         """
         Sets provided `Entity` object in db.
         Notice the entity stored in the db will be overwritten,
         so make sure all the combined keys are unique for each entity.
 
@@ -86,43 +87,46 @@
         Notice, key is represented as a list of strings, since one Entity can have multiple key fields.
 
         :param cls: `Entity` type
         :param key_values: a list of key values representing the entity
         :return: a retrieved Entity object
         """
         type_name = cls.__name__
-        _key = self.key_factory(type_name, *key_values)
+        _key = self.key_factory.get_key(type_name, *key_values)
         value = self.connection.get(_key)
         return self._get_serializer(type_name).deserialize(value)
 
     def delete(self, cls: Type[Entity], key_values: List[Any]) -> bool:
         """
         Deletes one entity of `Entity` type from db based on provided key values.
         Notice, key is represented as a list of strings, since one Entity can have multiple key fields.
 
         :param cls: `Entity` type
         :param key_values: a list of key values representing the entity
         :return: True if data were deleted
         """
         type_name = cls.__name__
-        _key = self.key_factory(type_name, *key_values)
+        _key = self.key_factory.get_key(type_name, *key_values)
         return self.connection.delete(_key)
 
     def get_many(
         self, cls: Type[Entity], keys_values: List[List[Any]]
     ) -> List[Optional[Entity]]:
         """
         Gets list of `Entity` objects from db based on provided list of keys.
 
         :param cls: `Entity` type
         :param keys_values: list of keys, each list defines a set key values for one Entity object
         :return: a list of retrieved Entity objects
         """
         type_name = cls.__name__
-        _keys = [self.key_factory(type_name, *key_values) for key_values in keys_values]
+        _keys = [
+            self.key_factory.get_key(type_name, *key_values)
+            for key_values in keys_values
+        ]
         records = list(self.connection.get_many(_keys).values())
         return self._get_serializer(type_name).deserialize(records, many=True)
 
     def set_many(self, entities: List[Entity]) -> List[Text]:
         """
         Saves multiple `Entity` objects in db.
 
@@ -140,18 +144,21 @@
         Deletes multiple `Entity` objects in db.
 
         :param cls: `Entity` type
         :param keys_values: list of keys, each list defines a set key values for one Entity object
         :return: True if data were deleted
         """
         type_name = cls.__name__
-        _keys = [self.key_factory(type_name, *key_values) for key_values in keys_values]
+        _keys = [
+            self.key_factory.get_key(type_name, *key_values)
+            for key_values in keys_values
+        ]
         return self.connection.delete_many(_keys)
 
     def keys(self, cls: Type[Entity]) -> List[Text]:
         """
         Gets a list of keys for a given Entity type.
 
         :param cls: Entity type
         :return: a list of keys
         """
-        return self.connection.keys(pattern=f"{cls.__name__}-*")
+        return self.connection.keys(pattern=self.key_factory.get_pattern(cls.__name__))
```

### Comparing `data_snack-0.2.0/src/data_snack/wrap/base.py` & `data_snack-0.2.1/src/data_snack/wrap/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.2.0/src/data_snack/wrap/data_frame.py` & `data_snack-0.2.1/src/data_snack/wrap/data_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 from typing import List, Text
 
 import pandas as pd
 
 from data_snack.wrap import EntityWrap
 from data_snack.wrap.exceptions import DataFrameMissingKeyColumn
 
@@ -34,8 +34,8 @@
         required_key_columns = self.entity_type.get_keys()
         if missing_columns := set(required_key_columns) - set(df.columns):
             raise DataFrameMissingKeyColumn(
                 f"Provided data frame is missing columns: {missing_columns}"
             )
 
         data = self.get_many(df[required_key_columns].values.tolist())
-        return pd.DataFrame(data)
+        return pd.DataFrame([asdict(row) if row else {} for row in data])
```

### Comparing `data_snack-0.2.0/src/data_snack/wrap/entity.py` & `data_snack-0.2.1/src/data_snack/wrap/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import List, Optional, Text, Type, Any
+from typing import Any, List, Optional, Text, Type
 
 from data_snack.entities import Entity
 
 from .base import Wrap
 
 
 @dataclass
```

### Comparing `data_snack-0.2.0/src/data_snack.egg-info/PKG-INFO` & `data_snack-0.2.1/src/data_snack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-snack
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-0.2.0/src/data_snack.egg-info/SOURCES.txt` & `data_snack-0.2.1/src/data_snack.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/data_snack/__init__.py
 src/data_snack/exceptions.py
-src/data_snack/key_factory.py
 src/data_snack/snack.py
 src/data_snack.egg-info/PKG-INFO
 src/data_snack.egg-info/SOURCES.txt
 src/data_snack.egg-info/dependency_links.txt
 src/data_snack.egg-info/requires.txt
 src/data_snack.egg-info/top_level.txt
 src/data_snack/connections/__init__.py
@@ -20,14 +19,18 @@
 src/data_snack/connections/redis.py
 src/data_snack/entities/__init__.py
 src/data_snack/entities/entity.py
 src/data_snack/entities/entity_meta.py
 src/data_snack/entities/exceptions.py
 src/data_snack/entities/registry.py
 src/data_snack/entities/schema.py
+src/data_snack/key_factories/__init__.py
+src/data_snack/key_factories/base.py
+src/data_snack/key_factories/cluster.py
+src/data_snack/key_factories/non_cluster.py
 src/data_snack/serializers/__init__.py
 src/data_snack/serializers/base.py
 src/data_snack/serializers/dataclass.py
 src/data_snack/wrap/__init__.py
 src/data_snack/wrap/base.py
 src/data_snack/wrap/data_frame.py
 src/data_snack/wrap/entity.py
```

