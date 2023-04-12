# Comparing `tmp/SISO-3.1.0.tar.gz` & `tmp/siso-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SISO-3.1.0.tar", last modified: Mon Jun 13 13:09:12 2022, max compression
+gzip compressed data, was "siso-4.1.0.tar", max compression
```

## Comparing `SISO-3.1.0.tar` & `siso-4.1.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:09:12.000000 SISO-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7504 2022-06-13 13:09:12.000000 SISO-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5622 2022-06-13 13:09:07.000000 SISO-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7504 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-13 13:09:12.000000 SISO-3.1.0/SISO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-13 13:09:12.000000 SISO-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-06-13 13:09:07.000000 SISO-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:09:12.000000 SISO-3.1.0/siso/
--rw-r--r--   0 runner    (1001) docker     (121)     8668 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8405 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:09:12.000000 SISO-3.1.0/siso/coords/
--rw-r--r--   0 runner    (1001) docker     (121)    10391 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6794 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/coords/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    10158 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    15744 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:09:12.000000 SISO-3.1.0/siso/reader/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16283 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/ifem.py
--rw-r--r--   0 runner    (1001) docker     (121)    12798 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/opera.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/puregeometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    21255 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/simra.py
--rw-r--r--   0 runner    (1001) docker     (121)    18706 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/reader/wrf.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     7150 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:09:12.000000 SISO-3.1.0/siso/writer/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9109 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/writer/nc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/writer/simra.py
--rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/writer/vtf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8624 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/writer/vtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-06-13 13:09:07.000000 SISO-3.1.0/siso/writer/writer.py
+-rw-r--r--   0        0        0    35489 2023-04-12 13:02:44.730068 siso-4.1.0/LICENSE
+-rw-r--r--   0        0        0     5622 2023-04-12 13:02:44.730068 siso-4.1.0/README.rst
+-rw-r--r--   0        0        0     1764 2023-04-12 13:02:44.730068 siso-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:44.730068 siso-4.1.0/siso/__init__.py
+-rw-r--r--   0        0        0    25609 2023-04-12 13:02:44.730068 siso-4.1.0/siso/__main__.py
+-rw-r--r--   0        0        0    29003 2023-04-12 13:02:44.730068 siso-4.1.0/siso/api.py
+-rw-r--r--   0        0        0    10120 2023-04-12 13:02:44.730068 siso-4.1.0/siso/coord.py
+-rw-r--r--   0        0        0      760 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/basis_filter.py
+-rw-r--r--   0        0        0     2881 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/basismerge.py
+-rw-r--r--   0        0        0     1910 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/coordtransform.py
+-rw-r--r--   0        0        0     5177 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/decompose.py
+-rw-r--r--   0        0        0     1857 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/discretize.py
+-rw-r--r--   0        0        0     1777 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/eigendisp.py
+-rw-r--r--   0        0        0      631 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/field_filter.py
+-rw-r--r--   0        0        0      914 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/force_unstructured.py
+-rw-r--r--   0        0        0     5213 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/keyzones.py
+-rw-r--r--   0        0        0     8489 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/passthrough.py
+-rw-r--r--   0        0        0     3506 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/recombine.py
+-rw-r--r--   0        0        0     4337 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/strict.py
+-rw-r--r--   0        0        0     4645 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/timeslice.py
+-rw-r--r--   0        0        0     2051 2023-04-12 13:02:44.730068 siso-4.1.0/siso/filter/zonemerge.py
+-rw-r--r--   0        0        0      433 2023-04-12 13:02:44.730068 siso-4.1.0/siso/impl.py
+-rw-r--r--   0        0        0     2495 2023-04-12 13:02:44.730068 siso-4.1.0/siso/instrument.py
+-rw-r--r--   0        0        0     3025 2023-04-12 13:02:44.730068 siso-4.1.0/siso/multisource.py
+-rw-r--r--   0        0        0     4744 2023-04-12 13:02:44.730068 siso-4.1.0/siso/reader/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-12 13:02:44.734068 siso-4.1.0/siso/reader/gotools.py
+-rw-r--r--   0        0        0    23419 2023-04-12 13:02:44.734068 siso-4.1.0/siso/reader/ifem.py
+-rw-r--r--   0        0        0     1057 2023-04-12 13:02:44.734068 siso-4.1.0/siso/reader/lrspline.py
+-rw-r--r--   0        0        0     2035 2023-04-12 13:02:44.734068 siso-4.1.0/siso/reader/puregeometry.py
+-rw-r--r--   0        0        0    36680 2023-04-12 13:02:44.734068 siso-4.1.0/siso/reader/simra.py
+-rw-r--r--   0        0        0    16711 2023-04-12 13:02:44.734068 siso-4.1.0/siso/reader/wrf.py
+-rw-r--r--   0        0        0    27146 2023-04-12 13:02:44.734068 siso-4.1.0/siso/topology.py
+-rw-r--r--   0        0        0    14910 2023-04-12 13:02:44.734068 siso-4.1.0/siso/util/__init__.py
+-rw-r--r--   0        0        0     3016 2023-04-12 13:02:44.734068 siso-4.1.0/siso/util/bisect.py
+-rw-r--r--   0        0        0     2621 2023-04-12 13:02:44.734068 siso-4.1.0/siso/util/cell_numbering.py
+-rw-r--r--   0        0        0     5965 2023-04-12 13:02:44.734068 siso-4.1.0/siso/util/coord.py
+-rw-r--r--   0        0        0    15684 2023-04-12 13:02:44.734068 siso-4.1.0/siso/util/field_data.py
+-rw-r--r--   0        0        0     1745 2023-04-12 13:02:44.734068 siso-4.1.0/siso/writer/__init__.py
+-rw-r--r--   0        0        0      927 2023-04-12 13:02:44.734068 siso-4.1.0/siso/writer/api.py
+-rw-r--r--   0        0        0     3219 2023-04-12 13:02:44.734068 siso-4.1.0/siso/writer/simra.py
+-rw-r--r--   0        0        0     5803 2023-04-12 13:02:44.734068 siso-4.1.0/siso/writer/vtf.py
+-rw-r--r--   0        0        0     8849 2023-04-12 13:02:44.734068 siso-4.1.0/siso/writer/vtk.py
+-rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 siso-4.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SISO-3.1.0/README.rst` & `siso-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `SISO-3.1.0/siso/coords/__init__.py` & `siso-4.1.0/siso/coord.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,355 +1,361 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from inspect import isabstract
+from collections import deque
+from typing import Callable, ClassVar, Dict, List, Optional, Sequence, Tuple, Type, TypeVar, cast
 
 import erfa
 import numpy as np
+from attrs import define
+from numpy import floating
+from typing_extensions import Self
 
-from typing import Union, Dict, List, Tuple, Callable, Set, Iterable, Optional
-from ..typing import Array2D
-
-from ..geometry import PatchKey
-from ..util import subclasses
-from .. import config
-
-from .util import spherical_cartesian_vf, utm_to_lonlat, utm_to_lonlat_vf, lonlat_to_utm, lonlat_to_utm_vf
+from . import api, util
+from .util import FieldData, coord
 
 
+systems: util.Registry[Type[api.CoordinateSystem]] = util.Registry()
+ellpsoids: util.Registry[Type[Ellipsoid]] = util.Registry()
 
-# Errors
-# ----------------------------------------------------------------------
 
+def find_system(code: str) -> api.CoordinateSystem:
+    name, *params = code.split(":")
+    if name in systems:
+        return systems[name].make(params)
+    return Named.make((code,))
 
-class CoordinateConversionError(TypeError):
-    pass
 
+@systems.register
+@define
+class Generic(api.CoordinateSystem):
+    name: ClassVar[str] = "Generic"
 
+    @classmethod
+    def make(cls, params: Sequence[str]) -> Generic:
+        if params:
+            raise api.BadInput("Generic coordinate system does not accept parameters")
+        return cls()
 
-# Reference ellipsoids
-# ----------------------------------------------------------------------
+    @classmethod
+    def default(cls) -> Generic:
+        return cls()
 
+    @property
+    def parameters(self) -> Tuple[str, ...]:
+        return cast(Tuple[str], ())
 
-class Ellipsoid(ABC):
 
-    name: str
+@systems.register
+@define
+class Named(api.CoordinateSystem):
+    name: ClassVar[str] = "Named"
+    identifier: str
 
-    @staticmethod
-    def find(name: str):
-        for cls in subclasses(Ellipsoid, root=False):
-            if hasattr(cls, 'name') and cls.name.lower() == name.lower():
-                return cls()
-        raise ValueError(f"Unknown reference ellipsoid: {name.lower()}")
+    @classmethod
+    def make(cls, params: Sequence[str]) -> Named:
+        if len(params) != 1:
+            raise api.BadInput("Named coordinate system requires one parameter")
+        (name,) = params
+        return cls(name)
 
-    def __str__(self):
-        return self.name
+    @classmethod
+    def default(cls) -> Named:
+        raise api.Unsupported("There is no default named coordinate system")
 
     @property
-    @abstractmethod
-    def parameters(self) -> Tuple[float, float]:
-        """Get the semi-major axis and flattening."""
-
-
-class SphericalEllipsoid(Ellipsoid):
+    def parameters(self) -> Tuple[str, ...]:
+        if self.identifier:
+            return (self.identifier,)
+        return cast(Tuple[str], ())
+
+    def fits_system_name(self, code: str) -> bool:
+        return code.casefold() == self.identifier.casefold()
 
-    name = 'sphere'
-
-    @property
-    def parameters(self) -> Tuple[float, float]:
-        mean_radius = 6_371_008.8
-        return mean_radius, 0.0
 
+@systems.register
+@define
+class Geodetic(api.CoordinateSystem):
+    name: ClassVar[str] = "Geodetic"
+    ellipsoid: Ellipsoid
 
-class ERFAEllipsoid(Ellipsoid):
+    @classmethod
+    def make(cls, params: Sequence[str]) -> Geodetic:
+        if len(params) >= 2:
+            raise api.BadInput("Geodetic coordinate system only accepts one optional parameter")
+        if params:
+            return cls(ellpsoids[params[0]]())
+        return cls(Wgs84())
 
-    erfa_code: int
+    @classmethod
+    def default(cls) -> Geodetic:
+        return cls(Wgs84())
 
     @property
-    def parameters(self) -> Tuple[float, float]:
-        return erfa.eform(self.erfa_code)
-
-
-class WGS84(ERFAEllipsoid):
-
-    name = 'WGS84'
-    erfa_code = 1
+    def parameters(self) -> Tuple[str, ...]:
+        return (self.ellipsoid.name,)
 
+    @property
+    def semi_major_axis(self) -> float:
+        return self.ellipsoid.semi_major_axis
 
-class GRS80(ERFAEllipsoid):
+    @property
+    def flattening(self) -> float:
+        return self.ellipsoid.flattening
 
-    name = 'GRS80'
-    erfa_code = 2
 
+@systems.register
+@define
+class Utm(api.CoordinateSystem):
+    name: ClassVar[str] = "UTM"
+    zone_number: int
+    northern: bool
 
-class WGS72(ERFAEllipsoid):
+    @classmethod
+    def make(cls, params: Sequence[str]) -> Utm:
+        (zone,) = params
+        try:
+            i = next(i for i in range(len(zone)) if not zone[i].isnumeric())
+        except StopIteration:
+            raise ValueError(zone)
+        zone_number = int(zone[:i])
+        lat_band = zone[i:]
+        if len(lat_band) == 1:
+            northern = lat_band.casefold() >= "N"
+        else:
+            northern = not lat_band[0].casefold() == "S"
+        return cls(zone_number, northern)
 
-    name = 'WGS72'
-    erfa_code = 3
+    @classmethod
+    def default(cls) -> Utm:
+        raise api.Unsupported("There is no default UTM coordinate system")
 
+    @property
+    def parameters(self) -> Tuple[str, ...]:
+        return (str(self.zone_number), "north" if self.northern else "south")
 
 
-# Coordinate systems
-# ----------------------------------------------------------------------
+@systems.register
+class Geocentric(api.CoordinateSystem):
+    name = "Geocentric"
+    parameters = cast(Tuple[str], ())
 
+    @classmethod
+    def make(cls, params: Sequence[str]) -> Self:
+        if params:
+            raise api.BadInput("Geocentric coordinate system does not accept parameters")
+        return cls()
 
-class Coords(ABC):
+    @classmethod
+    def default(cls) -> Geocentric:
+        return cls()
 
-    name: str
 
-    @staticmethod
-    def find(name: str) -> 'Coords':
-        root, *args = name.lower().split(':')
-        for cls in subclasses(Coords, root=False, invert=True):
-            if cls.name == root:
-                return cls(*args)
-        return Local(name)
+class Ellipsoid(ABC):
+    name: ClassVar[str]
 
-    def __str__(self):
-        return self.name
+    @property
+    @abstractmethod
+    def semi_major_axis(self) -> float:
+        ...
 
-    def __eq__(self, other):
-        if not isinstance(other, Coords):
-            return False
-        return str(self) == str(other)
+    @property
+    @abstractmethod
+    def flattening(self) -> float:
+        ...
 
-    def substitute(self):
-        return self
 
+@ellpsoids.register
+@define
+class SphericalEarth(Ellipsoid):
+    name = "Sphere"
+    flattening: float = 0.0
+    semi_major_axis: float = 6_371_008.8
 
-class Local(Coords):
-    """This class represents an unspecified coordinate system to and
-    from which conversion is impossible.  There may be several such,
-    which are distinguished by name.
-    """
 
-    name = 'local'
+class ErfaEllipsoid(Ellipsoid):
+    erfa_code: ClassVar[int]
 
-    specific_name: str
+    @property
+    def semi_major_axis(self) -> float:
+        return erfa.eform(self.erfa_code)[0]
 
-    def __init__(self, name='local'):
-        self.specific_name = name
+    @property
+    def flattening(self) -> float:
+        return erfa.eform(self.erfa_code)[1]
 
-    def __str__(self):
-        return f'Local({self.specific_name})'
 
-    def substitute(self):
-        return config.input_coords.get(self.specific_name, self)
+@ellpsoids.register
+@define
+class Wgs84(ErfaEllipsoid):
+    erfa_code = 1
+    name = "WGS84"
 
 
-class Geodetic(Coords):
-    """Latitude, longitude and height above the reference ellipsoid."""
+@ellpsoids.register
+@define
+class Grs80(ErfaEllipsoid):
+    erfa_code = 2
+    name = "GRS80"
 
-    name = 'geodetic'
 
+@ellpsoids.register
+@define
+class Wgs72(ErfaEllipsoid):
+    erfa_code = 3
+    name = "WGS72"
 
-class UTM(Coords):
-    """Universal Transversal Mercator"""
 
-    zone_number: int
-    zone_letter: str
+T = TypeVar("T", bound=api.CoordinateSystem)
+S = TypeVar("S", bound=api.CoordinateSystem)
 
-    name = 'utm'
 
-    def __init__(self, zone: str):
-        self.zone_number = int(zone[:-1])
-        self.zone_letter = zone[-1].upper()
+CoordConverter = Callable[[T, S, FieldData[floating]], FieldData[floating]]
+VectorConverter = Callable[[T, S, FieldData[floating], FieldData[floating]], FieldData[floating]]
+ConversionPath = List[api.CoordinateSystem]
 
-    def __str__(self):
-        return f'{self.name}:{self.zone_number}{self.zone_letter}'
 
-    @classmethod
-    def optimal(cls, lon: float, lat: float):
-        zone = None
-        if 56 <= lat < 64 and 3 <= lon < 12:
-            zone = 32
-        elif 72 <= lat <= 84 and lon >= 0:
-            if lon < 9:
-                zone = 31
-            elif lon < 21:
-                zone = 33
-            elif lon < 33:
-                zone = 35
-            elif lon < 42:
-                zone = 37
-        if zone is None:
-            zone = int((lon + 180) / 6) + 1
-
-        letter = 'CDEFGHJKLMNPQRSTUVWXX'[int(lat + 80) >> 3]
-        return cls(f'{zone}{letter}')
-
-
-class Geocentric(Coords):
-    """Geocentric coordinates with origin in the center of the Earth,
-    positive z pointing toward the north pole, the xy-plane aligned
-    with the equator, and positive x pointing in the direction of the
-    prime meridian.
-    """
+NEIGHBORS: Dict[str, List[str]] = {}
+COORD_CONVERTERS: Dict[Tuple[str, str], CoordConverter] = {}
+VECTOR_CONVERTERS: Dict[Tuple[str, str], VectorConverter] = {}
 
-    ellipsoid: Ellipsoid
 
-    name = 'geocentric'
+def register_coords(
+    src: Type[api.CoordinateSystem], tgt: Type[api.CoordinateSystem]
+) -> Callable[[CoordConverter[T, S]], CoordConverter[T, S]]:
+    def decorator(conv: CoordConverter) -> CoordConverter:
+        NEIGHBORS.setdefault(src.name, []).append(tgt.name)
+        COORD_CONVERTERS[(src.name, tgt.name)] = conv
+        return conv
 
-    def __init__(self, ellipsoid: Union[Ellipsoid, str] = WGS84()):
-        if isinstance(ellipsoid, str):
-            ellipsoid = Ellipsoid.find(ellipsoid)
-        self.ellipsoid = ellipsoid
-
-    def __str__(self):
-        return f'{self.name}:{self.ellipsoid}'
-
-
-
-# Coordinate conversion
-# ----------------------------------------------------------------------
-
-
-ConvDict = Dict[Tuple[str, str], Callable]
-
-class ConversionGraph:
-
-    # Keeps track of neighboring coordinate systems: those that can be
-    # directly reached by one converter
-    neighbors: Dict[str, List[str]]
-
-    # Keeps track of the actual point converter functions
-    point_converters: ConvDict
-
-    # Keeps track of the actual vector field converter functions
-    vector_converters: ConvDict
-
-    def __init__(self):
-        self.neighbors = dict()
-        self.point_converters = dict()
-        self.vector_converters = dict()
-
-    def points(self, source: str, target: str) -> Callable:
-        def decorator(func: Callable) -> Callable:
-            self.neighbors.setdefault(source, []).append(target)
-            self.point_converters[(source, target)] = func
-            return func
-        return decorator
-
-    def vectors(self, source: str, target: str, trivial: bool = True) -> Callable:
-        def decorator(func: Callable) -> Callable:
-            self.neighbors.setdefault(source, []).append(target)
-            self.vector_converters[(source, target)] = func
-            func.is_trivial = trivial
-            return func
-        return decorator
-
-    def path(self, source: Coords, target: Coords) -> 'Converter':
-        if source == target:
-            return Converter(self, [])
-
-        # Special case: conversion from Local(anything) to
-        # Local('local') is always allowed and is a no-op
-        if isinstance(source, Local) and target == Local('local'):
-            return Converter(self, [])
-
-        seen: Set[str] = set()
-        front: Dict[str, List[str]] = {source.name: [source.name]}
-
-        while front:
-            new_front = dict()
-            for front_point, path in front.items():
-                for neighbor in self.neighbors.get(front_point, []):
-                    if neighbor in seen:
-                        continue
-                    seen.add(neighbor)
-                    new_path = [*path, neighbor]
-                    if neighbor == target.name:
-                        return Converter(self, new_path)
-                    new_front[neighbor] = new_path
-            front = new_front
-
-        raise CoordinateConversionError(f"Unable to convert {source} to {target}")
-
-    def optimal_source(self, target: Coords, sources: Iterable[Coords]) -> Tuple[int, 'Converter']:
-        min_distance, retval = None, None
-        for i, source in enumerate(sources):
-            try:
-                converter = self.path(source, target)
-            except ValueError:
-                continue
-            if min_distance is None or len(converter) < min_distance:
-                min_distance = len(converter)
-                retval = (i, converter)
+    return decorator
 
-        if retval is None:
-            raise ValueError(f"Unable to find a conversion path to {target}")
-        return retval
 
-graph = ConversionGraph()
+def register_vectors(
+    src: Type[api.CoordinateSystem], tgt: Type[api.CoordinateSystem]
+) -> Callable[[VectorConverter[T, S]], VectorConverter[T, S]]:
+    def decorator(conv: VectorConverter) -> VectorConverter:
+        VECTOR_CONVERTERS[(src.name, tgt.name)] = conv
+        return conv
 
+    return decorator
 
-class Converter:
 
-    graph: ConversionGraph
-    path: List[str]
-    nodes: Dict[Tuple[Tuple[str, str], PatchKey], Array2D]
+def conversion_path(src: api.CoordinateSystem, tgt: api.CoordinateSystem) -> Optional[ConversionPath]:
+    if src == tgt:
+        return []
+    if isinstance(src, (Generic, Named)) and isinstance(tgt, Generic):
+        return []
 
-    def __init__(self, graph: ConversionGraph, path: List[str]):
-        self.graph = graph
-        self.path = path
-        self.nodes = dict()
+    visited: Dict[str, str] = {}
+    queue: deque[str] = deque((src.name,))
 
-    def __len__(self):
-        return len(self.path)
+    def construct_backpath() -> ConversionPath:
+        path = [tgt]
+        name = visited[tgt.name]
+        while name != src.name:
+            path.append(systems[name].default())
+            name = visited[name]
+        path.append(src)
+        return path[::-1]
 
-    @property
-    def is_trivial(self):
-        return all(
-            self.graph.vector_converters[(a, b)].is_trivial
-            for a, b in zip(self.path[:-1], self.path[1:])
+    while queue:
+        system = queue.popleft()
+        for neighbor in NEIGHBORS.get(system, []):
+            if neighbor in visited or neighbor == src.name:
+                continue
+            visited[neighbor] = system
+            if neighbor == tgt.name:
+                return construct_backpath()
+            queue.append(neighbor)
+
+    return None
+
+
+def optimal_system(
+    systems: Sequence[api.CoordinateSystem], target: api.CoordinateSystem
+) -> Optional[Tuple[int, ConversionPath]]:
+    optimal: Optional[Tuple[int, ConversionPath]] = None
+
+    for i, system in enumerate(systems):
+        new_path = conversion_path(system, target)
+        if new_path is None:
+            continue
+        if optimal is None:
+            optimal = i, new_path
+        _, prev_path = optimal
+        if len(new_path) < len(prev_path):
+            optimal = i, new_path
+
+    return optimal
+
+
+def convert_coords(
+    src: api.CoordinateSystem,
+    tgt: api.CoordinateSystem,
+    data: FieldData[floating],
+) -> FieldData[floating]:
+    return COORD_CONVERTERS[(src.name, tgt.name)](src, tgt, data)
+
+
+def convert_vectors(
+    src: api.CoordinateSystem,
+    tgt: api.CoordinateSystem,
+    data: FieldData[floating],
+    coords: FieldData[floating],
+) -> FieldData[floating]:
+    return VECTOR_CONVERTERS[(src.name, tgt.name)](src, tgt, data, coords)
+
+
+@register_coords(Geodetic, Geocentric)
+def _(src: Geodetic, tgt: Geocentric, data: FieldData[floating]) -> FieldData[floating]:
+    lon, lat, height = data.comps
+    return FieldData(
+        erfa.gd2gce(
+            src.ellipsoid.semi_major_axis,
+            src.ellipsoid.flattening,
+            np.deg2rad(lon),
+            np.deg2rad(lat),
+            height,
         )
+    )
+
 
-    def convert(self, src: Coords, tgt: Coords, data: Array2D, lookup: ConvDict, key: PatchKey, store: bool) -> Array2D:
-        if not self.path:
-            return data
-        path = [src] + [Coords.find(c) for c in self.path[1:-1]] + [tgt]
-        for a, b in zip(path[:-1], path[1:]):
-            edge = (a.name, b.name)
-            if store:
-                self.nodes[edge, key] = data
-                data = lookup[edge](a, b, data)
-            else:
-                data = lookup[edge](a, b, data, nodes=self.nodes[edge, key])
-        return data
-
-    def points(self, src: Coords, tgt: Coords, data: Array2D, key: PatchKey) -> Array2D:
-        return self.convert(src, tgt, data, self.graph.point_converters, key=key, store=True)
-
-    def vectors(self, src: Coords, tgt: Coords, data: Array2D, key: PatchKey) -> Array2D:
-        return self.convert(src, tgt, data, self.graph.vector_converters, key=key, store=False)
-
-
-@graph.points('geodetic', 'geocentric')
-def _(src: Geodetic, tgt: Geocentric, data: Array2D) -> Array2D:
-    lon, lat, h = data.T
-    lon = np.deg2rad(lon)
-    lat = np.deg2rad(lat)
-    a, f = tgt.ellipsoid.parameters
-    return erfa.gd2gce(a, f, lon, lat, h)
-
-@graph.vectors('geodetic', 'geocentric', trivial=False)
-def _(src: Geodetic, tgt: Geocentric, data: Array2D, nodes: Array2D) -> Array2D:
-    lon, lat = nodes[:,0], nodes[:,1]
-    return spherical_cartesian_vf(lon, lat, data)
-
-@graph.points('utm', 'geodetic')
-def _(src: UTM, tgt: Geodetic, data: Array2D) -> Array2D:
-    lon, lat = utm_to_lonlat(data[:,0], data[:,1], src.zone_number, src.zone_letter)
-    return np.hstack([lon.reshape(-1,1), lat.reshape(-1,1), data[:,2:]])
-
-@graph.vectors('utm', 'geodetic', trivial=False)
-def _(src: UTM, tgt: Geodetic, data: Array2D, nodes: Array2D) -> Array2D:
-    vx, vy = utm_to_lonlat_vf(nodes[:,0], nodes[:,1], data[:,0], data[:,1], src.zone_number, src.zone_letter)
-    return np.hstack([vx.reshape(-1,1), vy.reshape(-1,1), data[:,2:]])
-
-@graph.points('geodetic', 'utm')
-def _(src: Geodetic, tgt: UTM, data: Array2D) -> Array2D:
-    x, y = lonlat_to_utm(data[:,0], data[:,1], tgt.zone_number, tgt.zone_letter)
-    return np.hstack([x.reshape(-1,1), y.reshape(-1,1), data[:,2:]])
-
-@graph.vectors('geodetic', 'utm')
-def _(src: Geodetic, tgt: UTM, data: Array2D, nodes: Array2D) -> Array2D:
-    x, y = lonlat_to_utm_vf(nodes[:,0], nodes[:,1], data[:,0], data[:,1], tgt.zone_number, tgt.zone_letter)
-    return np.hstack([x.reshape(-1,1), y.reshape(-1,1), data[:,2:]])
+@register_vectors(Geodetic, Geocentric)
+def _(
+    src: Geodetic, tgt: Geocentric, data: FieldData[floating], coords: FieldData[floating]
+) -> FieldData[floating]:
+    return data.spherical_to_cartesian_vector_field(coords)
+
+
+@register_coords(Geodetic, Utm)
+def _(src: Geodetic, tgt: Utm, data: FieldData[floating]) -> FieldData[floating]:
+    lon, lat, *rest = data.comps
+    converter = coord.UtmConverter(src.semi_major_axis, src.flattening, tgt.zone_number, tgt.northern)
+    x, y = converter.to_utm(lon, lat)
+    return FieldData.join_comps(x, y, *rest)
+
+
+@register_vectors(Geodetic, Utm)
+def _(src: Geodetic, tgt: Utm, data: FieldData[floating], coords: FieldData[floating]) -> FieldData[floating]:
+    lon, lat, *_ = coords.comps
+    in_x, in_y, *rest = data.comps
+    converter = coord.UtmConverter(src.semi_major_axis, src.flattening, tgt.zone_number, tgt.northern)
+    out_x, out_y = converter.to_utm_vf(lon, lat, in_x, in_y)
+    return FieldData.join_comps(out_x, out_y, *rest)
+
+
+@register_coords(Utm, Geodetic)
+def _(src: Utm, tgt: Geodetic, data: FieldData[floating]) -> FieldData[floating]:
+    x, y, *rest = data.comps
+    converter = coord.UtmConverter(tgt.semi_major_axis, tgt.flattening, src.zone_number, src.northern)
+    lon, lat = converter.to_lonlat(x, y)
+    return FieldData.join_comps(lon, lat, *rest)
+
+
+@register_vectors(Utm, Geodetic)
+def _(src: Utm, tgt: Geodetic, data: FieldData[floating], coords: FieldData[floating]) -> FieldData[floating]:
+    x, y, *_ = coords.comps
+    in_x, in_y, *rest = data.comps
+    converter = coord.UtmConverter(tgt.semi_major_axis, tgt.flattening, src.zone_number, src.northern)
+    out_x, out_y = converter.to_lonlat_vf(x, y, in_x, in_y)
+    return FieldData.join_comps(out_x, out_y, *rest)
```

