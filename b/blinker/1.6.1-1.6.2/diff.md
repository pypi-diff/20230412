# Comparing `tmp/blinker-1.6.1.tar.gz` & `tmp/blinker-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ubuntu/blinker/dist/.tmp-tx6nq4mi/blinker-1.6.1.tar", last modified: Sun Apr  9 15:26:19 2023, max compression
+gzip compressed data, was "blinker-1.6.2.tar", last modified: Wed Apr 12 21:44:54 2023, max compression
```

## Comparing `blinker-1.6.1.tar` & `blinker-1.6.2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2752 2023-04-09 15:23:14.000000 blinker-1.6.1/CHANGES.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1054 2023-04-02 13:58:17.000000 blinker-1.6.1/LICENSE.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2023-04-02 13:58:17.000000 blinker-1.6.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1964 2023-04-09 15:26:19.289915 blinker-1.6.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      990 2023-04-02 13:58:17.000000 blinker-1.6.1/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      634 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/Makefile
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/docs/_static/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3627 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/_static/blinker-named.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1195 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9761 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      765 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/make.bat
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2023-04-09 15:23:14.000000 blinker-1.6.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-09 15:26:19.289915 blinker-1.6.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/src/blinker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      409 2023-04-09 15:23:14.000000 blinker-1.6.1/src/blinker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9081 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/_saferef.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/_utilities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20317 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/py.typed
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/src/blinker.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1964 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_context.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3747 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_saferef.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12962 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_signals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_utilities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      591 2023-04-02 13:58:17.000000 blinker-1.6.1/tox.ini
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/
+-rw-r--r--   0 david     (1000) david     (1000)     2914 2023-04-12 21:40:57.000000 blinker-1.6.2/CHANGES.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1054 2022-07-17 16:16:47.000000 blinker-1.6.2/LICENSE.rst
+-rw-r--r--   0 david     (1000) david     (1000)      127 2023-04-12 20:57:17.000000 blinker-1.6.2/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)     1964 2023-04-12 21:44:54.569893 blinker-1.6.2/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      990 2023-04-12 20:57:17.000000 blinker-1.6.2/README.rst
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/docs/
+-rw-r--r--   0 david     (1000) david     (1000)      634 2022-07-17 16:16:47.000000 blinker-1.6.2/docs/Makefile
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/docs/_static/
+-rw-r--r--   0 david     (1000) david     (1000)     3627 2022-07-17 16:16:47.000000 blinker-1.6.2/docs/_static/blinker-named.png
+-rw-r--r--   0 david     (1000) david     (1000)     1195 2023-04-12 20:57:17.000000 blinker-1.6.2/docs/conf.py
+-rw-r--r--   0 david     (1000) david     (1000)     9761 2023-04-12 20:57:17.000000 blinker-1.6.2/docs/index.rst
+-rw-r--r--   0 david     (1000) david     (1000)      765 2022-07-17 16:16:47.000000 blinker-1.6.2/docs/make.bat
+-rw-r--r--   0 david     (1000) david     (1000)     1829 2023-04-12 21:01:56.000000 blinker-1.6.2/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-04-12 21:44:54.569893 blinker-1.6.2/setup.cfg
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/src/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/src/blinker/
+-rw-r--r--   0 david     (1000) david     (1000)      408 2023-04-12 21:40:57.000000 blinker-1.6.2/src/blinker/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     9096 2023-04-12 21:15:04.000000 blinker-1.6.2/src/blinker/_saferef.py
+-rw-r--r--   0 david     (1000) david     (1000)     4110 2023-04-12 21:18:59.000000 blinker-1.6.2/src/blinker/_utilities.py
+-rw-r--r--   0 david     (1000) david     (1000)    20469 2023-04-12 21:23:17.000000 blinker-1.6.2/src/blinker/base.py
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-04-12 20:57:17.000000 blinker-1.6.2/src/blinker/py.typed
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/src/blinker.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     1964 2023-04-12 21:44:54.000000 blinker-1.6.2/src/blinker.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      501 2023-04-12 21:44:54.000000 blinker-1.6.2/src/blinker.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-04-12 21:44:54.000000 blinker-1.6.2/src/blinker.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        8 2023-04-12 21:44:54.000000 blinker-1.6.2/src/blinker.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-12 21:44:54.569893 blinker-1.6.2/tests/
+-rw-r--r--   0 david     (1000) david     (1000)     1053 2023-04-12 20:57:17.000000 blinker-1.6.2/tests/test_context.py
+-rw-r--r--   0 david     (1000) david     (1000)     3747 2023-04-12 20:57:17.000000 blinker-1.6.2/tests/test_saferef.py
+-rw-r--r--   0 david     (1000) david     (1000)    12962 2023-04-12 20:57:17.000000 blinker-1.6.2/tests/test_signals.py
+-rw-r--r--   0 david     (1000) david     (1000)      451 2023-04-12 20:57:17.000000 blinker-1.6.2/tests/test_utilities.py
+-rw-r--r--   0 david     (1000) david     (1000)      591 2023-04-12 20:57:17.000000 blinker-1.6.2/tox.ini
```

### Comparing `blinker-1.6.1/CHANGES.rst` & `blinker-1.6.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Version 1.6.2
+-------------
+
+Released 2023-04-12
+
+-   Type annotations are not evaluated at runtime. typing-extensions is not a runtime
+    dependency. :pr:`94`
+
 Version 1.6.1
 -------------
 
 Released 2023-04-09
 
 -   Ensure that py.typed is present in the distributions (to enable other
     projects to use blinker's typing).
```

### Comparing `blinker-1.6.1/LICENSE.rst` & `blinker-1.6.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/PKG-INFO` & `blinker-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blinker
-Version: 1.6.1
+Version: 1.6.2
 Summary: Fast, simple object-to-object and broadcast signaling
 Author-email: Jason Kirtland <jek@discorporate.us>
 Maintainer-email: Pallets Ecosystem <contact@palletsprojects.com>
 License: MIT License
 Project-URL: Homepage, https://blinker.readthedocs.io
 Project-URL: Documentation, https://blinker.readthedocs.io
 Project-URL: Source Code, https://github.com/pallets-eco/blinker/
```

### Comparing `blinker-1.6.1/README.rst` & `blinker-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/docs/Makefile` & `blinker-1.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/docs/_static/blinker-named.png` & `blinker-1.6.2/docs/_static/blinker-named.png`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/docs/conf.py` & `blinker-1.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/docs/index.rst` & `blinker-1.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/docs/make.bat` & `blinker-1.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/pyproject.toml` & `blinker-1.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">= 3.7"
 dynamic = ["version"]
-dependencies = ["typing-extensions>=4.2"]
 
 [project.urls]
 Homepage = "https://blinker.readthedocs.io"
 Documentation = "https://blinker.readthedocs.io"
 "Source Code" = "https://github.com/pallets-eco/blinker/"
 "Issue Tracker" = "https://github.com/pallets-eco/blinker/issues/"
 Chat = "https://discord.gg/pallets"
```

### Comparing `blinker-1.6.1/src/blinker/_saferef.py` & `blinker-1.6.2/src/blinker/_saferef.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
       BoundMethodWeakref objects indexed by the class's
       calculate_key(target) method applied to the target objects.
       This weak value dictionary is used to short-circuit creation so
       that multiple references to the same (object, function) pair
       produce the same BoundMethodWeakref instance.
     """
 
-    _all_instances = weakref.WeakValueDictionary()  # type: ignore
+    _all_instances = weakref.WeakValueDictionary()  # type: ignore[var-annotated]
 
     def __new__(cls, target, on_delete=None, *arguments, **named):
         """Create new instance or return current instance.
 
         Basically this method of construction allows us to
         short-circuit creation of references to already-referenced
         instance methods.  The key corresponding to the target is
```

### Comparing `blinker-1.6.1/src/blinker/_utilities.py` & `blinker-1.6.2/src/blinker/_utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import inspect
 import sys
 import typing as t
 from functools import partial
 from weakref import ref
 
@@ -36,28 +38,28 @@
     A slight refinement of the MAGICCOOKIE=object() pattern.  The primary
     advantage of symbol() is its repr().  They are also singletons.
 
     Repeated calls of symbol('name') will all return the same instance.
 
     """
 
-    symbols = {}  # type: ignore
+    symbols = {}  # type: ignore[var-annotated]
 
     def __new__(cls, name):
         try:
             return cls.symbols[name]
         except KeyError:
             return cls.symbols.setdefault(name, _symbol(name))
 
 
 def hashable_identity(obj: object) -> IdentityType:
     if hasattr(obj, "__func__"):
-        return (id(obj.__func__), id(obj.__self__))  # type: ignore
+        return (id(obj.__func__), id(obj.__self__))  # type: ignore[attr-defined]
     elif hasattr(obj, "im_func"):
-        return (id(obj.im_func), id(obj.im_self))  # type: ignore
+        return (id(obj.im_func), id(obj.im_self))  # type: ignore[attr-defined]
     elif isinstance(obj, (int, str)):
         return obj
     else:
         return id(obj)
 
 
 WeakTypes = (ref, BoundMethodWeakref)
@@ -66,25 +68,25 @@
 class annotatable_weakref(ref):
     """A weakref.ref that supports custom instance attributes."""
 
     receiver_id: t.Optional[IdentityType]
     sender_id: t.Optional[IdentityType]
 
 
-def reference(  # type: ignore
+def reference(  # type: ignore[no-untyped-def]
     object, callback=None, **annotations
 ) -> annotatable_weakref:
     """Return an annotated weak ref."""
     if callable(object):
         weak = callable_reference(object, callback)
     else:
         weak = annotatable_weakref(object, callback)
     for key, value in annotations.items():
         setattr(weak, key, value)
-    return weak  # type: ignore
+    return weak  # type: ignore[no-any-return]
 
 
 def callable_reference(object, callback=None):
     """Return an annotated weak ref, supporting bound instance methods."""
     if hasattr(object, "im_self") and object.im_self is not None:
         return BoundMethodWeakref(target=object, on_delete=callback)
     elif hasattr(object, "__self__") and object.__self__ is not None:
@@ -114,26 +116,27 @@
     if sys.version_info >= (3, 8):
         return asyncio.iscoroutinefunction(func)
     else:
         # Note that there is something special about the AsyncMock
         # such that it isn't determined as a coroutine function
         # without an explicit check.
         try:
-            from unittest.mock import AsyncMock  # type: ignore
+            from unittest.mock import AsyncMock  # type: ignore[attr-defined]
 
             if isinstance(func, AsyncMock):
                 return True
         except ImportError:
             # Not testing, no asynctest to import
             pass
 
         while inspect.ismethod(func):
             func = func.__func__
         while isinstance(func, partial):
             func = func.func
         if not inspect.isfunction(func):
             return False
-        result = bool(func.__code__.co_flags & inspect.CO_COROUTINE)
-        return (
-            result
-            or getattr(func, "_is_coroutine", None) is asyncio.coroutines._is_coroutine  # type: ignore  # noqa: B950
-        )
+
+        if func.__code__.co_flags & inspect.CO_COROUTINE:
+            return True
+
+        acic = asyncio.coroutines._is_coroutine  # type: ignore[attr-defined]
+        return getattr(func, "_is_coroutine", None) is acic
```

### Comparing `blinker-1.6.1/src/blinker/base.py` & `blinker-1.6.2/src/blinker/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,66 +3,68 @@
 A small implementation of signals, inspired by a snippet of Django signal
 API client code seen in a blog post.  Signals are first-class objects and
 each manages its own receivers and message emission.
 
 The :func:`signal` function provides singleton behavior for named signals.
 
 """
+from __future__ import annotations
+
 import typing as t
 from collections import defaultdict
 from contextlib import contextmanager
 from warnings import warn
 from weakref import WeakValueDictionary
 
-import typing_extensions as te
-
 from blinker._utilities import annotatable_weakref
 from blinker._utilities import hashable_identity
 from blinker._utilities import IdentityType
 from blinker._utilities import is_coroutine_function
 from blinker._utilities import lazy_property
 from blinker._utilities import reference
 from blinker._utilities import symbol
 from blinker._utilities import WeakTypes
 
+if t.TYPE_CHECKING:
+    import typing_extensions as te
 
-ANY = symbol("ANY")
-ANY.__doc__ = 'Token for "any sender".'
-ANY_ID = 0
+    T_callable = t.TypeVar("T_callable", bound=t.Callable[..., t.Any])
 
-T_callable = t.TypeVar("T_callable", bound=t.Callable)
+    T = t.TypeVar("T")
+    P = te.ParamSpec("P")
 
-T = t.TypeVar("T")
-P = te.ParamSpec("P")
+    AsyncWrapperType = t.Callable[[t.Callable[P, T]], t.Callable[P, t.Awaitable[T]]]
+    SyncWrapperType = t.Callable[[t.Callable[P, t.Awaitable[T]]], t.Callable[P, T]]
 
-AsyncWrapperType = t.Callable[[t.Callable[P, T]], t.Callable[P, t.Awaitable[T]]]
-SyncWrapperType = t.Callable[[t.Callable[P, t.Awaitable[T]]], t.Callable[P, T]]
+ANY = symbol("ANY")
+ANY.__doc__ = 'Token for "any sender".'
+ANY_ID = 0
 
 
 class Signal:
     """A notification emitter."""
 
     #: An :obj:`ANY` convenience synonym, allows ``Signal.ANY``
     #: without an additional import.
     ANY = ANY
 
     @lazy_property
-    def receiver_connected(self) -> "Signal":
+    def receiver_connected(self) -> Signal:
         """Emitted after each :meth:`connect`.
 
         The signal sender is the signal instance, and the :meth:`connect`
         arguments are passed through: *receiver*, *sender*, and *weak*.
 
         .. versionadded:: 1.2
 
         """
         return Signal(doc="Emitted after a receiver connects.")
 
     @lazy_property
-    def receiver_disconnected(self) -> "Signal":
+    def receiver_disconnected(self) -> Signal:
         """Emitted after :meth:`disconnect`.
 
         The sender is the signal instance, and the :meth:`disconnect` arguments
         are passed through: *receiver* and *sender*.
 
         Note, this signal is emitted **only** when :meth:`disconnect` is
         called explicitly.
@@ -77,35 +79,33 @@
         callback on weak receivers and senders.
 
         .. versionadded:: 1.2
 
         """
         return Signal(doc="Emitted after a receiver disconnects.")
 
-    def __init__(self, doc: t.Optional[str] = None) -> None:
+    def __init__(self, doc: str | None = None) -> None:
         """
         :param doc: optional.  If provided, will be assigned to the signal's
           __doc__ attribute.
 
         """
         if doc:
             self.__doc__ = doc
         #: A mapping of connected receivers.
         #:
         #: The values of this mapping are not meaningful outside of the
         #: internal :class:`Signal` implementation, however the boolean value
         #: of the mapping is useful as an extremely efficient check to see if
         #: any receivers are connected to the signal.
-        self.receivers: t.Dict[
-            IdentityType, t.Union[t.Callable, annotatable_weakref]
-        ] = {}
+        self.receivers: dict[IdentityType, t.Callable | annotatable_weakref] = {}
         self.is_muted = False
-        self._by_receiver: t.Dict[IdentityType, t.Set[IdentityType]] = defaultdict(set)
-        self._by_sender: t.Dict[IdentityType, t.Set[IdentityType]] = defaultdict(set)
-        self._weak_senders: t.Dict[IdentityType, annotatable_weakref] = {}
+        self._by_receiver: dict[IdentityType, set[IdentityType]] = defaultdict(set)
+        self._by_sender: dict[IdentityType, set[IdentityType]] = defaultdict(set)
+        self._weak_senders: dict[IdentityType, annotatable_weakref] = {}
 
     def connect(
         self, receiver: T_callable, sender: t.Any = ANY, weak: bool = True
     ) -> T_callable:
         """Connect *receiver* to signal events sent by *sender*.
 
         :param receiver: A callable.  Will be invoked by :meth:`send` with
@@ -121,15 +121,16 @@
 
         :param weak: If true, the Signal will hold a weakref to *receiver*
           and automatically disconnect when *receiver* goes out of scope or
           is garbage collected.  Defaults to True.
 
         """
         receiver_id = hashable_identity(receiver)
-        receiver_ref: t.Union[annotatable_weakref, T_callable]
+        receiver_ref: T_callable | annotatable_weakref
+
         if weak:
             receiver_ref = reference(receiver, self._cleanup_receiver)
             receiver_ref.receiver_id = receiver_id
         else:
             receiver_ref = receiver
         sender_id: IdentityType
         if sender is ANY:
@@ -267,17 +268,17 @@
             DeprecationWarning,
         )
         return self.connected_to(receiver, sender)
 
     def send(
         self,
         *sender: t.Any,
-        _async_wrapper: t.Optional[AsyncWrapperType] = None,
+        _async_wrapper: AsyncWrapperType | None = None,
         **kwargs: t.Any,
-    ) -> t.List[t.Tuple[t.Callable, t.Any]]:
+    ) -> list[tuple[t.Callable, t.Any]]:
         """Emit this signal on behalf of *sender*, passing on ``kwargs``.
 
         Returns a list of 2-tuples, pairing receivers with their return
         value. The ordering of receiver notification is undefined.
 
         :param sender: Any object or ``None``.  If omitted, synonymous
           with ``None``.  Only accepts one positional argument.
@@ -292,23 +293,24 @@
         sender = self._extract_sender(sender)
         results = []
         for receiver in self.receivers_for(sender):
             if is_coroutine_function(receiver):
                 if _async_wrapper is None:
                     raise RuntimeError("Cannot send to a coroutine function")
                 receiver = _async_wrapper(receiver)
-            results.append((receiver, receiver(sender, **kwargs)))  # type: ignore
+            result = receiver(sender, **kwargs)  # type: ignore[call-arg]
+            results.append((receiver, result))
         return results
 
     async def send_async(
         self,
         *sender: t.Any,
-        _sync_wrapper: t.Optional[SyncWrapperType] = None,
+        _sync_wrapper: SyncWrapperType | None = None,
         **kwargs: t.Any,
-    ) -> t.List[t.Tuple[t.Callable, t.Any]]:
+    ) -> list[tuple[t.Callable, t.Any]]:
         """Emit this signal on behalf of *sender*, passing on ``kwargs``.
 
         Returns a list of 2-tuples, pairing receivers with their return
         value. The ordering of receiver notification is undefined.
 
         :param sender: Any object or ``None``.  If omitted, synonymous
           with ``None``. Only accepts one positional argument.
