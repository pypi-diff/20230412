# Comparing `tmp/tarina-0.2.2.tar.gz` & `tmp/tarina-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.2.2.tar", last modified: Wed Apr 12 10:00:04 2023, max compression
+gzip compressed data, was "tarina-0.2.3.tar", last modified: Wed Apr 12 14:50:05 2023, max compression
```

## Comparing `tarina-0.2.2.tar` & `tarina-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.471043 tarina-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 09:59:44.000000 tarina-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 09:59:44.000000 tarina-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 10:00:04.467043 tarina-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 09:59:44.000000 tarina-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 09:59:44.000000 tarina-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:00:04.471043 tarina-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 09:59:44.000000 tarina-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.463043 tarina-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.467043 tarina-0.2.2/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_op.h
--rw-r--r--   0 runner    (1001) docker     (123)   204169 2023-04-12 09:59:54.000000 tarina-0.2.2/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.467043 tarina-0.2.2/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.516930 tarina-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 14:49:48.000000 tarina-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 14:49:48.000000 tarina-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 14:50:05.516930 tarina-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 14:49:48.000000 tarina-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 14:49:48.000000 tarina-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:50:05.516930 tarina-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 14:49:48.000000 tarina-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.512930 tarina-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.516930 tarina-0.2.3/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (123)   200403 2023-04-12 14:49:56.000000 tarina-0.2.3/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.516930 tarina-0.2.3/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/top_level.txt
```

### Comparing `tarina-0.2.2/LICENSE` & `tarina-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/PKG-INFO` & `tarina-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.2.2/pyproject.toml` & `tarina-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tarina"
-version = "0.2.2"
+version = "0.2.3"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
```

### Comparing `tarina-0.2.2/setup.py` & `tarina-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/_lru_c.c` & `tarina-0.2.3/src/tarina/_lru_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -426,20 +426,23 @@
 
     /* Trying to access the item by key. */
     result = lru_subscript(self, key);
 
     if (result)
         /* result != NULL, delete it from dict by key */
         lru_ass_sub(self, key, NULL);
-    else if (default_obj) {
-        /* result == NULL, i.e. key missing, and default_obj given */
-        PyErr_Clear();
-        Py_INCREF(default_obj);
-        result = default_obj;
+        return result;
+
+    if (!default_obj) {
+        Py_RETURN_NONE;
     }
+    /* result == NULL, i.e. key missing, and default_obj given */
+    PyErr_Clear();
+    Py_INCREF(default_obj);
+    result = default_obj;
     /* Otherwise (key missing, and default_obj not given [i.e. == NULL]), the
      * call to lru_subscript (at the location marked by "Trying to access the
      * item by key" in the comments) has already generated the appropriate
      * exception. */
 
     return result;
 }