### Comparing `SISO-3.1.0/siso/writer/vtf.py` & `siso-4.1.0/siso/writer/vtf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,144 @@
-"""Module for VTF format writer."""
+from __future__ import annotations
 
-from contextlib import contextmanager
+import logging
 from pathlib import Path
+from typing import Dict, List, Tuple, Type
 
-from typing import List, Dict, Any, Tuple, Type, Optional
+import vtfwriter as vtf
+from attrs import define
+from typing_extensions import Self
 
-from dataclasses import dataclass
-import treelog as log
+from .. import api
+from ..api import B, CellOrdering, DiscreteTopology, F, S, Step, StepInterpretation, T, Z, Zone
+from .api import OutputMode, Writer, WriterProperties, WriterSettings
 
-from .. import config
-from ..fields import SimpleField
-from ..geometry import Patch
-from ..util import ensure_ncomps
-from .writer import Writer
 
-from ..typing import Array2D, StepData
+@define
+class FieldInfo:
+    blocktype: Type[vtf.Block]
+    steps: Dict[int, List[vtf.ResultBlock]]
 
-try:
-    import vtfwriter as vtf
-    HAS_VTF = True
-except ImportError:
-    HAS_VTF = False
 
+class VtfWriter(Writer):
+    filename: Path
+    out: vtf.File
+    mode: OutputMode
 