@@ -322,19 +324,20 @@
 
         sender = self._extract_sender(sender)
         results = []
         for receiver in self.receivers_for(sender):
             if not is_coroutine_function(receiver):
                 if _sync_wrapper is None:
                     raise RuntimeError("Cannot send to a non-coroutine function")
-                receiver = _sync_wrapper(receiver)  # type: ignore
-            results.append((receiver, await receiver(sender, **kwargs)))  # type: ignore
+                receiver = _sync_wrapper(receiver)  # type: ignore[arg-type]
+            result = await receiver(sender, **kwargs)  # type: ignore[call-arg, misc]
+            results.append((receiver, result))
         return results
 
-    def _extract_sender(self, sender):
+    def _extract_sender(self, sender: t.Any) -> t.Any:
         if not self.receivers:
             # Ensure correct signature even on no-op sends, disable with -O
             # for lowest possible cost.
             if __debug__ and sender and len(sender) > 1:
                 raise TypeError(
                     f"send() accepts only one positional argument, {len(sender)} given"
                 )
@@ -367,15 +370,15 @@
             return True
         if sender is ANY:
             return False
         return hashable_identity(sender) in self._by_sender
 
     def receivers_for(
         self, sender: t.Any
-    ) -> t.Generator[t.Union[t.Callable, annotatable_weakref], None, None]:
+    ) -> t.Generator[t.Callable | annotatable_weakref, None, None]:
         """Iterate all live receivers listening for *sender*."""
         # TODO: test receivers_for(ANY)
         if self.receivers:
             sender_id = hashable_identity(sender)
             if sender_id in self._by_sender:
                 ids = self._by_sender[ANY_ID] | self._by_sender[sender_id]
             else:
@@ -386,16 +389,15 @@
                     continue
                 if isinstance(receiver, WeakTypes):
                     strong = receiver()
                     if strong is None:
                         self._disconnect(receiver_id, ANY_ID)
                         continue
                     receiver = strong
-                receiver = t.cast(t.Union[t.Callable, annotatable_weakref], receiver)
-                yield receiver
+                yield receiver  # type: ignore[misc]
 
     def disconnect(self, receiver: t.Callable, sender: t.Any = ANY) -> None:
         """Disconnect *receiver* from this signal's events.
 
         :param receiver: a previously :meth:`connected<connect>` callable
 
         :param sender: a specific sender to disconnect from, or :obj:`ANY`
@@ -491,57 +493,59 @@
 """
 )
 
 
 class NamedSignal(Signal):
     """A named generic notification emitter."""
 
-    def __init__(self, name: str, doc: t.Optional[str] = None) -> None:
+    def __init__(self, name: str, doc: str | None = None) -> None:
         Signal.__init__(self, doc)
 
         #: The name of this signal.
         self.name = name
 
     def __repr__(self) -> str:
         base = Signal.__repr__(self)
         return f"{base[:-1]}; {self.name!r}>"
 
 
 class Namespace(dict):
     """A mapping of signal names to signals."""
 