@@ -617,23 +620,23 @@
     {"values", (PyCFunction)LRU_values, METH_NOARGS,
                     PyDoc_STR("L.values() -> list of L's values in MRU order")},
     {"items", (PyCFunction)LRU_items, METH_NOARGS,
                     PyDoc_STR("L.items() -> list of L's items (key,value) in MRU order")},
     {"has_key",	(PyCFunction)LRU_contains, METH_VARARGS,
                     PyDoc_STR("L.has_key(key) -> Check if key is there in L")},
     {"get",	(PyCFunction)LRU_get, METH_VARARGS,
-                    PyDoc_STR("L.get(key, instead) -> If L has key return its value, otherwise instead")},
+                    PyDoc_STR("L.get(key[, instead]) -> If L has key return its value, otherwise instead")},
     {"setdefault", (PyCFunction)LRU_setdefault, METH_VARARGS,
                     PyDoc_STR("L.setdefault(key, default=None) -> If L has key return its value, otherwise insert key with a value of default and return default")},
     {"pop", (PyCFunction)LRU_pop, METH_VARARGS,
                     PyDoc_STR("L.pop(key[, default]) -> If L has key return its value and remove it from L, otherwise return default. If default is not given and key is not in L, a KeyError is raised.")},
     {"popitem", (PyCFunction)LRU_popitem, METH_VARARGS | METH_KEYWORDS,
                     PyDoc_STR("L.popitem([least_recent=True]) -> Returns and removes a (key, value) pair. The pair returned is the least-recently used if least_recent is true, or the most-recently used if false.")},
     {"set_size", (PyCFunction)LRU_set_size, METH_VARARGS,
-                    PyDoc_STR("L.set_size() -> set size of LRU")},
+                    PyDoc_STR("L.set_size(size) -> set size of LRU")},
     {"get_size", (PyCFunction)LRU_get_size, METH_NOARGS,
                     PyDoc_STR("L.get_size() -> get size of LRU")},
     {"clear", (PyCFunction)LRU_clear, METH_NOARGS,
                     PyDoc_STR("L.clear() -> clear LRU")},
     {"get_stats", (PyCFunction)LRU_get_stats, METH_NOARGS,
                     PyDoc_STR("L.get_stats() -> returns a tuple with cache hits and misses")},
     {"peek_first_item", (PyCFunction)LRU_peek_first_item, METH_NOARGS,
```

### Comparing `tarina-0.2.2/src/tarina/_lru_c.pyi` & `tarina-0.2.3/src/tarina/_lru_c.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 
 class LRU(Generic[_KT, _VT]):
 
     def __init__(
         self, size: int, callback: Callable[[_KT, _VT], Any] | None = ...
     ) -> None: ...
     def clear(self) -> None: ...
-    def get(self, key: _KT, default: _VT | _T) -> _VT | _T: ...
+    @overload
+    def get(self, key: _KT) -> _VT | None: ...
+    @overload
+    def get(self, key: _KT, instead: _VT | _T) -> _VT | _T: ...
 
     def get_size(self) -> int: ...
     def has_key(self, key: _KT) -> bool: ...
     def keys(self) -> list[_KT]: ...
     def values(self) -> list[_VT]: ...
     def items(self) -> list[tuple[_KT, _VT]]: ...
     def peek_first_item(self) -> tuple[_KT, _VT] | None: ...
     def peek_last_item(self) -> tuple[_KT, _VT] | None: ...
     @overload
-    def pop(self, key: _KT) -> _VT: ...
+    def pop(self, key: _KT) -> _VT | None: ...
     @overload
     def pop(self, key: _KT, default: _VT | _T) -> _VT | _T: ...
     def popitem(self, least_recent: bool = ...) -> tuple[_KT, _VT]: ...
     @overload
     def setdefault(self: LRU[_KT, _T | None], key: _KT) -> _T | None: ...
     @overload
     def setdefault(self, key: _KT, default: _VT) -> _VT: ...
```

### Comparing `tarina-0.2.2/src/tarina/_lru_py.py` & `tarina-0.2.3/src/tarina/_lru_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,27 @@
         self.__cache = OrderedDict()
         self.__size = 0
         self.__callback = callback
 
     def clear(self) -> None:
         self.__cache.clear()
 
-    def get(self, key: _KT, default: _VT | _T) -> _VT | _T:
+    @overload
+    def get(self, key: _KT) -> _VT | None:
+        ...
+
+    @overload
+    def get(self, key: _KT, instead: _VT | _T) -> _VT | _T:
+        ...
+
+    def get(self, key: _KT, instead: _VT | _T | None = None):
         if key in self.__cache:
             self.__cache.move_to_end(key, last=False)
             return self.__cache[key]
-        return default
+        return instead
 
     def get_size(self) -> int:
         return self.__max
 
     def has_key(self, key: _KT) -> bool:
         return key in self.__cache
 
@@ -55,15 +63,15 @@
     def peek_first_item(self) -> tuple[_KT, _VT] | None:
         return self.items()[0] if self.__cache else None
 
     def peek_last_item(self) -> tuple[_KT, _VT] | None:
         return self.items()[-1] if self.__cache else None
 
     @overload
-    def pop(self, key: _KT) -> _VT:
+    def pop(self, key: _KT) -> _VT | None:
         ...
 
     @overload
     def pop(self, key: _KT, default: _VT | _T) -> _VT | _T:
         ...
 
     def pop(self, key: _KT, default: _VT | _T | None = None):
```

### Comparing `tarina-0.2.2/src/tarina/_op.h` & `tarina-0.2.3/src/tarina/_op.h`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/_string_c.c` & `tarina-0.2.3/src/tarina/_string_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -1087,32 +1087,14 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
-/* GetItemIntUnicode.proto */
-#define __Pyx_GetItemInt_Unicode(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Unicode_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "string index out of range"), (Py_UCS4)-1))
-static CYTHON_INLINE Py_UCS4 __Pyx_GetItemInt_Unicode_Fast(PyObject* ustring, Py_ssize_t i,
-                                                           int wraparound, int boundscheck);
-
-/* SetItemInt.proto */
-#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
-               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
-                                               int is_list, int wraparound, int boundscheck);
-
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1254,22 +1236,22 @@
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
@@ -1377,15 +1359,15 @@
 static __Pyx_CachedCFunction __pyx_umethod_PyUnicode_Type_lstrip = {0, &__pyx_n_s_lstrip, 0, 0, 0};
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
 /* Late includes */
 
-/* "tarina/_string_c.pyx":13
+/* "tarina/_string_c.pyx":16
  *     bint set_contains_key(object anyset, object key) except -1
  * 
  * cdef inline int contains(tuple chs, Py_UCS4 ch):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = Py_SIZE(chs)
  */
 
@@ -1398,97 +1380,97 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("contains", 0);
 
-  /* "tarina/_string_c.pyx":14
+  /* "tarina/_string_c.pyx":17
  * 
  * cdef inline int contains(tuple chs, Py_UCS4 ch):
  *     cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:
  */
   __pyx_v_i = 0;
 
-  /* "tarina/_string_c.pyx":15
+  /* "tarina/_string_c.pyx":18
  * cdef inline int contains(tuple chs, Py_UCS4 ch):
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = Py_SIZE(chs)             # <<<<<<<<<<<<<<
  *     while i < length:
  *         if ch == <object>tupleitem(chs, i):
  */
   __pyx_v_length = Py_SIZE(__pyx_v_chs);
 
-  /* "tarina/_string_c.pyx":16
+  /* "tarina/_string_c.pyx":19
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:             # <<<<<<<<<<<<<<
  *         if ch == <object>tupleitem(chs, i):
  *             return 1
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_i < __pyx_v_length) != 0);
     if (!__pyx_t_1) break;
 
-    /* "tarina/_string_c.pyx":17
+    /* "tarina/_string_c.pyx":20
  *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:
  *         if ch == <object>tupleitem(chs, i):             # <<<<<<<<<<<<<<
  *             return 1
  *         i += 1
  */
-    __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+    __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = tupleitem(__pyx_v_chs, __pyx_v_i);
-    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_2, ((PyObject *)__pyx_t_3), Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 17, __pyx_L1_error)
+    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_2, ((PyObject *)__pyx_t_3), Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_1) {
 
-      /* "tarina/_string_c.pyx":18
+      /* "tarina/_string_c.pyx":21
  *     while i < length:
  *         if ch == <object>tupleitem(chs, i):
  *             return 1             # <<<<<<<<<<<<<<
  *         i += 1
  *     return 0
  */
       __pyx_r = 1;
       goto __pyx_L0;
 
-      /* "tarina/_string_c.pyx":17
+      /* "tarina/_string_c.pyx":20
  *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:
  *         if ch == <object>tupleitem(chs, i):             # <<<<<<<<<<<<<<
  *             return 1
  *         i += 1
  */
     }
 
-    /* "tarina/_string_c.pyx":19
+    /* "tarina/_string_c.pyx":22
  *         if ch == <object>tupleitem(chs, i):
  *             return 1
  *         i += 1             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "tarina/_string_c.pyx":20
+  /* "tarina/_string_c.pyx":23
  *             return 1
  *         i += 1
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef set QUOTES = {'"', '\''}
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":13
+  /* "tarina/_string_c.pyx":16
  *     bint set_contains_key(object anyset, object key) except -1
  * 
  * cdef inline int contains(tuple chs, Py_UCS4 ch):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = Py_SIZE(chs)
  */
 
@@ -1498,15 +1480,15 @@
   __Pyx_WriteUnraisable("tarina._string_c.contains", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tarina/_string_c.pyx":25
+/* "tarina/_string_c.pyx":28
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
 
@@ -1545,54 +1527,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separates)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, 1); __PYX_ERR(0, 25, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, 1); __PYX_ERR(0, 28, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_crlf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split") < 0)) __PYX_ERR(0, 25, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split") < 0)) __PYX_ERR(0, 28, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_text = ((PyObject*)values[0]);
     __pyx_v_separates = ((PyObject*)values[1]);
     if (values[2]) {
-      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L3_error)
+      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
     } else {
       __pyx_v_crlf = ((char)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 25, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 28, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tarina._string_c.split", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 25, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 28, __pyx_L1_error)
   __pyx_r = __pyx_pf_6tarina_9_string_c_split(__pyx_self, __pyx_v_text, __pyx_v_separates, __pyx_v_crlf);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -1607,476 +1589,474 @@
   Py_UCS4 __pyx_v_ch;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_length;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  Py_UCS4 __pyx_t_3;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
   int __pyx_t_6;
-  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("split", 0);
 
-  /* "tarina/_string_c.pyx":36
+  /* "tarina/_string_c.pyx":39
  *         List[str]: ,
  *     """
  *     cdef char escape = 0             # <<<<<<<<<<<<<<
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0
  */
   __pyx_v_escape = 0;
 
-  /* "tarina/_string_c.pyx":37
+  /* "tarina/_string_c.pyx":40
  *     """
  *     cdef char escape = 0
  *     cdef list result = []             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":38
+  /* "tarina/_string_c.pyx":41
  *     cdef char escape = 0
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0
  */
   __pyx_v_quotation = 0;
 
-  /* "tarina/_string_c.pyx":39
+  /* "tarina/_string_c.pyx":42
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  */
   __pyx_v_ch = 0;
 
-  /* "tarina/_string_c.pyx":40
+  /* "tarina/_string_c.pyx":43
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  */
   __pyx_v_i = 0;
 
-  /* "tarina/_string_c.pyx":41
+  /* "tarina/_string_c.pyx":44
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)             # <<<<<<<<<<<<<<
  * 
  *     while i < length:
  */
   __pyx_v_length = PyUnicode_GET_LENGTH(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":43
+  /* "tarina/_string_c.pyx":46
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  *     while i < length:             # <<<<<<<<<<<<<<
- *         ch = text[i]
+ *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_i < __pyx_v_length) != 0);
     if (!__pyx_t_2) break;
 
-    /* "tarina/_string_c.pyx":44
+    /* "tarina/_string_c.pyx":47
  * 
  *     while i < length:
- *         ch = text[i]             # <<<<<<<<<<<<<<
+ *         ch = PyUnicode_READ_CHAR(text, i)             # <<<<<<<<<<<<<<
  *         i += 1
  *         if ch == 92:  # \\
  */
-    __pyx_t_3 = __Pyx_GetItemInt_Unicode(__pyx_v_text, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(__pyx_t_3 == (Py_UCS4)-1)) __PYX_ERR(0, 44, __pyx_L1_error)
-    __pyx_v_ch = __pyx_t_3;
+    __pyx_v_ch = PyUnicode_READ_CHAR(__pyx_v_text, __pyx_v_i);
 
-    /* "tarina/_string_c.pyx":45
+    /* "tarina/_string_c.pyx":48
  *     while i < length:
- *         ch = text[i]
+ *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1             # <<<<<<<<<<<<<<
  *         if ch == 92:  # \\
  *             escape = 1
  */
     __pyx_v_i = (__pyx_v_i + 1);
 
-    /* "tarina/_string_c.pyx":46
- *         ch = text[i]
+    /* "tarina/_string_c.pyx":49
+ *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(result, ch)
  */
     __pyx_t_2 = ((__pyx_v_ch == 92) != 0);
     if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":47
+      /* "tarina/_string_c.pyx":50
  *         i += 1
  *         if ch == 92:  # \\
  *             escape = 1             # <<<<<<<<<<<<<<
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):
  */
       __pyx_v_escape = 1;
 
-      /* "tarina/_string_c.pyx":48
+      /* "tarina/_string_c.pyx":51
  *         if ch == 92:  # \\
  *             escape = 1
  *             PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:
  */
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 48, __pyx_L1_error)
+      __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":46
- *         ch = text[i]
+      /* "tarina/_string_c.pyx":49
+ *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(result, ch)
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":49
+    /* "tarina/_string_c.pyx":52
  *             escape = 1
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
     __pyx_t_1 = __pyx_v_6tarina_9_string_c_QUOTES;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_5); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_4); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_6 = (__pyx_t_2 != 0);
-    if (__pyx_t_6) {
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    if (__pyx_t_5) {
 
-      /* "tarina/_string_c.pyx":50
+      /* "tarina/_string_c.pyx":53
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
-      __pyx_t_6 = ((__pyx_v_quotation == 0) != 0);
-      if (__pyx_t_6) {
+      __pyx_t_5 = ((__pyx_v_quotation == 0) != 0);
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":51
+        /* "tarina/_string_c.pyx":54
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:
  *                 quotation = ch             # <<<<<<<<<<<<<<
  *             elif ch == quotation:
  *                 quotation = 0
  */
         __pyx_v_quotation = __pyx_v_ch;
 
-        /* "tarina/_string_c.pyx":50
+        /* "tarina/_string_c.pyx":53
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
         goto __pyx_L6;
       }
 
-      /* "tarina/_string_c.pyx":52
+      /* "tarina/_string_c.pyx":55
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
-      __pyx_t_6 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
-      if (__pyx_t_6) {
+      __pyx_t_5 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":53
+        /* "tarina/_string_c.pyx":56
  *                 quotation = ch
  *             elif ch == quotation:
  *                 quotation = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 PyList_Append(result, ch)
  */
         __pyx_v_quotation = 0;
 
-        /* "tarina/_string_c.pyx":52
+        /* "tarina/_string_c.pyx":55
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "tarina/_string_c.pyx":55
+      /* "tarina/_string_c.pyx":58
  *                 quotation = 0
  *             else:
  *                 PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *                 continue
  *             if escape:
  */
       /*else*/ {
-        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_t_5); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "tarina/_string_c.pyx":56
+        /* "tarina/_string_c.pyx":59
  *             else:
  *                 PyList_Append(result, ch)
  *                 continue             # <<<<<<<<<<<<<<
  *             if escape:
- *                 result[-1] = ch
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  */
         goto __pyx_L3_continue;
       }
       __pyx_L6:;
 
-      /* "tarina/_string_c.pyx":57
+      /* "tarina/_string_c.pyx":60
  *                 PyList_Append(result, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
- *                 result[-1] = ch
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  */
-      __pyx_t_6 = (__pyx_v_escape != 0);
-      if (__pyx_t_6) {
+      __pyx_t_5 = (__pyx_v_escape != 0);
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":58
+        /* "tarina/_string_c.pyx":61
  *                 continue
  *             if escape:
- *                 result[-1] = ch             # <<<<<<<<<<<<<<
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)             # <<<<<<<<<<<<<<
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':
  */
-        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_result, -1L, __pyx_t_5, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        PyList_SET_ITEM(__pyx_v_result, (Py_SIZE(__pyx_v_result) - 1), __pyx_t_4);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "tarina/_string_c.pyx":57
+        /* "tarina/_string_c.pyx":60
  *                 PyList_Append(result, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
- *                 result[-1] = ch
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  */
       }
 
-      /* "tarina/_string_c.pyx":49
+      /* "tarina/_string_c.pyx":52
  *             escape = 1
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":59
+    /* "tarina/_string_c.pyx":62
  *             if escape:
- *                 result[-1] = ch
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):             # <<<<<<<<<<<<<<
  *             if result and result[-1] != '\1':
  *                 PyList_Append(result, '\1')
  */
     __pyx_t_2 = ((__pyx_v_quotation == 0) != 0);
     if (!__pyx_t_2) {
       goto __pyx_L9_next_or;
     } else {
     }
     __pyx_t_2 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
     if (!__pyx_t_2) {
     } else {
-      __pyx_t_6 = __pyx_t_2;
+      __pyx_t_5 = __pyx_t_2;
       goto __pyx_L8_bool_binop_done;
     }
     __pyx_L9_next_or:;
     __pyx_t_2 = (__pyx_v_crlf != 0);
     if (__pyx_t_2) {
     } else {
-      __pyx_t_6 = __pyx_t_2;
+      __pyx_t_5 = __pyx_t_2;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_5 = __pyx_v_6tarina_9_string_c_CRLF;
-    __Pyx_INCREF(__pyx_t_5);
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_4 = __pyx_v_6tarina_9_string_c_CRLF;
+    __Pyx_INCREF(__pyx_t_4);
+    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = set_contains_key(__pyx_t_5, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 59, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_2 = set_contains_key(__pyx_t_4, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = (__pyx_t_2 != 0);
-    __pyx_t_6 = __pyx_t_7;
+    __pyx_t_6 = (__pyx_t_2 != 0);
+    __pyx_t_5 = __pyx_t_6;
     __pyx_L8_bool_binop_done:;
-    if (__pyx_t_6) {
+    if (__pyx_t_5) {
 
-      /* "tarina/_string_c.pyx":60
- *                 result[-1] = ch
+      /* "tarina/_string_c.pyx":63
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':             # <<<<<<<<<<<<<<
  *                 PyList_Append(result, '\1')
  *         else:
  */
-      __pyx_t_7 = (PyList_GET_SIZE(__pyx_v_result) != 0);
-      if (__pyx_t_7) {
+      __pyx_t_6 = (PyList_GET_SIZE(__pyx_v_result) != 0);
+      if (__pyx_t_6) {
       } else {
-        __pyx_t_6 = __pyx_t_7;
+        __pyx_t_5 = __pyx_t_6;
         goto __pyx_L13_bool_binop_done;
       }
-      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_result, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_result, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u_, Py_NE)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u_, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_6 = __pyx_t_7;
+      __pyx_t_5 = __pyx_t_6;
       __pyx_L13_bool_binop_done:;
-      if (__pyx_t_6) {
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":61
+        /* "tarina/_string_c.pyx":64
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':
  *                 PyList_Append(result, '\1')             # <<<<<<<<<<<<<<
  *         else:
  *             PyList_Append(result, ch)
  */
-        __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_kp_u_); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_kp_u_); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 64, __pyx_L1_error)
 
-        /* "tarina/_string_c.pyx":60
- *                 result[-1] = ch
+        /* "tarina/_string_c.pyx":63
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':             # <<<<<<<<<<<<<<
  *                 PyList_Append(result, '\1')
  *         else:
  */
       }
 
-      /* "tarina/_string_c.pyx":59
+      /* "tarina/_string_c.pyx":62
  *             if escape:
- *                 result[-1] = ch
+ *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):             # <<<<<<<<<<<<<<
  *             if result and result[-1] != '\1':
  *                 PyList_Append(result, '\1')
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":63
+    /* "tarina/_string_c.pyx":66
  *                 PyList_Append(result, '\1')
  *         else:
  *             PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:
  */
     /*else*/ {
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":64
+      /* "tarina/_string_c.pyx":67
  *         else:
  *             PyList_Append(result, ch)
  *             escape = 0             # <<<<<<<<<<<<<<
  *     if PyUnicode_GET_LENGTH(result) == 0:
  *         return []
  */
       __pyx_v_escape = 0;
     }
     __pyx_L5:;
     __pyx_L3_continue:;
   }
 
-  /* "tarina/_string_c.pyx":65
+  /* "tarina/_string_c.pyx":68
  *             PyList_Append(result, ch)
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:             # <<<<<<<<<<<<<<
  *         return []
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
  */
-  __pyx_t_6 = ((PyUnicode_GET_LENGTH(__pyx_v_result) == 0) != 0);
-  if (__pyx_t_6) {
+  __pyx_t_5 = ((PyUnicode_GET_LENGTH(__pyx_v_result) == 0) != 0);
+  if (__pyx_t_5) {
 
-    /* "tarina/_string_c.pyx":66
+    /* "tarina/_string_c.pyx":69
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:
  *         return []             # <<<<<<<<<<<<<<
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "tarina/_string_c.pyx":65
+    /* "tarina/_string_c.pyx":68
  *             PyList_Append(result, ch)
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:             # <<<<<<<<<<<<<<
  *         return []
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
  */
   }
 
-  /* "tarina/_string_c.pyx":67
+  /* "tarina/_string_c.pyx":70
  *     if PyUnicode_GET_LENGTH(result) == 0:
  *         return []
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyUnicode_Split(__pyx_t_1, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = PyUnicode_Split(__pyx_t_1, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":25
+  /* "tarina/_string_c.pyx":28
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("tarina._string_c.split", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tarina/_string_c.pyx":70
+/* "tarina/_string_c.pyx":73
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
 
@@ -2114,54 +2094,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separates)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, 1); __PYX_ERR(0, 70, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, 1); __PYX_ERR(0, 73, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_crlf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split_once") < 0)) __PYX_ERR(0, 70, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split_once") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_text = ((PyObject*)values[0]);
     __pyx_v_separates = ((PyObject*)values[1]);
     if (values[2]) {
-      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 70, __pyx_L3_error)
+      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
     } else {
       __pyx_v_crlf = ((char)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 70, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tarina._string_c.split_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 70, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_r = __pyx_pf_6tarina_9_string_c_2split_once(__pyx_self, __pyx_v_text, __pyx_v_separates, __pyx_v_crlf);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2177,482 +2157,480 @@
   char __pyx_v_escape;
   char __pyx_v_sep;
   Py_ssize_t __pyx_v_length;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  Py_UCS4 __pyx_t_3;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
   int __pyx_t_6;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("split_once", 0);
   __Pyx_INCREF(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":71
+  /* "tarina/_string_c.pyx":74
  * 
  * def split_once(str text, tuple separates, char crlf=True):
  *     text = text.lstrip()             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []
  */
-  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lstrip, __pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lstrip, __pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_text, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":72
+  /* "tarina/_string_c.pyx":75
  * def split_once(str text, tuple separates, char crlf=True):
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0             # <<<<<<<<<<<<<<
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0
  */
   __pyx_v_index = 0;
 
-  /* "tarina/_string_c.pyx":73
+  /* "tarina/_string_c.pyx":76
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_out_text = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":74
+  /* "tarina/_string_c.pyx":77
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0
  */
   __pyx_v_quotation = 0;
 
-  /* "tarina/_string_c.pyx":75
+  /* "tarina/_string_c.pyx":78
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0             # <<<<<<<<<<<<<<
  *     cdef char escape = 0
  *     cdef char sep = 0
  */
   __pyx_v_ch = 0;
 
-  /* "tarina/_string_c.pyx":76
+  /* "tarina/_string_c.pyx":79
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0             # <<<<<<<<<<<<<<
  *     cdef char sep = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  */
   __pyx_v_escape = 0;
 
-  /* "tarina/_string_c.pyx":77
+  /* "tarina/_string_c.pyx":80
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0
  *     cdef char sep = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  */
   __pyx_v_sep = 0;
 
-  /* "tarina/_string_c.pyx":78
+  /* "tarina/_string_c.pyx":81
  *     cdef char escape = 0
  *     cdef char sep = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)             # <<<<<<<<<<<<<<
  * 
  *     while index < length:
  */
   __pyx_v_length = PyUnicode_GET_LENGTH(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":80
+  /* "tarina/_string_c.pyx":83
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  *     while index < length:             # <<<<<<<<<<<<<<
- *         ch = text[index]
+ *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_index < __pyx_v_length) != 0);
     if (!__pyx_t_2) break;
 
-    /* "tarina/_string_c.pyx":81
+    /* "tarina/_string_c.pyx":84
  * 
  *     while index < length:
- *         ch = text[index]             # <<<<<<<<<<<<<<
+ *         ch = PyUnicode_READ_CHAR(text, index)             # <<<<<<<<<<<<<<
  *         index += 1
- *         if ch == 92:  # \\
+ *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
  */
-    __pyx_t_3 = __Pyx_GetItemInt_Unicode(__pyx_v_text, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(__pyx_t_3 == (Py_UCS4)-1)) __PYX_ERR(0, 81, __pyx_L1_error)
-    __pyx_v_ch = __pyx_t_3;
+    __pyx_v_ch = PyUnicode_READ_CHAR(__pyx_v_text, __pyx_v_index);
 
-    /* "tarina/_string_c.pyx":82
+    /* "tarina/_string_c.pyx":85
  *     while index < length:
- *         ch = text[index]
+ *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1             # <<<<<<<<<<<<<<
- *         if ch == 92:  # \\
- *             escape = 1
+ *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
+ *             sep = 1
  */
     __pyx_v_index = (__pyx_v_index + 1);
 
-    /* "tarina/_string_c.pyx":83
- *         ch = text[index]
+    /* "tarina/_string_c.pyx":86
+ *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1
+ *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):             # <<<<<<<<<<<<<<
+ *             sep = 1
+ *             continue
+ */
+    __pyx_t_3 = ((__pyx_v_quotation == 0) != 0);
+    if (__pyx_t_3) {
+    } else {
+      __pyx_t_2 = __pyx_t_3;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_3 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
+    if (!__pyx_t_3) {
+    } else {
+      __pyx_t_2 = __pyx_t_3;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_3 = (__pyx_v_crlf != 0);
+    if (__pyx_t_3) {
+    } else {
+      __pyx_t_2 = __pyx_t_3;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_1 = __pyx_v_6tarina_9_string_c_CRLF;
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = set_contains_key(__pyx_t_1, __pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_5 = (__pyx_t_3 != 0);
+    __pyx_t_2 = __pyx_t_5;
+    __pyx_L6_bool_binop_done:;
+    if (__pyx_t_2) {
+
+      /* "tarina/_string_c.pyx":87
+ *         index += 1
+ *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
+ *             sep = 1             # <<<<<<<<<<<<<<
+ *             continue
+ *         if sep == 1:
+ */
+      __pyx_v_sep = 1;
+
+      /* "tarina/_string_c.pyx":88
+ *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
+ *             sep = 1
+ *             continue             # <<<<<<<<<<<<<<
+ *         if sep == 1:
+ *             index -= 1
+ */
+      goto __pyx_L3_continue;
+
+      /* "tarina/_string_c.pyx":86
+ *         ch = PyUnicode_READ_CHAR(text, index)
+ *         index += 1
+ *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):             # <<<<<<<<<<<<<<
+ *             sep = 1
+ *             continue
+ */
+    }
+
+    /* "tarina/_string_c.pyx":89
+ *             sep = 1
+ *             continue
+ *         if sep == 1:             # <<<<<<<<<<<<<<
+ *             index -= 1
+ *             break
+ */
+    __pyx_t_2 = ((__pyx_v_sep == 1) != 0);
+    if (__pyx_t_2) {
+
+      /* "tarina/_string_c.pyx":90
+ *             continue
+ *         if sep == 1:
+ *             index -= 1             # <<<<<<<<<<<<<<
+ *             break
+ *         if ch == 92:  # \\
+ */
+      __pyx_v_index = (__pyx_v_index - 1);
+
+      /* "tarina/_string_c.pyx":91
+ *         if sep == 1:
+ *             index -= 1
+ *             break             # <<<<<<<<<<<<<<
+ *         if ch == 92:  # \\
+ *             escape = 1
+ */
+      goto __pyx_L4_break;
+
+      /* "tarina/_string_c.pyx":89
+ *             sep = 1
+ *             continue
+ *         if sep == 1:             # <<<<<<<<<<<<<<
+ *             index -= 1
+ *             break
+ */
+    }
+
+    /* "tarina/_string_c.pyx":92
+ *             index -= 1
+ *             break
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(out_text, ch)
  */
     __pyx_t_2 = ((__pyx_v_ch == 92) != 0);
     if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":84
- *         index += 1
+      /* "tarina/_string_c.pyx":93
+ *             break
  *         if ch == 92:  # \\
  *             escape = 1             # <<<<<<<<<<<<<<
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #
  */
       __pyx_v_escape = 1;
 
-      /* "tarina/_string_c.pyx":85
+      /* "tarina/_string_c.pyx":94
  *         if ch == 92:  # \\
  *             escape = 1
  *             PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:
  */
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 85, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_4); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 94, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "tarina/_string_c.pyx":83
- *         ch = text[index]
- *         index += 1
+      /* "tarina/_string_c.pyx":92
+ *             index -= 1
+ *             break
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(out_text, ch)
  */
-      goto __pyx_L5;
+      goto __pyx_L11;
     }
 
-    /* "tarina/_string_c.pyx":86
+    /* "tarina/_string_c.pyx":95
  *             escape = 1
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
-    __pyx_t_1 = __pyx_v_6tarina_9_string_c_QUOTES;
-    __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_5); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_4 = __pyx_v_6tarina_9_string_c_QUOTES;
+    __Pyx_INCREF(__pyx_t_4);
+    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = set_contains_key(__pyx_t_4, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_6 = (__pyx_t_2 != 0);
-    if (__pyx_t_6) {
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    if (__pyx_t_5) {
 
-      /* "tarina/_string_c.pyx":87
+      /* "tarina/_string_c.pyx":96
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
-      __pyx_t_6 = ((__pyx_v_quotation == 0) != 0);
-      if (__pyx_t_6) {
+      __pyx_t_5 = ((__pyx_v_quotation == 0) != 0);
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":88
+        /* "tarina/_string_c.pyx":97
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:
  *                 quotation = ch             # <<<<<<<<<<<<<<
  *             elif ch == quotation:
  *                 quotation = 0
  */
         __pyx_v_quotation = __pyx_v_ch;
 
-        /* "tarina/_string_c.pyx":87
+        /* "tarina/_string_c.pyx":96
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
-        goto __pyx_L6;
+        goto __pyx_L12;
       }
 
-      /* "tarina/_string_c.pyx":89
+      /* "tarina/_string_c.pyx":98
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
-      __pyx_t_6 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
-      if (__pyx_t_6) {
+      __pyx_t_5 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":90
+        /* "tarina/_string_c.pyx":99
  *                 quotation = ch
  *             elif ch == quotation:
  *                 quotation = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 PyList_Append(out_text, ch)
  */
         __pyx_v_quotation = 0;
 
-        /* "tarina/_string_c.pyx":89
+        /* "tarina/_string_c.pyx":98
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
-        goto __pyx_L6;
+        goto __pyx_L12;
       }
 
-      /* "tarina/_string_c.pyx":92
+      /* "tarina/_string_c.pyx":101
  *                 quotation = 0
  *             else:
  *                 PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
  *                 continue
  *             if escape:
  */
       /*else*/ {
-        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_4 = PyList_Append(__pyx_v_out_text, __pyx_t_5); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 92, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 101, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "tarina/_string_c.pyx":93
+        /* "tarina/_string_c.pyx":102
  *             else:
  *                 PyList_Append(out_text, ch)
  *                 continue             # <<<<<<<<<<<<<<
  *             if escape:
- *                 out_text[-1] = ch
+ *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
  */
         goto __pyx_L3_continue;
       }
-      __pyx_L6:;
+      __pyx_L12:;
 
-      /* "tarina/_string_c.pyx":94
+      /* "tarina/_string_c.pyx":103
  *                 PyList_Append(out_text, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
- *                 out_text[-1] = ch
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+ *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
+ *         else:
  */
-      __pyx_t_6 = (__pyx_v_escape != 0);
-      if (__pyx_t_6) {
+      __pyx_t_5 = (__pyx_v_escape != 0);
+      if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":95
+        /* "tarina/_string_c.pyx":104
  *                 continue
  *             if escape:
- *                 out_text[-1] = ch             # <<<<<<<<<<<<<<
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
- *             sep = 1
+ *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)             # <<<<<<<<<<<<<<
+ *         else:
+ *             PyList_Append(out_text, ch)
  */
-        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_out_text, -1L, __pyx_t_5, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        PyList_SET_ITEM(__pyx_v_out_text, (Py_SIZE(__pyx_v_out_text) - 1), __pyx_t_1);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "tarina/_string_c.pyx":94
+        /* "tarina/_string_c.pyx":103
  *                 PyList_Append(out_text, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
- *                 out_text[-1] = ch
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+ *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
+ *         else:
  */
       }
 
-      /* "tarina/_string_c.pyx":86
+      /* "tarina/_string_c.pyx":95
  *             escape = 1
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
-      goto __pyx_L5;
-    }
-
-    /* "tarina/_string_c.pyx":96
- *             if escape:
- *                 out_text[-1] = ch
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:             # <<<<<<<<<<<<<<
- *             sep = 1
- *             continue
- */
-    __pyx_t_2 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
-    if (!__pyx_t_2) {
-    } else {
-      goto __pyx_L9_next_and;
-    }
-    __pyx_t_2 = (__pyx_v_crlf != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_6 = __pyx_t_2;
-      goto __pyx_L8_bool_binop_done;
-    }
-    __pyx_t_5 = __pyx_v_6tarina_9_string_c_CRLF;
-    __Pyx_INCREF(__pyx_t_5);
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = set_contains_key(__pyx_t_5, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = (__pyx_t_2 != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L8_bool_binop_done;
-    }
-    __pyx_L9_next_and:;
-    __pyx_t_7 = ((__pyx_v_quotation == 0) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L8_bool_binop_done:;
-    if (__pyx_t_6) {
-
-      /* "tarina/_string_c.pyx":97
- *                 out_text[-1] = ch
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
- *             sep = 1             # <<<<<<<<<<<<<<
- *             continue
- *         else:
- */
-      __pyx_v_sep = 1;
-
-      /* "tarina/_string_c.pyx":98
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
- *             sep = 1
- *             continue             # <<<<<<<<<<<<<<
- *         else:
- *             if sep == 1:
- */
-      goto __pyx_L3_continue;
-
-      /* "tarina/_string_c.pyx":96
- *             if escape:
- *                 out_text[-1] = ch
- *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:             # <<<<<<<<<<<<<<
- *             sep = 1
- *             continue
- */
+      goto __pyx_L11;
     }
 
-    /* "tarina/_string_c.pyx":100
- *             continue
- *         else:
- *             if sep == 1:             # <<<<<<<<<<<<<<
- *                 index -= 1
- *                 break
- */
-    /*else*/ {
-      __pyx_t_6 = ((__pyx_v_sep == 1) != 0);
-      if (__pyx_t_6) {
-
-        /* "tarina/_string_c.pyx":101
- *         else:
- *             if sep == 1:
- *                 index -= 1             # <<<<<<<<<<<<<<
- *                 break
- *             PyList_Append(out_text, ch)
- */
-        __pyx_v_index = (__pyx_v_index - 1);
-
-        /* "tarina/_string_c.pyx":102
- *             if sep == 1:
- *                 index -= 1
- *                 break             # <<<<<<<<<<<<<<
- *             PyList_Append(out_text, ch)
- *             escape = 0
- */
-        goto __pyx_L4_break;
-
-        /* "tarina/_string_c.pyx":100
- *             continue
+    /* "tarina/_string_c.pyx":106
+ *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
  *         else:
- *             if sep == 1:             # <<<<<<<<<<<<<<
- *                 index -= 1
- *                 break
- */
-      }
-
-      /* "tarina/_string_c.pyx":103
- *                 index -= 1
- *                 break
  *             PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
  *             escape = 0
  *     return PyUnicode_Join('', out_text), text[index:]
  */
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+    /*else*/ {
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 103, __pyx_L1_error)
+      __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":104
- *                 break
+      /* "tarina/_string_c.pyx":107
+ *         else:
  *             PyList_Append(out_text, ch)
  *             escape = 0             # <<<<<<<<<<<<<<
  *     return PyUnicode_Join('', out_text), text[index:]
  */
       __pyx_v_escape = 0;
     }
-    __pyx_L5:;
+    __pyx_L11:;
     __pyx_L3_continue:;
   }
   __pyx_L4_break:;
 
-  /* "tarina/_string_c.pyx":105
+  /* "tarina/_string_c.pyx":108
  *             PyList_Append(out_text, ch)
  *             escape = 0
  *     return PyUnicode_Join('', out_text), text[index:]             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_out_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_out_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_v_text == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 105, __pyx_L1_error)
+    __PYX_ERR(0, 108, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_PyUnicode_Substring(__pyx_v_text, __pyx_v_index, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyUnicode_Substring(__pyx_v_text, __pyx_v_index, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_4);
   __pyx_t_1 = 0;
-  __pyx_t_5 = 0;
-  __pyx_r = __pyx_t_8;
-  __pyx_t_8 = 0;
+  __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_7;
+  __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":70
+  /* "tarina/_string_c.pyx":73
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("tarina._string_c.split_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_out_text);
   __Pyx_XDECREF(__pyx_v_text);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -2738,37 +2716,37 @@
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "tarina/_string_c.pyx":25
+  /* "tarina/_string_c.pyx":28
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_escape, __pyx_n_s_result, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_i, __pyx_n_s_length); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_escape, __pyx_n_s_result, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_i, __pyx_n_s_length); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 28, __pyx_L1_error)
 
-  /* "tarina/_string_c.pyx":70
+  /* "tarina/_string_c.pyx":73
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
-  __pyx_tuple__9 = PyTuple_Pack(10, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_index, __pyx_n_s_out_text, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_escape, __pyx_n_s_sep, __pyx_n_s_length); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(10, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_index, __pyx_n_s_out_text, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_escape, __pyx_n_s_sep, __pyx_n_s_length); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split_once, 70, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split_once, 73, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3061,68 +3039,68 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "tarina/_string_c.pyx":22
+  /* "tarina/_string_c.pyx":25
  *     return 0
  * 
  * cdef set QUOTES = {'"', '\''}             # <<<<<<<<<<<<<<
  * cdef set CRLF = {'\r', '\n'}
  * 
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__4) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__4) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_XGOTREF(__pyx_v_6tarina_9_string_c_QUOTES);
   __Pyx_DECREF_SET(__pyx_v_6tarina_9_string_c_QUOTES, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":23
+  /* "tarina/_string_c.pyx":26
  * 
  * cdef set QUOTES = {'"', '\''}
  * cdef set CRLF = {'\r', '\n'}             # <<<<<<<<<<<<<<
  * 
  * def split(str text, tuple separates, char crlf=True):
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__5) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__6) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__6) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_XGOTREF(__pyx_v_6tarina_9_string_c_CRLF);
   __Pyx_DECREF_SET(__pyx_v_6tarina_9_string_c_CRLF, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":25
+  /* "tarina/_string_c.pyx":28
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_1split, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_1split, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split, __pyx_t_1) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":70
+  /* "tarina/_string_c.pyx":73
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_3split_once, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_3split_once, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split_once, __pyx_t_1) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split_once, __pyx_t_1) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "tarina/_string_c.pyx":1
  * # cython: boundscheck=False             # <<<<<<<<<<<<<<
  * # cython: cdivision=True
  * # cython: initializedcheck=False
  */
@@ -3545,82 +3523,14 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
-/* GetItemIntUnicode */
-static CYTHON_INLINE Py_UCS4 __Pyx_GetItemInt_Unicode_Fast(PyObject* ustring, Py_ssize_t i,
-                                                           int wraparound, int boundscheck) {
-    Py_ssize_t length;
-    if (unlikely(__Pyx_PyUnicode_READY(ustring) < 0)) return (Py_UCS4)-1;
-    if (wraparound | boundscheck) {
-        length = __Pyx_PyUnicode_GET_LENGTH(ustring);
-        if (wraparound & unlikely(i < 0)) i += length;
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(i, length))) {
-            return __Pyx_PyUnicode_READ_CHAR(ustring, i);
-        } else {
-            PyErr_SetString(PyExc_IndexError, "string index out of range");
-            return (Py_UCS4)-1;
-        }
-    } else {
-        return __Pyx_PyUnicode_READ_CHAR(ustring, i);
-    }
-}
-
-/* SetItemInt */
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
-    int r;
-    if (!j) return -1;
-    r = PyObject_SetItem(o, j, v);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
-                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
-            PyObject* old = PyList_GET_ITEM(o, n);
-            Py_INCREF(v);
-            PyList_SET_ITEM(o, n, v);
-            Py_DECREF(old);
-            return 1;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_ass_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return -1;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_ass_item(o, i, v);
-        }
-    }
-#else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
-    {
-        return PySequence_SetItem(o, i, v);
-    }
-#endif
-    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
-}
-
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -4351,123 +4261,123 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
+        if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(long) <= sizeof(long)) {
+        if (sizeof(int) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
+        return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(char) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(char) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(char) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(char),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(char) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(char) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(char) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(char),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `tarina-0.2.2/src/tarina/_string_c.pyi` & `tarina-0.2.3/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/_string_c.pyx` & `tarina-0.2.3/src/tarina/_string_c.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # cython: boundscheck=False
 # cython: cdivision=True
 # cython: initializedcheck=False
 
 from cpython.object cimport PyObject, Py_SIZE
 from cpython.unicode cimport PyUnicode_Join, PyUnicode_Split, PyUnicode_GET_LENGTH
-from cpython.list cimport PyList_Append
+from cpython.list cimport PyList_Append, PyList_SET_ITEM
+
+cdef extern from "Python.h":
+    Py_UCS4 PyUnicode_READ_CHAR(object s, Py_ssize_t i)
 
 cdef extern from "_op.h":
     PyObject* tupleitem(object a, Py_ssize_t i)
     bint set_contains_key(object anyset, object key) except -1
 
 cdef inline int contains(tuple chs, Py_UCS4 ch):
     cdef Py_ssize_t i = 0
@@ -37,29 +40,29 @@
     cdef list result = []
     cdef Py_UCS4 quotation = 0
     cdef Py_UCS4 ch = 0
     cdef Py_ssize_t i = 0
     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
 
     while i < length:
-        ch = text[i]
+        ch = PyUnicode_READ_CHAR(text, i)
         i += 1
         if ch == 92:  # \\
             escape = 1
             PyList_Append(result, ch)
         elif set_contains_key(QUOTES, ch):
             if quotation == 0:
                 quotation = ch
             elif ch == quotation:
                 quotation = 0
             else:
                 PyList_Append(result, ch)
                 continue
             if escape:
-                result[-1] = ch
+                PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
             if result and result[-1] != '\1':
                 PyList_Append(result, '\1')
         else:
             PyList_Append(result, ch)
             escape = 0
     if PyUnicode_GET_LENGTH(result) == 0:
@@ -74,32 +77,32 @@
     cdef Py_UCS4 quotation = 0
     cdef Py_UCS4 ch = 0
     cdef char escape = 0
     cdef char sep = 0
     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
 
     while index < length:
-        ch = text[index]
+        ch = PyUnicode_READ_CHAR(text, index)
         index += 1
+        if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
+            sep = 1
+            continue
+        if sep == 1:
+            index -= 1
+            break
         if ch == 92:  # \\
             escape = 1
             PyList_Append(out_text, ch)
         elif set_contains_key(QUOTES, ch):  # 遇到引号括起来的部分跳过分隔
             if quotation == 0:
                 quotation = ch
             elif ch == quotation:
                 quotation = 0
             else:
                 PyList_Append(out_text, ch)
                 continue
             if escape:
-                out_text[-1] = ch
-        elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
-            sep = 1
-            continue
+                PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
         else:
-            if sep == 1:
-                index -= 1
-                break
             PyList_Append(out_text, ch)
             escape = 0
     return PyUnicode_Join('', out_text), text[index:]
```

### Comparing `tarina-0.2.2/src/tarina/_string_py.py` & `tarina-0.2.3/src/tarina/_string_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,34 +14,34 @@
     Returns:
         Tuple[str, str]: 切割后的字符串, 可能含有空格
     """
     index, out_text, quotation, escape, sep = 0, "", "", False, False
     text = text.lstrip()
     for char in text:
         index += 1
+        if (char in separates or (crlf and char in CRLF)) and not quotation:
+            sep = True
+            continue
+        if sep:
+            index -= 1
+            break
         if char == "\\":
             escape = True
             out_text += char
         elif char in QUOTATION:  # 遇到引号括起来的部分跳过分隔
             if not quotation:
                 quotation = char
             elif char == quotation:
                 quotation = ""
             else:
                 out_text += char
                 continue
             if escape:
                 out_text = out_text[:-1] + char
-        elif (char in separates or (crlf and char in CRLF)) and not quotation:
-            sep = True
-            continue
         else:
-            if sep:
-                index -= 1
-                break
             out_text += char
             escape = False
     return out_text, text[index:]
 
 
 def split(text: str, separates: tuple[str, ...], crlf: bool = True):
     """尊重引号与转义的字符串切分
```

### Comparing `tarina-0.2.2/src/tarina/context.py` & `tarina-0.2.3/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/generic.py` & `tarina-0.2.3/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/guard.py` & `tarina-0.2.3/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/lru.pyi` & `tarina-0.2.3/src/tarina/lru.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 
 class LRU(Generic[_KT, _VT]):
 
     def __init__(
         self, size: int, callback: Callable[[_KT, _VT], Any] | None = ...
     ) -> None: ...
     def clear(self) -> None: ...
-    def get(self, key: _KT, default: _VT | _T) -> _VT | _T: ...
+
+    @overload
+    def get(self, key: _KT) -> _VT: ...
+
+    @overload
+    def get(self, key: _KT, instead: _VT | _T) -> _VT | _T: ...
 
     def get_size(self) -> int: ...
     def has_key(self, key: _KT) -> bool: ...
     def keys(self) -> list[_KT]: ...
     def values(self) -> list[_VT]: ...
     def items(self) -> list[tuple[_KT, _VT]]: ...
     def peek_first_item(self) -> tuple[_KT, _VT] | None: ...
```

### Comparing `tarina-0.2.2/src/tarina/signature.py` & `tarina-0.2.3/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/string.py` & `tarina-0.2.3/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina/tools.py` & `tarina-0.2.3/src/tarina/tools.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.2/src/tarina.egg-info/PKG-INFO` & `tarina-0.2.3/src/tarina.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.2.2/src/tarina.egg-info/SOURCES.txt` & `tarina-0.2.3/src/tarina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