-
-@dataclass
-class Field:
-    """Utility class for block book-keeping."""
-    blocktype: Type['vtf.Block']
-    steps: Dict[int, List['vtf.ResultBlock']]
-
-
-class VTFWriter(Writer):
-    """Writer for VTF format."""
-
-    writer_name = "VTF"
-
-    out: 'vtf.File'             # vtf is optional
-    dirty_geometry: bool
-
-    steps: List[Dict[str, Any]]
-    geometry_blocks: List[Tuple['vtf.NodeBlock', 'vtf.ElementBlock']]
-    field_blocks: Dict[str, Field]
-
-    gblock: Optional['vtf.GeometryBlock']
-
-    @classmethod
-    def applicable(cls, fmt: str) -> bool:
-        return HAS_VTF and fmt == 'vtf'
+    geometry_block: vtf.GeometryBlock
+    geometry_blocks: List[Tuple[vtf.NodeBlock, vtf.ElementBlock]]
+    timesteps: List[Step]
+    field_info: Dict[str, FieldInfo]
+    step_interpretation: StepInterpretation
 
     def __init__(self, filename: Path):
-        super().__init__(filename)
-        self.steps = []
+        self.filename = filename
+        self.timesteps = []
         self.geometry_blocks = []
+        self.field_info = {}
+        self.step_interpretation = StepInterpretation.Time
 
