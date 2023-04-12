# Comparing `tmp/tarina-0.2.1.tar.gz` & `tmp/tarina-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.2.1.tar", last modified: Tue Apr 11 12:28:17 2023, max compression
+gzip compressed data, was "tarina-0.2.2.tar", last modified: Wed Apr 12 10:00:04 2023, max compression
```

## Comparing `tarina-0.2.1.tar` & `tarina-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.486463 tarina-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 12:28:01.000000 tarina-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 12:28:01.000000 tarina-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 12:28:17.486463 tarina-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-11 12:28:01.000000 tarina-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 12:28:01.000000 tarina-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:28:17.486463 tarina-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-11 12:28:01.000000 tarina-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.482463 tarina-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.482463 tarina-0.2.1/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (123)   195090 2023-04-11 12:28:08.000000 tarina-0.2.1/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.486463 tarina-0.2.1/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.471043 tarina-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 09:59:44.000000 tarina-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 09:59:44.000000 tarina-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 10:00:04.467043 tarina-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 09:59:44.000000 tarina-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 09:59:44.000000 tarina-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:00:04.471043 tarina-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 09:59:44.000000 tarina-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.463043 tarina-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.467043 tarina-0.2.2/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (123)   204169 2023-04-12 09:59:54.000000 tarina-0.2.2/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-12 09:59:44.000000 tarina-0.2.2/src/tarina/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:00:04.467043 tarina-0.2.2/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 10:00:04.000000 tarina-0.2.2/src/tarina.egg-info/top_level.txt
```

### Comparing `tarina-0.2.1/LICENSE` & `tarina-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/PKG-INFO` & `tarina-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.2.1/pyproject.toml` & `tarina-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tarina"
-version = "0.2.1"
+version = "0.2.2"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
```

### Comparing `tarina-0.2.1/setup.py` & `tarina-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/_lru_c.c` & `tarina-0.2.2/src/tarina/_lru_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/_lru_c.pyi` & `tarina-0.2.2/src/tarina/_lru_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/_lru_py.py` & `tarina-0.2.2/src/tarina/_lru_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,13 +128,14 @@
 
     def __setitem__(self, key: _KT, value: _VT) -> None:
         if key in self.__cache:
             self.__cache.move_to_end(key, last=False)
             self.__cache[key] = value
             return
         self.__cache[key] = value
+        self.__cache.move_to_end(key, last=False)
         self.__size += 1
         if self.__max < self.__size:
             _k, _v = self.__cache.popitem(last=True)
             self.__size -= 1
             if self.__callback:
                 self.__callback(_k, _v)
```

### Comparing `tarina-0.2.1/src/tarina/_string_c.c` & `tarina-0.2.2/src/tarina/_string_c.c`

 * *Files 3% similar despite different names*

```diff
@@ -737,14 +737,17 @@
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__tarina___string_c
 #define __PYX_HAVE_API__tarina___string_c
 /* Early includes */
+#include <string.h>
+#include <stdio.h>
+#include "_op.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -947,14 +950,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "src/tarina/_string_c.pyx",
+  "type.pxd",
 };
 
 /*--- Type declarations ---*/
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
@@ -1015,36 +1019,14 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
@@ -1113,46 +1095,45 @@
 #define __Pyx_GetItemInt_Unicode(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Unicode_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
     (PyErr_SetString(PyExc_IndexError, "string index out of range"), (Py_UCS4)-1))
 static CYTHON_INLINE Py_UCS4 __Pyx_GetItemInt_Unicode_Fast(PyObject* ustring, Py_ssize_t i,
                                                            int wraparound, int boundscheck);
 
-/* ListAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
-        Py_INCREF(x);
-        PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
-#else
-#define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
-#endif
-
 /* SetItemInt.proto */
 #define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
                __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
                                                int is_list, int wraparound, int boundscheck);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
@@ -1193,14 +1174,33 @@
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
 /* PyUnicode_Substring.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Substring(
             PyObject* text, Py_ssize_t start, Py_ssize_t stop);
 
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto
+#define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize {
+   __Pyx_ImportType_CheckSize_Error = 0,
+   __Pyx_ImportType_CheckSize_Warn = 1,
+   __Pyx_ImportType_CheckSize_Ignore = 2
+};
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1256,14 +1256,20 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
@@ -1282,29 +1288,49 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
+/* Module declarations from 'libc.string' */
+
+/* Module declarations from 'libc.stdio' */
+
+/* Module declarations from '__builtin__' */
+
+/* Module declarations from 'cpython.type' */
+static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+
+/* Module declarations from 'cpython' */
+
+/* Module declarations from 'cpython.object' */
+
+/* Module declarations from 'cpython.unicode' */
+
+/* Module declarations from 'cpython.list' */
+
 /* Module declarations from 'tarina._string_c' */
-static CYTHON_INLINE int __pyx_f_6tarina_9_string_c_contains(Py_UCS4, PyObject *); /*proto*/
+static PyObject *__pyx_v_6tarina_9_string_c_QUOTES = 0;
+static PyObject *__pyx_v_6tarina_9_string_c_CRLF = 0;
+static CYTHON_INLINE int __pyx_f_6tarina_9_string_c_contains(PyObject *, Py_UCS4); /*proto*/
 #define __Pyx_MODULE_NAME "tarina._string_c"
 extern int __pyx_module_is_main_tarina___string_c;
 int __pyx_module_is_main_tarina___string_c = 0;
 
 /* Implementation of 'tarina._string_c' */
-static const char __pyx_k_[] = "\"";
+static const char __pyx_k_[] = "\001";
 static const char __pyx_k_i[] = "i";
-static const char __pyx_k__2[] = "'";
-static const char __pyx_k__4[] = "\r";
-static const char __pyx_k__5[] = "\n";
-static const char __pyx_k__7[] = "\000";
-static const char __pyx_k__8[] = "";
+static const char __pyx_k__2[] = "";
+static const char __pyx_k__3[] = "\"";
+static const char __pyx_k__4[] = "'";
+static const char __pyx_k__5[] = "\r";
+static const char __pyx_k__6[] = "\n";
 static const char __pyx_k_ch[] = "ch";
+static const char __pyx_k_sep[] = "sep";
 static const char __pyx_k_crlf[] = "crlf";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_split[] = "split";
@@ -1317,186 +1343,171 @@
 static const char __pyx_k_separates[] = "separates";
 static const char __pyx_k_split_once[] = "split_once";
 static const char __pyx_k_tarina__string_c[] = "tarina._string_c";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_src_tarina__string_c_pyx[] = "src/tarina/_string_c.pyx";
 static PyObject *__pyx_kp_u_;
 static PyObject *__pyx_kp_u__2;
+static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_kp_u__4;
 static PyObject *__pyx_kp_u__5;
-static PyObject *__pyx_kp_u__7;
-static PyObject *__pyx_kp_u__8;
+static PyObject *__pyx_kp_u__6;
 static PyObject *__pyx_n_s_ch;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_crlf;
 static PyObject *__pyx_n_s_escape;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_length;
 static PyObject *__pyx_n_s_lstrip;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_out_text;
 static PyObject *__pyx_n_s_quotation;
 static PyObject *__pyx_n_s_result;
+static PyObject *__pyx_n_s_sep;
 static PyObject *__pyx_n_s_separates;
 static PyObject *__pyx_n_s_split;
 static PyObject *__pyx_n_s_split_once;
 static PyObject *__pyx_kp_s_src_tarina__string_c_pyx;
 static PyObject *__pyx_n_s_tarina__string_c;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_text;
 static PyObject *__pyx_pf_6tarina_9_string_c_split(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_text, PyObject *__pyx_v_separates, char __pyx_v_crlf); /* proto */
 static PyObject *__pyx_pf_6tarina_9_string_c_2split_once(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_text, PyObject *__pyx_v_separates, char __pyx_v_crlf); /* proto */
 static __Pyx_CachedCFunction __pyx_umethod_PyUnicode_Type_lstrip = {0, &__pyx_n_s_lstrip, 0, 0, 0};
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
 /* Late includes */
 
-/* "tarina/_string_c.pyx":5
- * # cython: initializedcheck=False
+/* "tarina/_string_c.pyx":13
+ *     bint set_contains_key(object anyset, object key) except -1
  * 
- * cdef inline int contains(Py_UCS4 ch, tuple chs):             # <<<<<<<<<<<<<<
+ * cdef inline int contains(tuple chs, Py_UCS4 ch):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = len(chs)
+ *     cdef Py_ssize_t length = Py_SIZE(chs)
  */
 