-    def signal(self, name: str, doc: t.Optional[str] = None) -> NamedSignal:
+    def signal(self, name: str, doc: str | None = None) -> NamedSignal:
         """Return the :class:`NamedSignal` *name*, creating it if required.
 
         Repeated calls to this function will return the same signal object.
 
         """
         try:
-            return self[name]  # type: ignore
+            return self[name]  # type: ignore[no-any-return]
         except KeyError:
-            return self.setdefault(name, NamedSignal(name, doc))  # type: ignore
+            result = self.setdefault(name, NamedSignal(name, doc))
+            return result  # type: ignore[no-any-return]
 
 
 class WeakNamespace(WeakValueDictionary):
     """A weak mapping of signal names to signals.
 
     Automatically cleans up unused Signals when the last reference goes out
     of scope.  This namespace implementation exists for a measure of legacy
     compatibility with Blinker <= 1.2, and may be dropped in the future.
 
     .. versionadded:: 1.3
 
     """
 
-    def signal(self, name: str, doc: t.Optional[str] = None) -> NamedSignal:
+    def signal(self, name: str, doc: str | None = None) -> NamedSignal:
         """Return the :class:`NamedSignal` *name*, creating it if required.
 
         Repeated calls to this function will return the same signal object.
 
         """
         try:
-            return self[name]  # type: ignore
+            return self[name]  # type: ignore[no-any-return]
         except KeyError:
-            return self.setdefault(name, NamedSignal(name, doc))  # type: ignore
+            result = self.setdefault(name, NamedSignal(name, doc))
+            return result  # type: ignore[no-any-return]
 
 
 signal = Namespace().signal
```

### Comparing `blinker-1.6.1/src/blinker.egg-info/PKG-INFO` & `blinker-1.6.2/src/blinker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blinker
-Version: 1.6.1
+Version: 1.6.2
 Summary: Fast, simple object-to-object and broadcast signaling
 Author-email: Jason Kirtland <jek@discorporate.us>
 Maintainer-email: Pallets Ecosystem <contact@palletsprojects.com>
 License: MIT License
 Project-URL: Homepage, https://blinker.readthedocs.io
 Project-URL: Documentation, https://blinker.readthedocs.io
 Project-URL: Source Code, https://github.com/pallets-eco/blinker/
```

### Comparing `blinker-1.6.1/tests/test_context.py` & `blinker-1.6.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/tests/test_saferef.py` & `blinker-1.6.2/tests/test_saferef.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/tests/test_signals.py` & `blinker-1.6.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.1/tox.ini` & `blinker-1.6.2/tox.ini`

 * *Files identical despite different names*