-        self.field_blocks = dict()
-        self.dirty_geometry = False
-
-        self.gblock = None
-
-    def validate(self):
-        config.require_in(reason="not supported by VTF", output_mode=('binary', 'ascii'))
+    @property
+    def properties(self) -> WriterProperties:
+        return WriterProperties(
+            require_discrete_topology=True,
+            require_single_basis=True,
+        )
+
+    def configure(self, settings: WriterSettings):
+        if settings.output_mode is not None:
+            if settings.output_mode not in (OutputMode.Binary, OutputMode.Ascii):
+                raise api.Unsupported(f"Unsupported output mode for VTF: {settings.output_mode}")
+            self.mode = settings.output_mode
+        else:
+            self.mode = OutputMode.Binary
 
-    def __enter__(self) -> 'Writer':
-        super().__enter__()
-        self.out = vtf.File(str(self.make_filename()), 'w' if config.output_mode == 'ascii' else 'wb').__enter__()
-        self.gblock = self.out.GeometryBlock().__enter__()
+    def __enter__(self) -> Self:
+        self.out = vtf.File(
+            str(self.filename),
+            "w" if self.mode == OutputMode.Ascii else "wb",
+        ).__enter__()
+        self.geometry_block = self.out.GeometryBlock().__enter__()
         return self
 