-static CYTHON_INLINE int __pyx_f_6tarina_9_string_c_contains(Py_UCS4 __pyx_v_ch, PyObject *__pyx_v_chs) {
+static CYTHON_INLINE int __pyx_f_6tarina_9_string_c_contains(PyObject *__pyx_v_chs, Py_UCS4 __pyx_v_ch) {
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_length;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("contains", 0);
 
-  /* "tarina/_string_c.pyx":6
+  /* "tarina/_string_c.pyx":14
  * 
- * cdef inline int contains(Py_UCS4 ch, tuple chs):
+ * cdef inline int contains(tuple chs, Py_UCS4 ch):
  *     cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = len(chs)
+ *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:
  */
   __pyx_v_i = 0;
 
-  /* "tarina/_string_c.pyx":7
- * cdef inline int contains(Py_UCS4 ch, tuple chs):
+  /* "tarina/_string_c.pyx":15
+ * cdef inline int contains(tuple chs, Py_UCS4 ch):
  *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = len(chs)             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = Py_SIZE(chs)             # <<<<<<<<<<<<<<
  *     while i < length:
- *         if ch == chs[i]:
+ *         if ch == <object>tupleitem(chs, i):
  */
-  if (unlikely(__pyx_v_chs == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 7, __pyx_L1_error)
-  }
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_chs); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 7, __pyx_L1_error)
-  __pyx_v_length = __pyx_t_1;
+  __pyx_v_length = Py_SIZE(__pyx_v_chs);
 