-    def __exit__(self, *args, **kwargs):
-        for fname, data in self.field_blocks.items():
-            with data.blocktype() as fblock:
-                fblock.SetName(fname)
-                for stepid, rblocks in data.steps.items():
-                    fblock.BindResultBlocks(stepid, *rblocks)
-
-        self.gblock.__exit__(*args, **kwargs)
-        self.exit_stateinfo()
-        self.out.__exit__(*args, **kwargs)
-        super().__exit__(*args, **kwargs)
-        log.user(self.make_filename())
-
-    def exit_stateinfo(self):
-        """Create the state info block, as the last thing to happen before
-        closing the file.
-        """
-        with self.out.StateInfoBlock() as states:
-            for stepid, data in enumerate(self.steps):
-                key, value = next(iter(data.items()))
-                func = states.SetStepData if key == 'time' else states.SetModeData
-                desc = {'value': 'Eigenvalue', 'frequency': 'Frequency', 'time': 'Time'}[key]
-                func(stepid+1, '{} {:.4g}'.format(desc, value), value)
-
-    @contextmanager
-    def step(self, stepdata: StepData):
-        self.steps.append(stepdata)
-        with super().step(stepdata) as step:
-            yield step
-
-    @contextmanager
-    def geometry(self, field: Field):
-        with super().geometry(field) as geometry:
-            yield geometry
-            if self.dirty_geometry:
-                self.gblock.BindElementBlocks(*[e for _, e in self.geometry_blocks], step=self.stepid+1)
-            self.dirty_geometry = False
-
-    def update_geometry(self, geometry: Field, patch: Patch, data: Array2D):
-        data = ensure_ncomps(data, 3, allow_scalar=False)
-        patchid = patch.key[0]
-
-        # If we haven't seen this patch before, assert that it's the
-        # next unseen one
-        if len(self.geometry_blocks) <= patchid:
-            assert len(self.geometry_blocks) == patchid
-
-        with self.out.NodeBlock() as nblock:
-            nblock.SetNodes(data.flat)
-
-        with self.out.ElementBlock() as eblock:
-            eblock.AddElements(patch.topology.cells.flat, patch.topology.num_pardim)
-            eblock.SetPartName('Patch {}'.format(patchid+1))
-            eblock.BindNodeBlock(nblock, patchid+1)
+    def __exit__(self, *args) -> None:
+        for field_name, info in self.field_info.items():
+            with info.blocktype() as field_block:
+                field_block.SetName(field_name)
+                for index, result_blocks in info.steps.items():
+                    field_block.BindResultBlocks(index, *result_blocks)
+
+        self.geometry_block.__exit__(*args)
+
+        with self.out.StateInfoBlock() as state_info:
+            setter = state_info.SetStepData if self.step_interpretation.is_time else state_info.SetModeData
+            desc = str(self.step_interpretation)
+            for timestep in self.timesteps:
+                time = timestep.value if timestep.value is not None else float(timestep.index)
+                setter(timestep.index + 1, f"{desc} {time:.4g}", time)
+
+        self.out.__exit__(*args)
+        logging.info(self.filename)
+
+    def update_geometry(
+        self, timestep: S, source: api.Source[B, F, S, DiscreteTopology, Zone[int]], geometry: F
+    ) -> None:
+        for zone in source.zones():
+            topology = source.topology(timestep, source.basis_of(geometry), zone)
+            nodes = source.field_data(timestep, geometry, zone).ensure_ncomps(3)
+
+            with self.out.NodeBlock() as node_block:
+                node_block.SetNodes(nodes.numpy().flatten())
+
+            with self.out.ElementBlock() as element_block:
+                element_block.AddElements(
+                    topology.cells_as(CellOrdering.Vtk).numpy().flatten(), topology.pardim
+                )
+                element_block.SetPartName(f"Patch {zone.key + 1}")
+                element_block.BindNodeBlock(node_block, zone.key + 1)
 
-        if len(self.geometry_blocks) <= patchid:
-            self.geometry_blocks.append((nblock, eblock))
-        else:
-            self.geometry_blocks[patchid] = (nblock, eblock)
-        self.dirty_geometry = True
-
-    def update_field(self, field: SimpleField, patch: Patch, data: Array2D):
-        data = ensure_ncomps(data, 3, allow_scalar=field.is_scalar)
-        patchid = patch.key[0]
-
-        nblock, eblock = self.geometry_blocks[patchid]
-        with self.out.ResultBlock(cells=field.cells, vector=field.is_vector) as rblock:
-            rblock.SetResults(data.flatten())
-            rblock.BindBlock(eblock if field.cells else nblock)
-
-        if field.name not in self.field_blocks:
-            if field.is_scalar:
-                blocktype = self.out.ScalarBlock
-            elif not field.is_displacement:
-                blocktype = self.out.VectorBlock
+            if len(self.geometry_blocks) <= zone.key:
+                self.geometry_blocks.append((node_block, element_block))
             else:
-                blocktype = self.out.DisplacementBlock
-            self.field_blocks[field.name] = Field(blocktype, {})
+                self.geometry_blocks[zone.key] = (node_block, element_block)
+
+        self.geometry_block.BindElementBlocks(*(e for _, e in self.geometry_blocks), step=timestep.index + 1)
 
-        steps = self.field_blocks[field.name].steps
-        steps.setdefault(self.stepid + 1, []).append(rblock)
+    def update_field(
+        self, timestep: S, source: api.Source[B, F, S, DiscreteTopology, Zone[int]], field: F
+    ) -> None:
+        for zone in source.zones():
+            data = source.field_data(timestep, field, zone)
+            data = data.ensure_ncomps(3, allow_scalar=field.is_scalar, pad_right=not field.is_displacement)
+            node_block, element_block = self.geometry_blocks[zone.key]
+
+            with self.out.ResultBlock(cells=field.cellwise, vector=field.is_vector) as result_block:
+                result_block.SetResults(data.numpy().flatten())
+                result_block.BindBlock(element_block if field.cellwise else node_block)
+
+            if field.name not in self.field_info:
+                if field.is_scalar:
+                    blocktype = self.out.ScalarBlock
+                elif not field.is_displacement:
+                    blocktype = self.out.VectorBlock
+                else:
+                    blocktype = self.out.DisplacementBlock
+                self.field_info[field.name] = FieldInfo(blocktype, {})
+
+            steps = self.field_info[field.name].steps
+            steps.setdefault(timestep.index + 1, []).append(result_block)
+
+    def consume_timestep(
+        self, timestep: S, source: api.Source[B, F, S, DiscreteTopology, Zone[int]], geometry: F
+    ) -> None:
+        if source.field_updates(timestep, geometry):
+            self.update_geometry(timestep, source, geometry)
+        for field in source.fields(source.single_basis()):
+            if source.field_updates(timestep, field):
+                self.update_field(timestep, source, field)
+
+    def consume(self, source: api.Source[B, F, S, T, Z], geometry: F):
+        casted = source.cast_discrete_topology().cast_globally_keyed()
+        self.step_interpretation = source.properties.step_interpretation
+        for step in casted.steps():
+            self.timesteps.append(step)
+            self.consume_timestep(step, casted, geometry)
```

### Comparing `SISO-3.1.0/siso/writer/vtk.py` & `siso-4.1.0/siso/writer/vtk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,265 +1,253 @@
-"""Module for VTK format writers."""
+from __future__ import annotations
 
-from abc import abstractmethod, abstractclassmethod
-from contextlib import contextmanager
-from os import makedirs
+import logging
+from abc import ABC, abstractmethod
+from enum import Enum, auto
 from pathlib import Path
+from typing import IO, Tuple, TypeVar, Union
 
-from typing import TextIO, Optional
+from numpy import number
+from typing_extensions import Self
 
-import numpy as np
-import treelog as log
-
-# We import from vtkmodules to help linters find the module members
+from vtkmodules.util.numpy_support import numpy_to_vtkIdTypeArray
 from vtkmodules.vtkCommonCore import vtkPoints
 from vtkmodules.vtkCommonDataModel import (
-    vtkDataSet, vtkUnstructuredGrid, vtkStructuredGrid, vtkCellArray,
-    VTK_HEXAHEDRON, VTK_QUAD, VTK_LINE
+    VTK_HEXAHEDRON,
+    VTK_LINE,
+    VTK_QUAD,
+    vtkCellArray,
+    vtkPointSet,
+    vtkStructuredGrid,
+    vtkUnstructuredGrid,
 )
-from vtkmodules.vtkIOLegacy import vtkUnstructuredGridWriter, vtkStructuredGridWriter
-from vtkmodules.vtkIOXML import vtkXMLUnstructuredGridWriter, vtkXMLStructuredGridWriter
-from vtkmodules.util.numpy_support import numpy_to_vtk, numpy_to_vtkIdTypeArray
+from vtkmodules.vtkIOLegacy import vtkDataWriter, vtkStructuredGridWriter, vtkUnstructuredGridWriter
+from vtkmodules.vtkIOXML import vtkXMLStructuredGridWriter, vtkXMLUnstructuredGridWriter, vtkXMLWriter
 
-from .. import config
-from ..fields import Field
-from ..geometry import StructuredTopology, Hex, Quad, Line, Patch
-from ..util import ensure_ncomps, prod
-from .writer import Writer
+from .. import api, util
+from ..api import B, CellOrdering, DiscreteTopology, F, NodeShape, S, Source, T, Z
+from ..topology import CellType, StructuredTopology
+from ..util import FieldData
+from .api import OutputMode, Writer, WriterProperties, WriterSettings
 
-from ..typing import Array2D, StepData
 
+class Behavior(Enum):
+    OnlyStructured = auto()
+    OnlyUnstructured = auto()
+    Whatever = auto()
 
 
-def transpose(data, grid, cells=False):
-    if isinstance(grid, vtkStructuredGrid):
-        shape = grid.GetDimensions()
-        if cells:
-            shape = tuple(max(s-1,1) for s in shape)
-        data = data.reshape(*shape, -1).transpose(2, 1, 0, 3).reshape(prod(shape), -1)
-    return data
+Sc = TypeVar("Sc", bound=number)
+BackendWriter = Union[vtkXMLWriter, vtkDataWriter]
 
 
+def transpose(data: FieldData[Sc], grid: vtkPointSet, cellwise: bool = False) -> FieldData[Sc]:
+    if not isinstance(grid, vtkStructuredGrid):
+        return data
+    shape = grid.GetDimensions()
+    if cellwise:
+        i, j, k = shape
+        shape = (max(i - 1, 1), max(j - 1, 1), max(k - 1, 1))
+    return data.transpose(NodeShape(shape), (2, 1, 0))
+
+
+def get_grid(
+    topology: DiscreteTopology, legacy: bool, behavior: Behavior
+) -> Tuple[vtkPointSet, BackendWriter]:
+    if isinstance(topology, StructuredTopology) and behavior != Behavior.OnlyUnstructured:
+        sgrid = vtkStructuredGrid()
+        shape = tuple(topology.cellshape)
+        while len(shape) < 3:
+            shape = (*shape, 0)
+        sgrid.SetDimensions(*(s + 1 for s in shape))
+        if legacy:
+            return sgrid, vtkStructuredGridWriter()
+        else:
+            return sgrid, vtkXMLStructuredGridWriter()
 