-  /* "tarina/_string_c.pyx":8
+  /* "tarina/_string_c.pyx":16
  *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = len(chs)
+ *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:             # <<<<<<<<<<<<<<
- *         if ch == chs[i]:
+ *         if ch == <object>tupleitem(chs, i):
  *             return 1
  */
   while (1) {
-    __pyx_t_2 = ((__pyx_v_i < __pyx_v_length) != 0);
-    if (!__pyx_t_2) break;
+    __pyx_t_1 = ((__pyx_v_i < __pyx_v_length) != 0);
+    if (!__pyx_t_1) break;
 
-    /* "tarina/_string_c.pyx":9
- *     cdef Py_ssize_t length = len(chs)
+    /* "tarina/_string_c.pyx":17
+ *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:
- *         if ch == chs[i]:             # <<<<<<<<<<<<<<
+ *         if ch == <object>tupleitem(chs, i):             # <<<<<<<<<<<<<<
  *             return 1
  *         i += 1
  */
-    __pyx_t_3 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(__pyx_v_chs == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 9, __pyx_L1_error)
-    }
-    __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_chs, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_t_4, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 9, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (__pyx_t_2) {
+    __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = tupleitem(__pyx_v_chs, __pyx_v_i);
+    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_2, ((PyObject *)__pyx_t_3), Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 17, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (__pyx_t_1) {
 
-      /* "tarina/_string_c.pyx":10
+      /* "tarina/_string_c.pyx":18
  *     while i < length:
- *         if ch == chs[i]:
+ *         if ch == <object>tupleitem(chs, i):
  *             return 1             # <<<<<<<<<<<<<<
  *         i += 1
  *     return 0
  */
       __pyx_r = 1;
       goto __pyx_L0;
 
-      /* "tarina/_string_c.pyx":9
- *     cdef Py_ssize_t length = len(chs)
+      /* "tarina/_string_c.pyx":17
+ *     cdef Py_ssize_t length = Py_SIZE(chs)
  *     while i < length:
- *         if ch == chs[i]:             # <<<<<<<<<<<<<<
+ *         if ch == <object>tupleitem(chs, i):             # <<<<<<<<<<<<<<
  *             return 1
  *         i += 1
  */
     }
 
-    /* "tarina/_string_c.pyx":11
- *         if ch == chs[i]:
+    /* "tarina/_string_c.pyx":19
+ *         if ch == <object>tupleitem(chs, i):
  *             return 1
  *         i += 1             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "tarina/_string_c.pyx":12
+  /* "tarina/_string_c.pyx":20
  *             return 1
  *         i += 1
  *     return 0             # <<<<<<<<<<<<<<
  * 
- * 
+ * cdef set QUOTES = {'"', '\''}
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":5
- * # cython: initializedcheck=False
+  /* "tarina/_string_c.pyx":13
+ *     bint set_contains_key(object anyset, object key) except -1
  * 
- * cdef inline int contains(Py_UCS4 ch, tuple chs):             # <<<<<<<<<<<<<<
+ * cdef inline int contains(tuple chs, Py_UCS4 ch):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = len(chs)
+ *     cdef Py_ssize_t length = Py_SIZE(chs)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_WriteUnraisable("tarina._string_c.contains", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tarina/_string_c.pyx":15
- * 
+/* "tarina/_string_c.pyx":25
+ * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
 
 /* Python wrapper */
@@ -1534,54 +1545,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separates)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, 1); __PYX_ERR(0, 15, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, 1); __PYX_ERR(0, 25, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_crlf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split") < 0)) __PYX_ERR(0, 15, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split") < 0)) __PYX_ERR(0, 25, __pyx_L3_error)
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
-      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L3_error)
+      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L3_error)
     } else {
       __pyx_v_crlf = ((char)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 15, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 25, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tarina._string_c.split", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 15, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 25, __pyx_L1_error)
   __pyx_r = __pyx_pf_6tarina_9_string_c_split(__pyx_self, __pyx_v_text, __pyx_v_separates, __pyx_v_crlf);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -1595,458 +1606,477 @@
   Py_UCS4 __pyx_v_quotation;
   Py_UCS4 __pyx_v_ch;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_length;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  int __pyx_t_3;
-  Py_UCS4 __pyx_t_4;
-  int __pyx_t_5;
+  int __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("split", 0);
 
-  /* "tarina/_string_c.pyx":26
+  /* "tarina/_string_c.pyx":36
  *         List[str]: ,
  *     """
  *     cdef char escape = 0             # <<<<<<<<<<<<<<
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0
  */
   __pyx_v_escape = 0;
 
-  /* "tarina/_string_c.pyx":27
+  /* "tarina/_string_c.pyx":37
  *     """
  *     cdef char escape = 0
  *     cdef list result = []             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":28
+  /* "tarina/_string_c.pyx":38
  *     cdef char escape = 0
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0
  */
   __pyx_v_quotation = 0;
 
-  /* "tarina/_string_c.pyx":29
+  /* "tarina/_string_c.pyx":39
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = len(text)
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  */
   __pyx_v_ch = 0;
 
-  /* "tarina/_string_c.pyx":30
+  /* "tarina/_string_c.pyx":40
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = len(text)
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  */
   __pyx_v_i = 0;
 
-  /* "tarina/_string_c.pyx":31
+  /* "tarina/_string_c.pyx":41
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = len(text)             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)             # <<<<<<<<<<<<<<
  * 
  *     while i < length:
  */
-  if (unlikely(__pyx_v_text == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 31, __pyx_L1_error)
-  }
-  __pyx_t_2 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_text); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_v_length = __pyx_t_2;
+  __pyx_v_length = PyUnicode_GET_LENGTH(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":33
- *     cdef Py_ssize_t length = len(text)
+  /* "tarina/_string_c.pyx":43
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  *     while i < length:             # <<<<<<<<<<<<<<
  *         ch = text[i]
  *         i += 1
  */
   while (1) {
-    __pyx_t_3 = ((__pyx_v_i < __pyx_v_length) != 0);
-    if (!__pyx_t_3) break;
+    __pyx_t_2 = ((__pyx_v_i < __pyx_v_length) != 0);
+    if (!__pyx_t_2) break;
 
-    /* "tarina/_string_c.pyx":34
+    /* "tarina/_string_c.pyx":44
  * 
  *     while i < length:
  *         ch = text[i]             # <<<<<<<<<<<<<<
  *         i += 1
  *         if ch == 92:  # \\
  */
-    __pyx_t_4 = __Pyx_GetItemInt_Unicode(__pyx_v_text, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(__pyx_t_4 == (Py_UCS4)-1)) __PYX_ERR(0, 34, __pyx_L1_error)
-    __pyx_v_ch = __pyx_t_4;
+    __pyx_t_3 = __Pyx_GetItemInt_Unicode(__pyx_v_text, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(__pyx_t_3 == (Py_UCS4)-1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_v_ch = __pyx_t_3;
 
-    /* "tarina/_string_c.pyx":35
+    /* "tarina/_string_c.pyx":45
  *     while i < length:
  *         ch = text[i]
  *         i += 1             # <<<<<<<<<<<<<<
  *         if ch == 92:  # \\
  *             escape = 1
  */
     __pyx_v_i = (__pyx_v_i + 1);
 
-    /* "tarina/_string_c.pyx":36
+    /* "tarina/_string_c.pyx":46
  *         ch = text[i]
  *         i += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
- *             result.append(ch)
+ *             PyList_Append(result, ch)
  */
-    __pyx_t_3 = ((__pyx_v_ch == 92) != 0);
-    if (__pyx_t_3) {
+    __pyx_t_2 = ((__pyx_v_ch == 92) != 0);
+    if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":37
+      /* "tarina/_string_c.pyx":47
  *         i += 1
  *         if ch == 92:  # \\
  *             escape = 1             # <<<<<<<<<<<<<<
- *             result.append(ch)
- *         elif contains(ch, ('"', "'")):
+ *             PyList_Append(result, ch)
+ *         elif set_contains_key(QUOTES, ch):
  */
       __pyx_v_escape = 1;
 
-      /* "tarina/_string_c.pyx":38
+      /* "tarina/_string_c.pyx":48
  *         if ch == 92:  # \\
  *             escape = 1
- *             result.append(ch)             # <<<<<<<<<<<<<<
- *         elif contains(ch, ('"', "'")):
+ *             PyList_Append(result, ch)             # <<<<<<<<<<<<<<
+ *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:
  */
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 38, __pyx_L1_error)
+      __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":36
+      /* "tarina/_string_c.pyx":46
  *         ch = text[i]
  *         i += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
- *             result.append(ch)
+ *             PyList_Append(result, ch)
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":39
+    /* "tarina/_string_c.pyx":49
  *             escape = 1
- *             result.append(ch)
- *         elif contains(ch, ('"', "'")):             # <<<<<<<<<<<<<<
+ *             PyList_Append(result, ch)
+ *         elif set_contains_key(QUOTES, ch):             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
-    __pyx_t_3 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_ch, __pyx_tuple__3) != 0);
-    if (__pyx_t_3) {
-
-      /* "tarina/_string_c.pyx":40
- *             result.append(ch)
- *         elif contains(ch, ('"', "'")):
+    __pyx_t_1 = __pyx_v_6tarina_9_string_c_QUOTES;
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_5); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 49, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_6 = (__pyx_t_2 != 0);
+    if (__pyx_t_6) {
+
+      /* "tarina/_string_c.pyx":50
+ *             PyList_Append(result, ch)
+ *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
- *                 if escape:
+ *             elif ch == quotation:
  */
-      __pyx_t_3 = ((__pyx_v_quotation == 0) != 0);
-      if (__pyx_t_3) {
+      __pyx_t_6 = ((__pyx_v_quotation == 0) != 0);
+      if (__pyx_t_6) {
 
-        /* "tarina/_string_c.pyx":41
- *         elif contains(ch, ('"', "'")):
+        /* "tarina/_string_c.pyx":51
+ *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:
  *                 quotation = ch             # <<<<<<<<<<<<<<
- *                 if escape:
- *                     result[-1] = ch
- */
-        __pyx_v_quotation = __pyx_v_ch;
-
-        /* "tarina/_string_c.pyx":42
- *             if quotation == 0:
- *                 quotation = ch
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     result[-1] = ch
- *             elif ch == quotation:
- */
-        __pyx_t_3 = (__pyx_v_escape != 0);
-        if (__pyx_t_3) {
-
-          /* "tarina/_string_c.pyx":43
- *                 quotation = ch
- *                 if escape:
- *                     result[-1] = ch             # <<<<<<<<<<<<<<
  *             elif ch == quotation:
  *                 quotation = 0
  */
-          __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (unlikely(__Pyx_SetItemInt(__pyx_v_result, -1L, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 43, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-          /* "tarina/_string_c.pyx":42
- *             if quotation == 0:
- *                 quotation = ch
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     result[-1] = ch
- *             elif ch == quotation:
- */
-        }
+        __pyx_v_quotation = __pyx_v_ch;
 
-        /* "tarina/_string_c.pyx":40
- *             result.append(ch)
- *         elif contains(ch, ('"', "'")):
+        /* "tarina/_string_c.pyx":50
+ *             PyList_Append(result, ch)
+ *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
- *                 if escape:
+ *             elif ch == quotation:
  */
         goto __pyx_L6;
       }
 
-      /* "tarina/_string_c.pyx":44
- *                 if escape:
- *                     result[-1] = ch
+      /* "tarina/_string_c.pyx":52
+ *             if quotation == 0:
+ *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
- *                 if escape:
+ *             else:
  */
-      __pyx_t_3 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
-      if (__pyx_t_3) {
+      __pyx_t_6 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
+      if (__pyx_t_6) {
 
-        /* "tarina/_string_c.pyx":45
- *                     result[-1] = ch
+        /* "tarina/_string_c.pyx":53
+ *                 quotation = ch
  *             elif ch == quotation:
  *                 quotation = 0             # <<<<<<<<<<<<<<
- *                 if escape:
- *                     result[-1] = ch
+ *             else:
+ *                 PyList_Append(result, ch)
  */
         __pyx_v_quotation = 0;
 
-        /* "tarina/_string_c.pyx":46
- *             elif ch == quotation:
+        /* "tarina/_string_c.pyx":52
+ *             if quotation == 0:
+ *                 quotation = ch
+ *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
+ *             else:
  */
-        __pyx_t_3 = (__pyx_v_escape != 0);
-        if (__pyx_t_3) {
-
-          /* "tarina/_string_c.pyx":47
- *                 quotation = 0
- *                 if escape:
- *                     result[-1] = ch             # <<<<<<<<<<<<<<
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
- *             if result and result[-1] != '\0':
- */
-          __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (unlikely(__Pyx_SetItemInt(__pyx_v_result, -1L, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 47, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        goto __pyx_L6;
+      }
 
-          /* "tarina/_string_c.pyx":46
- *             elif ch == quotation:
+      /* "tarina/_string_c.pyx":55
  *                 quotation = 0
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
+ *             else:
+ *                 PyList_Append(result, ch)             # <<<<<<<<<<<<<<
+ *                 continue
+ *             if escape:
+ */
+      /*else*/ {
+        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_t_5); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+        /* "tarina/_string_c.pyx":56
+ *             else:
+ *                 PyList_Append(result, ch)
+ *                 continue             # <<<<<<<<<<<<<<
+ *             if escape:
+ *                 result[-1] = ch
  */
-        }
+        goto __pyx_L3_continue;
+      }
+      __pyx_L6:;
 
-        /* "tarina/_string_c.pyx":44
- *                 if escape:
- *                     result[-1] = ch
- *             elif ch == quotation:             # <<<<<<<<<<<<<<
- *                 quotation = 0
- *                 if escape:
+      /* "tarina/_string_c.pyx":57
+ *                 PyList_Append(result, ch)
+ *                 continue
+ *             if escape:             # <<<<<<<<<<<<<<
+ *                 result[-1] = ch
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
+ */
+      __pyx_t_6 = (__pyx_v_escape != 0);
+      if (__pyx_t_6) {
+
+        /* "tarina/_string_c.pyx":58
+ *                 continue
+ *             if escape:
+ *                 result[-1] = ch             # <<<<<<<<<<<<<<
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
+ *             if result and result[-1] != '\1':
+ */
+        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_result, -1L, __pyx_t_5, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+        /* "tarina/_string_c.pyx":57
+ *                 PyList_Append(result, ch)
+ *                 continue
+ *             if escape:             # <<<<<<<<<<<<<<
+ *                 result[-1] = ch
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  */
       }
-      __pyx_L6:;
 
-      /* "tarina/_string_c.pyx":39
+      /* "tarina/_string_c.pyx":49
  *             escape = 1
- *             result.append(ch)
- *         elif contains(ch, ('"', "'")):             # <<<<<<<<<<<<<<
+ *             PyList_Append(result, ch)
+ *         elif set_contains_key(QUOTES, ch):             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":48
- *                 if escape:
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):             # <<<<<<<<<<<<<<
- *             if result and result[-1] != '\0':
- *                 result.append('\0')
- */
-    __pyx_t_6 = ((__pyx_v_quotation == 0) != 0);
-    if (!__pyx_t_6) {
-      goto __pyx_L10_next_or;
+    /* "tarina/_string_c.pyx":59
+ *             if escape:
+ *                 result[-1] = ch
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):             # <<<<<<<<<<<<<<
+ *             if result and result[-1] != '\1':
+ *                 PyList_Append(result, '\1')
+ */
+    __pyx_t_2 = ((__pyx_v_quotation == 0) != 0);
+    if (!__pyx_t_2) {
+      goto __pyx_L9_next_or;
     } else {
     }
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_v_separates, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 48, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = (__pyx_t_6 != 0);
-    if (!__pyx_t_7) {
+    __pyx_t_2 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
+    if (!__pyx_t_2) {
     } else {
-      __pyx_t_3 = __pyx_t_7;
-      goto __pyx_L9_bool_binop_done;
+      __pyx_t_6 = __pyx_t_2;
+      goto __pyx_L8_bool_binop_done;
     }
-    __pyx_L10_next_or:;
-    __pyx_t_7 = (__pyx_v_crlf != 0);
-    if (__pyx_t_7) {
+    __pyx_L9_next_or:;
+    __pyx_t_2 = (__pyx_v_crlf != 0);
+    if (__pyx_t_2) {
     } else {
-      __pyx_t_3 = __pyx_t_7;
-      goto __pyx_L9_bool_binop_done;
+      __pyx_t_6 = __pyx_t_2;
+      goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_7 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_ch, __pyx_tuple__6) != 0);
-    __pyx_t_3 = __pyx_t_7;
-    __pyx_L9_bool_binop_done:;
-    if (__pyx_t_3) {
-
-      /* "tarina/_string_c.pyx":49
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
- *             if result and result[-1] != '\0':             # <<<<<<<<<<<<<<
- *                 result.append('\0')
+    __pyx_t_5 = __pyx_v_6tarina_9_string_c_CRLF;
+    __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = set_contains_key(__pyx_t_5, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_7 = (__pyx_t_2 != 0);
+    __pyx_t_6 = __pyx_t_7;
+    __pyx_L8_bool_binop_done:;
+    if (__pyx_t_6) {
+
+      /* "tarina/_string_c.pyx":60
+ *                 result[-1] = ch
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
+ *             if result and result[-1] != '\1':             # <<<<<<<<<<<<<<
+ *                 PyList_Append(result, '\1')
  *         else:
  */
       __pyx_t_7 = (PyList_GET_SIZE(__pyx_v_result) != 0);
       if (__pyx_t_7) {
       } else {
-        __pyx_t_3 = __pyx_t_7;
-        goto __pyx_L14_bool_binop_done;
+        __pyx_t_6 = __pyx_t_7;
+        goto __pyx_L13_bool_binop_done;
       }
-      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_result, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_result, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__7, Py_NE)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u_, Py_NE)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_3 = __pyx_t_7;
-      __pyx_L14_bool_binop_done:;
-      if (__pyx_t_3) {
-
-        /* "tarina/_string_c.pyx":50
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
- *             if result and result[-1] != '\0':
- *                 result.append('\0')             # <<<<<<<<<<<<<<
+      __pyx_t_6 = __pyx_t_7;
+      __pyx_L13_bool_binop_done:;
+      if (__pyx_t_6) {
+
+        /* "tarina/_string_c.pyx":61
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
+ *             if result and result[-1] != '\1':
+ *                 PyList_Append(result, '\1')             # <<<<<<<<<<<<<<
  *         else:
- *             result.append(ch)
+ *             PyList_Append(result, ch)
  */
-        __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_result, __pyx_kp_u__7); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 50, __pyx_L1_error)
+        __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_kp_u_); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 61, __pyx_L1_error)
 
-        /* "tarina/_string_c.pyx":49
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
- *             if result and result[-1] != '\0':             # <<<<<<<<<<<<<<
- *                 result.append('\0')
+        /* "tarina/_string_c.pyx":60
+ *                 result[-1] = ch
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
+ *             if result and result[-1] != '\1':             # <<<<<<<<<<<<<<
+ *                 PyList_Append(result, '\1')
  *         else:
  */
       }
 
-      /* "tarina/_string_c.pyx":48
- *                 if escape:
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):             # <<<<<<<<<<<<<<
- *             if result and result[-1] != '\0':
- *                 result.append('\0')
+      /* "tarina/_string_c.pyx":59
+ *             if escape:
+ *                 result[-1] = ch
+ *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):             # <<<<<<<<<<<<<<
+ *             if result and result[-1] != '\1':
+ *                 PyList_Append(result, '\1')
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":52
- *                 result.append('\0')
+    /* "tarina/_string_c.pyx":63
+ *                 PyList_Append(result, '\1')
  *         else:
- *             result.append(ch)             # <<<<<<<<<<<<<<
+ *             PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *             escape = 0
- *     return ''.join(result).split('\0') if result else []
+ *     if PyUnicode_GET_LENGTH(result) == 0:
  */
     /*else*/ {
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
+      __pyx_t_4 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":53
+      /* "tarina/_string_c.pyx":64
  *         else:
- *             result.append(ch)
+ *             PyList_Append(result, ch)
  *             escape = 0             # <<<<<<<<<<<<<<
- *     return ''.join(result).split('\0') if result else []
- * 
+ *     if PyUnicode_GET_LENGTH(result) == 0:
+ *         return []
  */
       __pyx_v_escape = 0;
     }
     __pyx_L5:;
+    __pyx_L3_continue:;
   }
 
-  /* "tarina/_string_c.pyx":54
- *             result.append(ch)
+  /* "tarina/_string_c.pyx":65
+ *             PyList_Append(result, ch)
+ *             escape = 0
+ *     if PyUnicode_GET_LENGTH(result) == 0:             # <<<<<<<<<<<<<<
+ *         return []
+ *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
+ */
+  __pyx_t_6 = ((PyUnicode_GET_LENGTH(__pyx_v_result) == 0) != 0);
+  if (__pyx_t_6) {
+
+    /* "tarina/_string_c.pyx":66
+ *             escape = 0
+ *     if PyUnicode_GET_LENGTH(result) == 0:
+ *         return []             # <<<<<<<<<<<<<<
+ *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+
+    /* "tarina/_string_c.pyx":65
+ *             PyList_Append(result, ch)
  *             escape = 0
- *     return ''.join(result).split('\0') if result else []             # <<<<<<<<<<<<<<
+ *     if PyUnicode_GET_LENGTH(result) == 0:             # <<<<<<<<<<<<<<
+ *         return []
+ *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
+ */
+  }
+
+  /* "tarina/_string_c.pyx":67
+ *     if PyUnicode_GET_LENGTH(result) == 0:
+ *         return []
+ *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = (PyList_GET_SIZE(__pyx_v_result) != 0);
-  if (__pyx_t_3) {
-    __pyx_t_8 = PyUnicode_Join(__pyx_kp_u__8, __pyx_v_result); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = PyUnicode_Split(((PyObject*)__pyx_t_8), __pyx_kp_u__7, -1L); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_1 = __pyx_t_9;
-    __pyx_t_9 = 0;
-  } else {
-    __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_1 = __pyx_t_9;
-    __pyx_t_9 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyUnicode_Split(__pyx_t_1, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":15
- * 
+  /* "tarina/_string_c.pyx":25
+ * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("tarina._string_c.split", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tarina/_string_c.pyx":57
+/* "tarina/_string_c.pyx":70
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
 
@@ -2084,54 +2114,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separates)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, 1); __PYX_ERR(0, 57, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, 1); __PYX_ERR(0, 70, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_crlf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split_once") < 0)) __PYX_ERR(0, 57, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split_once") < 0)) __PYX_ERR(0, 70, __pyx_L3_error)
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
-      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L3_error)
+      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 70, __pyx_L3_error)
     } else {
       __pyx_v_crlf = ((char)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 57, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 70, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tarina._string_c.split_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 57, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 70, __pyx_L1_error)
   __pyx_r = __pyx_pf_6tarina_9_string_c_2split_once(__pyx_self, __pyx_v_text, __pyx_v_separates, __pyx_v_crlf);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2141,434 +2171,488 @@
 
 static PyObject *__pyx_pf_6tarina_9_string_c_2split_once(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_text, PyObject *__pyx_v_separates, char __pyx_v_crlf) {
   Py_ssize_t __pyx_v_index;
   PyObject *__pyx_v_out_text = 0;
   Py_UCS4 __pyx_v_quotation;
   Py_UCS4 __pyx_v_ch;
   char __pyx_v_escape;
+  char __pyx_v_sep;
   Py_ssize_t __pyx_v_length;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  int __pyx_t_3;
-  Py_UCS4 __pyx_t_4;
-  int __pyx_t_5;
+  int __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("split_once", 0);
   __Pyx_INCREF(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":58
+  /* "tarina/_string_c.pyx":71
  * 
  * def split_once(str text, tuple separates, char crlf=True):
  *     text = text.lstrip()             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []
  */
-  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lstrip, __pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lstrip, __pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_text, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":59
+  /* "tarina/_string_c.pyx":72
  * def split_once(str text, tuple separates, char crlf=True):
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0             # <<<<<<<<<<<<<<
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0
  */
   __pyx_v_index = 0;
 
-  /* "tarina/_string_c.pyx":60
+  /* "tarina/_string_c.pyx":73
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_out_text = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":61
+  /* "tarina/_string_c.pyx":74
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0
  */
   __pyx_v_quotation = 0;
 
-  /* "tarina/_string_c.pyx":62
+  /* "tarina/_string_c.pyx":75
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0             # <<<<<<<<<<<<<<
  *     cdef char escape = 0
- *     cdef Py_ssize_t length = len(text)
+ *     cdef char sep = 0
  */
   __pyx_v_ch = 0;
 
-  /* "tarina/_string_c.pyx":63
+  /* "tarina/_string_c.pyx":76
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = len(text)
- * 
+ *     cdef char sep = 0
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  */
   __pyx_v_escape = 0;
 
-  /* "tarina/_string_c.pyx":64
+  /* "tarina/_string_c.pyx":77
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0
- *     cdef Py_ssize_t length = len(text)             # <<<<<<<<<<<<<<
+ *     cdef char sep = 0             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
+ * 
+ */
+  __pyx_v_sep = 0;
+
+  /* "tarina/_string_c.pyx":78
+ *     cdef char escape = 0
+ *     cdef char sep = 0
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)             # <<<<<<<<<<<<<<
  * 
  *     while index < length:
  */
-  if (unlikely(__pyx_v_text == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 64, __pyx_L1_error)
-  }
-  __pyx_t_2 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_text); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_v_length = __pyx_t_2;
+  __pyx_v_length = PyUnicode_GET_LENGTH(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":66
- *     cdef Py_ssize_t length = len(text)
+  /* "tarina/_string_c.pyx":80
+ *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  *     while index < length:             # <<<<<<<<<<<<<<
  *         ch = text[index]
  *         index += 1
  */
   while (1) {
-    __pyx_t_3 = ((__pyx_v_index < __pyx_v_length) != 0);
-    if (!__pyx_t_3) break;
+    __pyx_t_2 = ((__pyx_v_index < __pyx_v_length) != 0);
+    if (!__pyx_t_2) break;
 
-    /* "tarina/_string_c.pyx":67
+    /* "tarina/_string_c.pyx":81
  * 
  *     while index < length:
  *         ch = text[index]             # <<<<<<<<<<<<<<
  *         index += 1
  *         if ch == 92:  # \\
  */
-    __pyx_t_4 = __Pyx_GetItemInt_Unicode(__pyx_v_text, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(__pyx_t_4 == (Py_UCS4)-1)) __PYX_ERR(0, 67, __pyx_L1_error)
-    __pyx_v_ch = __pyx_t_4;
+    __pyx_t_3 = __Pyx_GetItemInt_Unicode(__pyx_v_text, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(__pyx_t_3 == (Py_UCS4)-1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_v_ch = __pyx_t_3;
 
-    /* "tarina/_string_c.pyx":68
+    /* "tarina/_string_c.pyx":82
  *     while index < length:
  *         ch = text[index]
  *         index += 1             # <<<<<<<<<<<<<<
  *         if ch == 92:  # \\
  *             escape = 1
  */
     __pyx_v_index = (__pyx_v_index + 1);
 
-    /* "tarina/_string_c.pyx":69
+    /* "tarina/_string_c.pyx":83
  *         ch = text[index]
  *         index += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
- *             out_text.append(ch)
+ *             PyList_Append(out_text, ch)
  */
-    __pyx_t_3 = ((__pyx_v_ch == 92) != 0);
-    if (__pyx_t_3) {
+    __pyx_t_2 = ((__pyx_v_ch == 92) != 0);
+    if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":70
+      /* "tarina/_string_c.pyx":84
  *         index += 1
  *         if ch == 92:  # \\
  *             escape = 1             # <<<<<<<<<<<<<<
- *             out_text.append(ch)
- *         elif contains(ch, ('"', "'")):  #
+ *             PyList_Append(out_text, ch)
+ *         elif set_contains_key(QUOTES, ch):  #
  */
       __pyx_v_escape = 1;
 
-      /* "tarina/_string_c.pyx":71
+      /* "tarina/_string_c.pyx":85
  *         if ch == 92:  # \\
  *             escape = 1
- *             out_text.append(ch)             # <<<<<<<<<<<<<<
- *         elif contains(ch, ('"', "'")):  #
+ *             PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
+ *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:
  */
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 71, __pyx_L1_error)
+      __pyx_t_4 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":69
+      /* "tarina/_string_c.pyx":83
  *         ch = text[index]
  *         index += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
- *             out_text.append(ch)
+ *             PyList_Append(out_text, ch)
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":72
+    /* "tarina/_string_c.pyx":86
  *             escape = 1
- *             out_text.append(ch)
- *         elif contains(ch, ('"', "'")):  #             # <<<<<<<<<<<<<<
+ *             PyList_Append(out_text, ch)
+ *         elif set_contains_key(QUOTES, ch):  #             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
-    __pyx_t_3 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_ch, __pyx_tuple__3) != 0);
-    if (__pyx_t_3) {
-
-      /* "tarina/_string_c.pyx":73
- *             out_text.append(ch)
- *         elif contains(ch, ('"', "'")):  #
+    __pyx_t_1 = __pyx_v_6tarina_9_string_c_QUOTES;
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_5); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_6 = (__pyx_t_2 != 0);
+    if (__pyx_t_6) {
+
+      /* "tarina/_string_c.pyx":87
+ *             PyList_Append(out_text, ch)
+ *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
- *                 if escape:
+ *             elif ch == quotation:
  */
-      __pyx_t_3 = ((__pyx_v_quotation == 0) != 0);
-      if (__pyx_t_3) {
+      __pyx_t_6 = ((__pyx_v_quotation == 0) != 0);
+      if (__pyx_t_6) {
 
-        /* "tarina/_string_c.pyx":74
- *         elif contains(ch, ('"', "'")):  #
+        /* "tarina/_string_c.pyx":88
+ *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:
  *                 quotation = ch             # <<<<<<<<<<<<<<
- *                 if escape:
- *                     out_text[-1] = ch
- */
-        __pyx_v_quotation = __pyx_v_ch;
-
-        /* "tarina/_string_c.pyx":75
- *             if quotation == 0:
- *                 quotation = ch
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     out_text[-1] = ch
- *             elif ch == quotation:
- */
-        __pyx_t_3 = (__pyx_v_escape != 0);
-        if (__pyx_t_3) {
-
-          /* "tarina/_string_c.pyx":76
- *                 quotation = ch
- *                 if escape:
- *                     out_text[-1] = ch             # <<<<<<<<<<<<<<
  *             elif ch == quotation:
  *                 quotation = 0
  */
-          __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (unlikely(__Pyx_SetItemInt(__pyx_v_out_text, -1L, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 76, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-          /* "tarina/_string_c.pyx":75
- *             if quotation == 0:
- *                 quotation = ch
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     out_text[-1] = ch
- *             elif ch == quotation:
- */
-        }
+        __pyx_v_quotation = __pyx_v_ch;
 
-        /* "tarina/_string_c.pyx":73
- *             out_text.append(ch)
- *         elif contains(ch, ('"', "'")):  #
+        /* "tarina/_string_c.pyx":87
+ *             PyList_Append(out_text, ch)
+ *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
- *                 if escape:
+ *             elif ch == quotation:
  */
         goto __pyx_L6;
       }
 
-      /* "tarina/_string_c.pyx":77
- *                 if escape:
- *                     out_text[-1] = ch
+      /* "tarina/_string_c.pyx":89
+ *             if quotation == 0:
+ *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
- *                 if escape:
+ *             else:
  */
-      __pyx_t_3 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
-      if (__pyx_t_3) {
+      __pyx_t_6 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
+      if (__pyx_t_6) {
 
-        /* "tarina/_string_c.pyx":78
- *                     out_text[-1] = ch
+        /* "tarina/_string_c.pyx":90
+ *                 quotation = ch
  *             elif ch == quotation:
  *                 quotation = 0             # <<<<<<<<<<<<<<
- *                 if escape:
- *                     out_text[-1] = ch
+ *             else:
+ *                 PyList_Append(out_text, ch)
  */
         __pyx_v_quotation = 0;
 
-        /* "tarina/_string_c.pyx":79
- *             elif ch == quotation:
+        /* "tarina/_string_c.pyx":89
+ *             if quotation == 0:
+ *                 quotation = ch
+ *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     out_text[-1] = ch
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:
+ *             else:
  */
-        __pyx_t_3 = (__pyx_v_escape != 0);
-        if (__pyx_t_3) {
-
-          /* "tarina/_string_c.pyx":80
- *                 quotation = 0
- *                 if escape:
- *                     out_text[-1] = ch             # <<<<<<<<<<<<<<
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:
- *             break
- */
-          __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (unlikely(__Pyx_SetItemInt(__pyx_v_out_text, -1L, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 80, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        goto __pyx_L6;
+      }
 
-          /* "tarina/_string_c.pyx":79
- *             elif ch == quotation:
+      /* "tarina/_string_c.pyx":92
  *                 quotation = 0
- *                 if escape:             # <<<<<<<<<<<<<<
- *                     out_text[-1] = ch
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:
+ *             else:
+ *                 PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
+ *                 continue
+ *             if escape:
+ */
+      /*else*/ {
+        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_4 = PyList_Append(__pyx_v_out_text, __pyx_t_5); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 92, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+        /* "tarina/_string_c.pyx":93
+ *             else:
+ *                 PyList_Append(out_text, ch)
+ *                 continue             # <<<<<<<<<<<<<<
+ *             if escape:
+ *                 out_text[-1] = ch
  */
-        }
+        goto __pyx_L3_continue;
+      }
+      __pyx_L6:;
 
-        /* "tarina/_string_c.pyx":77
- *                 if escape:
- *                     out_text[-1] = ch
- *             elif ch == quotation:             # <<<<<<<<<<<<<<
- *                 quotation = 0
- *                 if escape:
+      /* "tarina/_string_c.pyx":94
+ *                 PyList_Append(out_text, ch)
+ *                 continue
+ *             if escape:             # <<<<<<<<<<<<<<
+ *                 out_text[-1] = ch
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+ */
+      __pyx_t_6 = (__pyx_v_escape != 0);
+      if (__pyx_t_6) {
+
+        /* "tarina/_string_c.pyx":95
+ *                 continue
+ *             if escape:
+ *                 out_text[-1] = ch             # <<<<<<<<<<<<<<
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+ *             sep = 1
+ */
+        __pyx_t_5 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_out_text, -1L, __pyx_t_5, long, 1, __Pyx_PyInt_From_long, 1, 1, 0) < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+        /* "tarina/_string_c.pyx":94
+ *                 PyList_Append(out_text, ch)
+ *                 continue
+ *             if escape:             # <<<<<<<<<<<<<<
+ *                 out_text[-1] = ch
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
  */
       }
-      __pyx_L6:;
 
-      /* "tarina/_string_c.pyx":72
+      /* "tarina/_string_c.pyx":86
  *             escape = 1
- *             out_text.append(ch)
- *         elif contains(ch, ('"', "'")):  #             # <<<<<<<<<<<<<<
+ *             PyList_Append(out_text, ch)
+ *         elif set_contains_key(QUOTES, ch):  #             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":81
- *                 if escape:
- *                     out_text[-1] = ch
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:             # <<<<<<<<<<<<<<
- *             break
- *         else:
+    /* "tarina/_string_c.pyx":96
+ *             if escape:
+ *                 out_text[-1] = ch
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:             # <<<<<<<<<<<<<<
+ *             sep = 1
+ *             continue
  */
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_v_separates, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 81, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = (__pyx_t_6 != 0);
-    if (!__pyx_t_7) {
+    __pyx_t_2 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
+    if (!__pyx_t_2) {
     } else {
-      goto __pyx_L10_next_and;
+      goto __pyx_L9_next_and;
     }
-    __pyx_t_7 = (__pyx_v_crlf != 0);
-    if (__pyx_t_7) {
+    __pyx_t_2 = (__pyx_v_crlf != 0);
+    if (__pyx_t_2) {
     } else {
-      __pyx_t_3 = __pyx_t_7;
-      goto __pyx_L9_bool_binop_done;
+      __pyx_t_6 = __pyx_t_2;
+      goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_7 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_ch, __pyx_tuple__9) != 0);
+    __pyx_t_5 = __pyx_v_6tarina_9_string_c_CRLF;
+    __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = set_contains_key(__pyx_t_5, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_7 = (__pyx_t_2 != 0);
     if (__pyx_t_7) {
     } else {
-      __pyx_t_3 = __pyx_t_7;
-      goto __pyx_L9_bool_binop_done;
+      __pyx_t_6 = __pyx_t_7;
+      goto __pyx_L8_bool_binop_done;
     }
-    __pyx_L10_next_and:;
+    __pyx_L9_next_and:;
     __pyx_t_7 = ((__pyx_v_quotation == 0) != 0);
-    __pyx_t_3 = __pyx_t_7;
-    __pyx_L9_bool_binop_done:;
-    if (__pyx_t_3) {
-
-      /* "tarina/_string_c.pyx":82
- *                     out_text[-1] = ch
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:
- *             break             # <<<<<<<<<<<<<<
+    __pyx_t_6 = __pyx_t_7;
+    __pyx_L8_bool_binop_done:;
+    if (__pyx_t_6) {
+
+      /* "tarina/_string_c.pyx":97
+ *                 out_text[-1] = ch
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+ *             sep = 1             # <<<<<<<<<<<<<<
+ *             continue
  *         else:
- *             out_text.append(ch)
  */
-      goto __pyx_L4_break;
+      __pyx_v_sep = 1;
 
-      /* "tarina/_string_c.pyx":81
- *                 if escape:
- *                     out_text[-1] = ch
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:             # <<<<<<<<<<<<<<
- *             break
+      /* "tarina/_string_c.pyx":98
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+ *             sep = 1
+ *             continue             # <<<<<<<<<<<<<<
  *         else:
+ *             if sep == 1:
+ */
+      goto __pyx_L3_continue;
+
+      /* "tarina/_string_c.pyx":96
+ *             if escape:
+ *                 out_text[-1] = ch
+ *         elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:             # <<<<<<<<<<<<<<
+ *             sep = 1
+ *             continue
  */
     }
 
-    /* "tarina/_string_c.pyx":84
- *             break
+    /* "tarina/_string_c.pyx":100
+ *             continue
  *         else:
- *             out_text.append(ch)             # <<<<<<<<<<<<<<
- *             escape = 0
- *     return ''.join(out_text), text[index:]
+ *             if sep == 1:             # <<<<<<<<<<<<<<
+ *                 index -= 1
+ *                 break
  */
     /*else*/ {
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+      __pyx_t_6 = ((__pyx_v_sep == 1) != 0);
+      if (__pyx_t_6) {
+
+        /* "tarina/_string_c.pyx":101
+ *         else:
+ *             if sep == 1:
+ *                 index -= 1             # <<<<<<<<<<<<<<
+ *                 break
+ *             PyList_Append(out_text, ch)
+ */
+        __pyx_v_index = (__pyx_v_index - 1);
+
+        /* "tarina/_string_c.pyx":102
+ *             if sep == 1:
+ *                 index -= 1
+ *                 break             # <<<<<<<<<<<<<<
+ *             PyList_Append(out_text, ch)
+ *             escape = 0
+ */
+        goto __pyx_L4_break;
+
+        /* "tarina/_string_c.pyx":100
+ *             continue
+ *         else:
+ *             if sep == 1:             # <<<<<<<<<<<<<<
+ *                 index -= 1
+ *                 break
+ */
+      }
+
+      /* "tarina/_string_c.pyx":103
+ *                 index -= 1
+ *                 break
+ *             PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
+ *             escape = 0
+ *     return PyUnicode_Join('', out_text), text[index:]
+ */
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 84, __pyx_L1_error)
+      __pyx_t_4 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 103, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":85
- *         else:
- *             out_text.append(ch)
+      /* "tarina/_string_c.pyx":104
+ *                 break
+ *             PyList_Append(out_text, ch)
  *             escape = 0             # <<<<<<<<<<<<<<
- *     return ''.join(out_text), text[index:]
+ *     return PyUnicode_Join('', out_text), text[index:]
  */
       __pyx_v_escape = 0;
     }
     __pyx_L5:;
+    __pyx_L3_continue:;
   }
   __pyx_L4_break:;
 
-  /* "tarina/_string_c.pyx":86
- *             out_text.append(ch)
+  /* "tarina/_string_c.pyx":105
+ *             PyList_Append(out_text, ch)
  *             escape = 0
- *     return ''.join(out_text), text[index:]             # <<<<<<<<<<<<<<
+ *     return PyUnicode_Join('', out_text), text[index:]             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__8, __pyx_v_out_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_out_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_v_text == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 86, __pyx_L1_error)
+    __PYX_ERR(0, 105, __pyx_L1_error)
   }
-  __pyx_t_8 = __Pyx_PyUnicode_Substring(__pyx_v_text, __pyx_v_index, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Substring(__pyx_v_text, __pyx_v_index, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_5);
   __pyx_t_1 = 0;
+  __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
-  __pyx_r = __pyx_t_9;
-  __pyx_t_9 = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":57
+  /* "tarina/_string_c.pyx":70
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("tarina._string_c.split_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_out_text);
   __Pyx_XDECREF(__pyx_v_text);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -2619,31 +2703,32 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
+  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
   {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
-  {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
-  {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
+  {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
   {&__pyx_n_s_ch, __pyx_k_ch, sizeof(__pyx_k_ch), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_crlf, __pyx_k_crlf, sizeof(__pyx_k_crlf), 0, 0, 1, 1},
   {&__pyx_n_s_escape, __pyx_k_escape, sizeof(__pyx_k_escape), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
   {&__pyx_n_s_lstrip, __pyx_k_lstrip, sizeof(__pyx_k_lstrip), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_out_text, __pyx_k_out_text, sizeof(__pyx_k_out_text), 0, 0, 1, 1},
   {&__pyx_n_s_quotation, __pyx_k_quotation, sizeof(__pyx_k_quotation), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
+  {&__pyx_n_s_sep, __pyx_k_sep, sizeof(__pyx_k_sep), 0, 0, 1, 1},
   {&__pyx_n_s_separates, __pyx_k_separates, sizeof(__pyx_k_separates), 0, 0, 1, 1},
   {&__pyx_n_s_split, __pyx_k_split, sizeof(__pyx_k_split), 0, 0, 1, 1},
   {&__pyx_n_s_split_once, __pyx_k_split_once, sizeof(__pyx_k_split_once), 0, 0, 1, 1},
   {&__pyx_kp_s_src_tarina__string_c_pyx, __pyx_k_src_tarina__string_c_pyx, sizeof(__pyx_k_src_tarina__string_c_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_tarina__string_c, __pyx_k_tarina__string_c, sizeof(__pyx_k_tarina__string_c), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
@@ -2653,70 +2738,37 @@
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "tarina/_string_c.pyx":39
- *             escape = 1
- *             result.append(ch)
- *         elif contains(ch, ('"', "'")):             # <<<<<<<<<<<<<<
- *             if quotation == 0:
- *                 quotation = ch
- */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_kp_u__2); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "tarina/_string_c.pyx":48
- *                 if escape:
- *                     result[-1] = ch
- *         elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):             # <<<<<<<<<<<<<<
- *             if result and result[-1] != '\0':
- *                 result.append('\0')
- */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_kp_u__4, __pyx_kp_u__5); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 48, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "tarina/_string_c.pyx":81
- *                 if escape:
- *                     out_text[-1] = ch
- *         elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:             # <<<<<<<<<<<<<<
- *             break
- *         else:
- */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_kp_u__5, __pyx_kp_u__4); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 81, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-
-  /* "tarina/_string_c.pyx":15
- * 
+  /* "tarina/_string_c.pyx":25
+ * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_escape, __pyx_n_s_result, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_i, __pyx_n_s_length); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_escape, __pyx_n_s_result, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_i, __pyx_n_s_length); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 25, __pyx_L1_error)
 
-  /* "tarina/_string_c.pyx":57
+  /* "tarina/_string_c.pyx":70
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
-  __pyx_tuple__12 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_index, __pyx_n_s_out_text, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_escape, __pyx_n_s_length); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split_once, 57, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(10, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_index, __pyx_n_s_out_text, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_escape, __pyx_n_s_sep, __pyx_n_s_length); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split_once, 70, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2736,14 +2788,16 @@
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
+  __pyx_v_6tarina_9_string_c_QUOTES = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  __pyx_v_6tarina_9_string_c_CRLF = ((PyObject*)Py_None); Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
@@ -2766,18 +2820,37 @@
   /*--- Type init code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  #else
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  #endif
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_variable_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __Pyx_RefNannyFinishContext();
@@ -2980,44 +3053,76 @@
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  (void)__Pyx_modinit_type_import_code();
+  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "tarina/_string_c.pyx":15
+  /* "tarina/_string_c.pyx":22
+ *     return 0
  * 
+ * cdef set QUOTES = {'"', '\''}             # <<<<<<<<<<<<<<
+ * cdef set CRLF = {'\r', '\n'}
+ * 
+ */
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__4) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_XGOTREF(__pyx_v_6tarina_9_string_c_QUOTES);
+  __Pyx_DECREF_SET(__pyx_v_6tarina_9_string_c_QUOTES, ((PyObject*)__pyx_t_1));
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "tarina/_string_c.pyx":23
+ * 
+ * cdef set QUOTES = {'"', '\''}
+ * cdef set CRLF = {'\r', '\n'}             # <<<<<<<<<<<<<<
+ * 
+ * def split(str text, tuple separates, char crlf=True):
+ */
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__5) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__6) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_XGOTREF(__pyx_v_6tarina_9_string_c_CRLF);
+  __Pyx_DECREF_SET(__pyx_v_6tarina_9_string_c_CRLF, ((PyObject*)__pyx_t_1));
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "tarina/_string_c.pyx":25
+ * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_1split, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_1split, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":57
+  /* "tarina/_string_c.pyx":70
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_3split_once, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_3split_once, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split_once, __pyx_t_1) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split_once, __pyx_t_1) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "tarina/_string_c.pyx":1
  * # cython: boundscheck=False             # <<<<<<<<<<<<<<
  * # cython: cdivision=True
  * # cython: initializedcheck=False
  */
@@ -3064,101 +3169,14 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
 /* BytesEquals */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
 #if CYTHON_COMPILING_IN_PYPY
     return PyObject_RichCompareBool(s1, s2, equals);
 #else
     if (s1 == s2) {
         return (equals == Py_EQ);
@@ -3595,14 +3613,101 @@
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
@@ -3693,14 +3798,93 @@
     return PyUnicode_FromKindAndData(PyUnicode_KIND(text),
         PyUnicode_1BYTE_DATA(text) + start*PyUnicode_KIND(text), stop-start);
 #else
     return PyUnicode_FromUnicode(PyUnicode_AS_UNICODE(text)+start, stop-start);
 #endif
 }
 
+/* TypeImport */
+#ifndef __PYX_HAVE_RT_ImportType
+#define __PYX_HAVE_RT_ImportType
+static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+{
+    PyObject *result = 0;
+    char warning[200];
+    Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
+#ifdef Py_LIMITED_API
+    PyObject *py_basicsize;
+    PyObject *py_itemsize;
+#endif
+    result = PyObject_GetAttrString(module, class_name);
+    if (!result)
+        goto bad;
+    if (!PyType_Check(result)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s.%.200s is not a type object",
+            module_name, class_name);
+        goto bad;
+    }
+#ifndef Py_LIMITED_API
+    basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
+#else
+    py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
+    if (!py_basicsize)
+        goto bad;
+    basicsize = PyLong_AsSsize_t(py_basicsize);
+    Py_DECREF(py_basicsize);
+    py_basicsize = 0;
+    if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
+#endif
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
+        PyErr_Format(PyExc_ValueError,
+            "%.200s.%.200s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
+        goto bad;
+    }
+    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+        PyErr_Format(PyExc_ValueError,
+            "%.200s.%.200s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
+        goto bad;
+    }
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+        PyOS_snprintf(warning, sizeof(warning),
+            "%s.%s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
+        if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
+    }
+    return (PyTypeObject *)result;
+bad:
+    Py_XDECREF(result);
+    return NULL;
+}
+#endif
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -4204,14 +4388,90 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const char neg_one = (char) -1, const_zero = (char) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(char) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(char) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(char) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(char),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
```

### Comparing `tarina-0.2.1/src/tarina/_string_c.pyi` & `tarina-0.2.2/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/_string_c.pyx` & `tarina-0.2.2/src/tarina/_string_c.pyx`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 # cython: boundscheck=False
 # cython: cdivision=True
 # cython: initializedcheck=False
 
-cdef inline int contains(Py_UCS4 ch, tuple chs):
+from cpython.object cimport PyObject, Py_SIZE
+from cpython.unicode cimport PyUnicode_Join, PyUnicode_Split, PyUnicode_GET_LENGTH
+from cpython.list cimport PyList_Append
+
+cdef extern from "_op.h":
+    PyObject* tupleitem(object a, Py_ssize_t i)
+    bint set_contains_key(object anyset, object key) except -1
+
+cdef inline int contains(tuple chs, Py_UCS4 ch):
     cdef Py_ssize_t i = 0
-    cdef Py_ssize_t length = len(chs)
+    cdef Py_ssize_t length = Py_SIZE(chs)
     while i < length:
-        if ch == chs[i]:
+        if ch == <object>tupleitem(chs, i):
             return 1
         i += 1
     return 0
 
+cdef set QUOTES = {'"', '\''}
+cdef set CRLF = {'\r', '\n'}
 
 def split(str text, tuple separates, char crlf=True):
     """尊重引号与转义的字符串切分
 
     Args:
         text (str): 要切割的字符串
         separates (tuple[str, ...]): 切割符. 默认为 " ".
@@ -24,63 +34,72 @@
         List[str]: 切割后的字符串, 可能含有空格
     """
     cdef char escape = 0
     cdef list result = []
     cdef Py_UCS4 quotation = 0
     cdef Py_UCS4 ch = 0
     cdef Py_ssize_t i = 0
-    cdef Py_ssize_t length = len(text)
+    cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
 
     while i < length:
         ch = text[i]
         i += 1
         if ch == 92:  # \\
             escape = 1
-            result.append(ch)
-        elif contains(ch, ('"', "'")):
+            PyList_Append(result, ch)
+        elif set_contains_key(QUOTES, ch):
             if quotation == 0:
                 quotation = ch
-                if escape:
-                    result[-1] = ch
             elif ch == quotation:
                 quotation = 0
-                if escape:
-                    result[-1] = ch
-        elif (quotation == 0 and ch in separates) or (crlf and contains(ch, ('\r', '\n'))):
-            if result and result[-1] != '\0':
-                result.append('\0')
+            else:
+                PyList_Append(result, ch)
+                continue
+            if escape:
+                result[-1] = ch
+        elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
+            if result and result[-1] != '\1':
+                PyList_Append(result, '\1')
         else:
-            result.append(ch)
+            PyList_Append(result, ch)
             escape = 0
-    return ''.join(result).split('\0') if result else []
+    if PyUnicode_GET_LENGTH(result) == 0:
+        return []
+    return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
 
 
 def split_once(str text, tuple separates, char crlf=True):
     text = text.lstrip()
     cdef Py_ssize_t index = 0
     cdef list out_text = []
     cdef Py_UCS4 quotation = 0
     cdef Py_UCS4 ch = 0
     cdef char escape = 0
-    cdef Py_ssize_t length = len(text)
+    cdef char sep = 0
+    cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
 
     while index < length:
         ch = text[index]
         index += 1
         if ch == 92:  # \\
             escape = 1
-            out_text.append(ch)
-        elif contains(ch, ('"', "'")):  # 遇到引号括起来的部分跳过分隔
+            PyList_Append(out_text, ch)
+        elif set_contains_key(QUOTES, ch):  # 遇到引号括起来的部分跳过分隔
             if quotation == 0:
                 quotation = ch
-                if escape:
-                    out_text[-1] = ch
             elif ch == quotation:
                 quotation = 0
-                if escape:
-                    out_text[-1] = ch
-        elif (ch in separates or (crlf and contains(ch, ('\n', '\r')))) and quotation == 0:
-            break
+            else:
+                PyList_Append(out_text, ch)
+                continue
+            if escape:
+                out_text[-1] = ch
+        elif (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))) and quotation == 0:
+            sep = 1
+            continue
         else:
-            out_text.append(ch)
+            if sep == 1:
+                index -= 1
+                break
+            PyList_Append(out_text, ch)
             escape = 0
-    return ''.join(out_text), text[index:]
+    return PyUnicode_Join('', out_text), text[index:]
```

### Comparing `tarina-0.2.1/src/tarina/_string_py.py` & `tarina-0.2.2/src/tarina/_string_py.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 from __future__ import annotations
 
-QUOTATION = {"'", '"', "’", "“"}
+QUOTATION = {"'", '"'}
+CRLF = {"\n", "\r"}
 
 
 def split_once(text: str, separates: tuple[str, ...], crlf: bool = True):
     """尊重引号与转义的字符串切分, 只切割一次
 
     Args:
         text (str): 要切割的字符串
         separates (tuple[str, ...]): 切割符.
         crlf (bool): 是否去除 \n 与 \r，默认为 True
     Returns:
         Tuple[str, str]: 切割后的字符串, 可能含有空格
     """
-    index, out_text, quotation, escape = 0, "", "", False
+    index, out_text, quotation, escape, sep = 0, "", "", False, False
     text = text.lstrip()
     for char in text:
         index += 1
         if char == "\\":
             escape = True
             out_text += char
         elif char in QUOTATION:  # 遇到引号括起来的部分跳过分隔
             if not quotation:
                 quotation = char
-                if escape:
-                    out_text = out_text[:-1] + char
             elif char == quotation:
                 quotation = ""
-                if escape:
-                    out_text = out_text[:-1] + char
-        elif (char in separates or (crlf and char in {"\n", "\r"})) and not quotation:
-            break
+            else:
+                out_text += char
+                continue
+            if escape:
+                out_text = out_text[:-1] + char
+        elif (char in separates or (crlf and char in CRLF)) and not quotation:
+            sep = True
+            continue
         else:
+            if sep:
+                index -= 1
+                break
             out_text += char
             escape = False
     return out_text, text[index:]
 
 
 def split(text: str, separates: tuple[str, ...], crlf: bool = True):
     """尊重引号与转义的字符串切分
@@ -52,20 +58,21 @@
     for char in text:
         if char == "\\":
             escape = True
             result += char
         elif char in QUOTATION:
             if not quotation:
                 quotation = char
-                if escape:
-                    result = result[:-1] + char
             elif char == quotation:
                 quotation = ""
-                if escape:
-                    result = result[:-1] + char
-        elif (not quotation and char in separates) or (crlf and char in {"\n", "\r"}):
+            else:
+                result += char
+                continue
+            if escape:
+                result = result[:-1] + char
+        elif (not quotation and char in separates) or (crlf and char in CRLF):
             if result and result[-1] != "\0":
                 result += "\0"
         else:
             result += char
             escape = False
     return result.split('\0') if result else []
```

### Comparing `tarina-0.2.1/src/tarina/context.py` & `tarina-0.2.2/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/generic.py` & `tarina-0.2.2/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/guard.py` & `tarina-0.2.2/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/lru.pyi` & `tarina-0.2.2/src/tarina/lru.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/signature.py` & `tarina-0.2.2/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/string.py` & `tarina-0.2.2/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina/tools.py` & `tarina-0.2.2/src/tarina/tools.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.1/src/tarina.egg-info/PKG-INFO` & `tarina-0.2.2/src/tarina.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.2.1/src/tarina.egg-info/SOURCES.txt` & `tarina-0.2.2/src/tarina.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 src/tarina/__init__.py
 src/tarina/_lru_c.c
 src/tarina/_lru_c.pyi
 src/tarina/_lru_py.py
+src/tarina/_op.h
 src/tarina/_string_c.c
 src/tarina/_string_c.pyi
 src/tarina/_string_c.pyx
 src/tarina/_string_py.py
 src/tarina/const.py
 src/tarina/context.py
 src/tarina/generic.py
```