-class AbstractVTKWriter(Writer):
-    """Superclass for all VTK format writers."""
+    if behavior == Behavior.OnlyStructured:
+        raise api.Unexpected("Unstructured topology passed to structured-only context")
+    if topology.celltype not in (CellType.Line, CellType.Quadrilateral, CellType.Hexahedron):
+        raise api.Unsupported("VTK writer only supports lines, quadrilaterals and hexahedra")
+
+    ugrid = vtkUnstructuredGrid()
+    cells = (
+        FieldData.join_comps(
+            topology.cells.constant_like(topology.cells.num_comps, ncomps=1, dtype=int),
+            topology.cells_as(CellOrdering.Vtk),
+        )
+        .numpy()
+        .ravel()
+        .astype("i8")
+    )
+    cellarray = vtkCellArray()
+    cellarray.SetCells(len(cells), numpy_to_vtkIdTypeArray(cells))
+    celltype = {
+        CellType.Line: VTK_LINE,
+        CellType.Quadrilateral: VTK_QUAD,
+        CellType.Hexahedron: VTK_HEXAHEDRON,
+    }[topology.celltype]
+    ugrid.SetCells(celltype, cellarray)
+
+    if legacy:
+        return ugrid, vtkUnstructuredGridWriter()
+    else:
+        return ugrid, vtkXMLUnstructuredGridWriter()
+
+
+def apply_output_mode(writer: Union[vtkXMLWriter, vtkDataWriter], mode: OutputMode) -> None:
+    if isinstance(writer, vtkDataWriter):
+        if mode == OutputMode.Binary:
+            writer.SetFileTypeToBinary()
+        elif mode == OutputMode.Ascii:
+            writer.SetFileTypeToASCII()
+    elif isinstance(writer, vtkXMLWriter):
+        if mode == OutputMode.Binary:
+            writer.SetDataModeToBinary()
+        elif mode == OutputMode.Ascii:
+            writer.SetDataModeToAscii()
+        elif mode == OutputMode.Appended:
+            writer.SetDataModeToAppended()
 
-    grid: Optional[vtkDataSet]
 
-    allow_structured: bool
-    require_structured: bool
+class VtkWriterBase(ABC, Writer):
+    filename: Path
+    output_mode: OutputMode = OutputMode.Binary
+    allow_nan_in_ascii: bool
 
-    @staticmethod
-    def nan_filter(data: Array2D) -> Array2D:
-        """Filter out nans in the data array, if necessary."""
-        i, j = np.where(np.isnan(data))
-        if len(i) > 0 and config.output_mode == 'ascii':
-            log.warning("VTK ASCII files do not support NaN, will be set to zero")
-            data[i, j] = 0.0
-        return data
+    def __init__(self, filename: Path):
+        self.filename = filename
+
+    def __enter__(self) -> Self:
+        return self
+
+    def __exit__(self, *args) -> None:
+        return
+
+    @property
+    def properties(self) -> WriterProperties:
+        return WriterProperties(
+            require_single_zone=True,
+            require_single_basis=True,
+            require_discrete_topology=True,
+        )
+
+    def configure(self, settings: WriterSettings) -> None:
+        if settings.output_mode is not None:
+            if settings.output_mode not in (OutputMode.Binary, OutputMode.Ascii):
+                raise api.Unsupported(f"Unsupported output mode for VTK: {settings.output_mode}")
+            self.output_mode = settings.output_mode
 
     @abstractmethod
-    def get_writer(self):
-        pass
+    def grid_and_writer(self, topology: DiscreteTopology) -> Tuple[vtkPointSet, BackendWriter]:
+        ...
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.grid = None
-
-    def update_geometry(self, geometry: Field, patch: Patch, data: Array2D):
-        super().update_geometry(geometry, patch, data)
-
-        if not isinstance(patch.topology, StructuredTopology) and self.require_structured:
-            raise TypeError(f"{self.writer_name} does not support unstructured grids")
-
-        if isinstance(patch.topology, StructuredTopology) and self.allow_structured:
-            if not isinstance(self.grid, vtkStructuredGrid):
-                self.grid = vtkStructuredGrid()
-            shape = patch.topology.shape
-            while len(shape) < 3:
-                shape = (*shape, 0)
-            if not config.fix_orientation:
-                shape = shape[::-1]
-            self.grid.SetDimensions(*(s + 1 for s in shape))
-        elif not self.grid:
-            self.grid = vtkUnstructuredGrid()
+    def consume_timestep(
+        self, step: S, filename: Path, source: Source[B, F, S, DiscreteTopology, Z], geometry: F
+    ) -> None:
+        zone = source.single_zone()
+        topology = source.topology(step, source.basis_of(geometry), zone)
 
-        data = ensure_ncomps(self.nan_filter(data), 3, allow_scalar=False)
+        grid, writer = self.grid_and_writer(topology)
+        apply_output_mode(writer, self.output_mode)
 
-        if config.fix_orientation:
-            data = transpose(data, self.grid)
+        data = source.field_data(step, geometry, zone)
+        data = transpose(data, grid, geometry.cellwise)
 
         points = vtkPoints()
-        points.SetData(numpy_to_vtk(data))
-        self.grid.SetPoints(points)
-
-        if isinstance(self.grid, vtkUnstructuredGrid):
-            if patch.topology.celltype not in [Line(), Quad(), Hex()]:
-                raise TypeError(f"Unexpected cell type found: needed line, quad or hex")
-            cells = patch.topology.cells
-            cells = np.hstack([cells.shape[-1] * np.ones((len(cells), 1), dtype=int), cells]).ravel()
-            cells = cells.astype('i8')
-            cellarray = vtkCellArray()
-            cellarray.SetCells(len(cells), numpy_to_vtkIdTypeArray(cells))
-            if patch.topology.celltype == Hex():
-                celltype = VTK_HEXAHEDRON
-            elif patch.topology.celltype == Quad():
-                celltype = VTK_QUAD
+        p = data.ensure_ncomps(3, allow_scalar=False)
+        points.SetData(p.vtk())
+        grid.SetPoints(points)
+
+        for field in source.fields(source.single_basis()):
+            if field.is_geometry:
+                continue
+            target = grid.GetCellData() if field.cellwise else grid.GetPointData()
+            data = source.field_data(step, field, zone)
+            if field.is_displacement:
+                data = data.ensure_ncomps(3, allow_scalar=False, pad_right=False)
             else:
-                celltype = VTK_LINE
-            self.grid.SetCells(celltype, cellarray)
-
-    def update_field(self, field: Field, patch: Patch, data: Array2D):
-        target = self.grid.GetCellData() if field.cells else self.grid.GetPointData()
-        data = ensure_ncomps(self.nan_filter(data), 3, allow_scalar=field.is_scalar)
-        data = transpose(data, self.grid, cells=field.cells)
-        array = numpy_to_vtk(data)
-        array.SetName(field.name)
-        target.AddArray(array)
-
-    @contextmanager
-    def step(self, stepdata: StepData):
-        with super().step(stepdata) as step:
-            yield step
+                data = data.ensure_ncomps(3, allow_scalar=field.is_scalar)
+            data = transpose(data, grid, field.cellwise)
+            if self.output_mode == OutputMode.Ascii and not self.allow_nan_in_ascii:
+                data = data.nan_filter()
+            array = data.vtk()
+            array.SetName(field.name)
+            target.AddArray(array)
 
-        filename = self.make_filename(with_step=True)
-        writer = self.get_writer()
         writer.SetFileName(str(filename))
-        writer.SetInputData(self.grid)
+        writer.SetInputData(grid)
         writer.Write()
 
-        log.user(filename)
-
-
-class VTKLegacyWriter(AbstractVTKWriter):
-    """Writer for VTK legacy format."""
-
-    writer_name = "VTK-legacy"
-
-    allow_structured = True
-    require_structured = False
+        logging.info(filename)
 
-    @classmethod
-    def applicable(cls, fmt: str) -> bool:
-        return fmt == 'vtk'
+    def consume(self, source: Source[B, F, S, T, Z], geometry: F) -> None:
+        casted = source.cast_discrete_topology()
+        filenames = util.filename_generator(self.filename, source.properties.instantaneous)
+        for step, filename in zip(casted.steps(), filenames):
+            self.consume_timestep(step, filename, casted, geometry)
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if config.require_unstructured:
-            self.allow_structured = False
 
-    def validate(self):
-        config.require_in(reason="not supported by VTK", output_mode=('binary', 'ascii'))
-
-    def get_writer(self):
-        if isinstance(self.grid, vtkStructuredGrid):
-            writer = vtkStructuredGridWriter()
-        else:
-            writer = vtkUnstructuredGridWriter()
-        if config.output_mode == 'ascii':
-            writer.SetFileTypeToASCII()
-        else:
-            writer.SetFileTypeToBinary()
-        return writer
+class VtkWriter(VtkWriterBase):
+    allow_nan_in_ascii = False
 
+    def __init__(self, filename: Path):
+        super().__init__(filename)
 
-class VTKXMLWriter(AbstractVTKWriter):
-    """Writer for VTK XML-based format."""
+    def grid_and_writer(self, topology: DiscreteTopology) -> Tuple[vtkPointSet, BackendWriter]:
+        return get_grid(topology, legacy=True, behavior=Behavior.Whatever)
 
-    @abstractclassmethod
-    def applicable(cls, fmt: str) -> bool:
-        pass
 
-    def validate(self):
-        super().validate()
-        config.require_in(reason=f"not supported by {self.writer_name}", output_mode=('binary', 'ascii', 'appended'))
+class VtuWriter(VtkWriterBase):
+    allow_nan_in_ascii = True
 
-    @staticmethod
-    def nan_filter(data: Array2D) -> Array2D:
-        return data
+    def __init__(self, filename: Path):
+        super().__init__(filename)
 
-    def get_writer(self):
-        if isinstance(self.grid, vtkStructuredGrid):
-            writer = vtkXMLStructuredGridWriter()
-        else:
-            writer = vtkXMLUnstructuredGridWriter()
-        if config.output_mode == 'appended':
-            writer.SetDataModeToAppended()
-        elif config.output_mode == 'ascii':
-            writer.SetDataModeToAscii()
-        elif config.output_mode == 'binary':
-            writer.SetDataModeToBinary()
-        return writer
+    def grid_and_writer(self, topology: DiscreteTopology) -> Tuple[vtkPointSet, BackendWriter]:
+        return get_grid(topology, legacy=False, behavior=Behavior.OnlyUnstructured)
 
 
-class VTUWriter(VTKXMLWriter):
-    """Writer for VTU format (XML-based unstructured grid)."""
+class VtsWriter(VtkWriterBase):
+    allow_nan_in_ascii = True
 
-    writer_name = "VTU"
-    allow_structured = False
-    require_structured = False
+    def __init__(self, filename: Path):
+        super().__init__(filename)
 
-    @classmethod
-    def applicable(cls, fmt: str) -> bool:
-        return fmt == 'vtu'
+    def grid_and_writer(self, topology: DiscreteTopology) -> Tuple[vtkPointSet, BackendWriter]:
+        return get_grid(topology, legacy=False, behavior=Behavior.OnlyStructured)
 
 
-class VTSWriter(VTKXMLWriter):
-    """Writer for VTS format (XML-based structured grid)."""
+class PvdWriter(VtuWriter):
+    pvd_dirname: Path
+    pvd_filename: Path
+    pvd: IO[str]
 
-    writer_name = "VTS"
-    allow_structured = True
-    require_structured = True
+    def __init__(self, filename: Path):
+        self.pvd_filename = filename
+        self.pvd_dirname = filename.with_suffix(f"{filename.suffix}-data")
+        super().__init__(self.pvd_dirname / "data.vtu")
 
-    @classmethod
-    def applicable(cls, fmt: str) -> bool:
-        return fmt == 'vts'
-
-
-class PVDWriter(VTUWriter):
-    """Writer for PVD format (XML-based file with links to other files per timestep)."""
-
-    writer_name = "PVD"
-
-    pvd: TextIO
-
-    @classmethod
-    def applicable(cls, fmt: str) -> bool:
-        return fmt == 'pvd'
-
-    def __init__(self, outpath: Path):
-        self.rootfile = outpath
-        super().__init__(outpath.with_suffix(f'{outpath.suffix}-data') / 'data.vtu')
-
-    def __enter__(self):
-        super().__enter__()
-        self.pvd = open(self.rootfile, 'w')
+    def __enter__(self) -> Self:
+        self.pvd_dirname.mkdir(exist_ok=True, parents=True)
+        self.pvd = self.pvd_filename.open("w").__enter__()
         self.pvd.write('<VTKFile type="Collection">\n')
-        self.pvd.write('  <Collection>\n')
-        return self
+        self.pvd.write("  <Collection>\n")
+        return super().__enter__()
 
-    def __exit__(self, type_, value, backtrace):
-        super().__exit__(type_, value, backtrace)
-        if value is not None:
-            self.pvd.close()
-        else:
-            self.pvd.write('  </Collection>\n')
-            self.pvd.write('</VTKFile>\n')
-            self.pvd.close()
-            log.user(self.rootfile)
-
-    def make_filename(self, *args, **kwargs):
-        filename = super().make_filename(*args, **kwargs)
-        makedirs(filename.parent, mode=0o775, exist_ok=True)
-        return filename
-
-    @contextmanager
-    def step(self, stepdata: StepData):
-        with super().step(stepdata) as step:
-            yield step
-        filename = self.make_filename(with_step=True)
-        relative_filename = filename.relative_to(self.rootfile.parent)
-        if self.stepdata:
-            timestep = next(iter(self.stepdata.values()))
+    def __exit__(self, *args) -> None:
+        super().__exit__(*args)
+        self.pvd.write("  </Collection>\n")
+        self.pvd.write("</VTKFile>\n")
+        self.pvd.__exit__(*args)
+        logging.info(self.pvd_filename)
+
+    def consume_timestep(
+        self, timestep: S, filename: Path, source: Source[B, F, S, DiscreteTopology, Z], geometry: F
+    ) -> None:
+        super().consume_timestep(timestep, filename, source, geometry)
+        relative_filename = filename.relative_to(self.pvd_filename.parent)
+        if timestep.value is not None:
+            time = timestep.value
         else:
-            timestep = self.stepid
-        self.pvd.write('    <DataSet timestep="{}" part="0" file="{}" />\n'.format(timestep, relative_filename))
+            time = timestep.index
+        self.pvd.write(f'    <DataSet timestep="{time}" part="0" file="{relative_filename}" />\n')
```

