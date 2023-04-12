# Comparing `tmp/sparseqr-1.2.tar.gz` & `tmp/sparseqr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparseqr-1.2.tar", max compression
+gzip compressed data, was "sparseqr-1.2.1.tar", max compression
```

## Comparing `sparseqr-1.2.tar` & `sparseqr-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     7049 2017-08-30 16:53:09.000000 sparseqr-1.2/LICENSE.md
--rw-r--r--   0        0        0     4398 2022-05-27 18:12:06.886055 sparseqr-1.2/README.md
--rw-r--r--   0        0        0      479 2022-05-27 16:35:21.356810 sparseqr-1.2/pyproject.toml
--rw-r--r--   0        0        0      739 2022-05-27 16:40:02.816496 sparseqr-1.2/sparseqr/__init__.py
--rw-r--r--   0        0        0     1539 2017-08-30 16:53:09.000000 sparseqr-1.2/sparseqr/cffi_asarray.py
--rw-r--r--   0        0        0    16497 2022-05-27 16:34:33.658003 sparseqr-1.2/sparseqr/sparseqr.py
--rw-r--r--   0        0        0    15737 2022-05-27 18:19:25.771360 sparseqr-1.2/sparseqr/sparseqr_gen.py
--rw-r--r--   0        0        0     2097 2022-05-27 18:16:56.475818 sparseqr-1.2/test/test.py
--rw-r--r--   0        0        0      652 2022-05-27 18:22:46.269318 sparseqr-1.2/setup.py
--rw-r--r--   0        0        0      606 2022-05-27 18:22:46.269538 sparseqr-1.2/PKG-INFO
+-rw-r--r--   0        0        0     7049 2017-08-30 16:53:09.000000 sparseqr-1.2.1/LICENSE.md
+-rw-r--r--   0        0        0     4500 2023-04-12 16:14:35.258190 sparseqr-1.2.1/README.md
+-rw-r--r--   0        0        0      481 2023-04-12 15:59:16.414247 sparseqr-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      741 2023-04-12 15:53:31.124753 sparseqr-1.2.1/sparseqr/__init__.py
+-rw-r--r--   0        0        0     1539 2017-08-30 16:53:09.000000 sparseqr-1.2.1/sparseqr/cffi_asarray.py
+-rw-r--r--   0        0        0    16599 2023-04-12 16:00:33.094078 sparseqr-1.2.1/sparseqr/sparseqr.py
+-rw-r--r--   0        0        0    15737 2022-05-27 18:19:25.771360 sparseqr-1.2.1/sparseqr/sparseqr_gen.py
+-rw-r--r--   0        0        0     2577 2023-04-12 16:14:19.984513 sparseqr-1.2.1/test/test.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 sparseqr-1.2.1/PKG-INFO
```

### Comparing `sparseqr-1.2/LICENSE.md` & `sparseqr-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sparseqr-1.2/README.md` & `sparseqr-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,50 +16,52 @@
 import scipy.sparse.linalg
 import sparseqr
 
 # QR decompose a sparse matrix M such that  Q R = M E
 #
 M = scipy.sparse.rand( 10, 10, density = 0.1 )
 Q, R, E, rank = sparseqr.qr( M )
-print( abs( Q*R - M*sparseqr.permutation_vector_to_matrix(E) ).sum() )  # should be approximately zero
+print( "Should be approximately zero:", abs( Q*R - M*sparseqr.permutation_vector_to_matrix(E) ).sum() ) 
 
 # Solve many linear systems "M x = b for b in columns(B)"
 #
 B = scipy.sparse.rand( 10, 5, density = 0.1 )  # many RHS, sparse (could also have just one RHS with shape (10,))
 x = sparseqr.solve( M, B, tolerance = 0 )
 
 # Solve an overdetermined linear system  A x = b  in the least-squares sense
 #
 # The same routine also works for the usual non-overdetermined case.
 #
 A = scipy.sparse.rand( 20, 10, density = 0.1 )  # 20 equations, 10 unknowns
 b = numpy.random.random(20)  # one RHS, dense, but could also have many (in shape (20,k))
 x = sparseqr.solve( A, b, tolerance = 0 )
+## Call `rz()`:
+sparseqr.rz( A, b, tolerance = 0 )
 
 # Solve a linear system  M x = B  via QR decomposition
 #
 # This approach is slow due to the explicit construction of Q, but may be
 # useful if a large number of systems need to be solved with the same M.
 #
 M = scipy.sparse.rand( 10, 10, density = 0.1 )
 Q, R, E, rank = sparseqr.qr( M )
 r = rank  # r could be min(M.shape) if M is full-rank
 
 # The system is only solvable if the lower part of Q.T @ B is all zero:
-print( "System is solvable if this is zero:", abs( (( Q.tocsc()[:,r:] ).T ).dot( B ) ).sum() )
+print( "System is solvable if this is zero (unlikely for a random matrix):", abs( (( Q.tocsc()[:,r:] ).T ).dot( B ) ).sum() )
 
 # Systems with large non-square matrices can benefit from "economy" decomposition.
 M = scipy.sparse.rand( 20, 5, density=0.1 )
 B = scipy.sparse.rand( 20, 5, density = 0.1 )
 Q, R, E, rank = sparseqr.qr( M )
-print("Q shape:", Q.shape)  # Q shape: (20, 20)
-print("R shape:", R.shape)  # R shape: (20, 5)
+print("Q shape (should be 20x20):", Q.shape)
+print("R shape (should be 20x5):", R.shape)
 Q, R, E, rank = sparseqr.qr( M, economy=True )
-print("Q shape:", Q.shape)  # Q shape: (20, 5)
-print("R shape:", R.shape)  # R shape: (5, 5)
+print("Q shape (should be 20x5):", Q.shape)
+print("R shape (should be 5x5):", R.shape)
 
 # Use CSC format for fast indexing of columns.
 R = R.tocsc()[:r,:r]
 Q = Q.tocsc()[:,:r]
 QB = (Q.T).dot(B).tocsc()  # for best performance, spsolve() wants the RHS to be in CSC format.
 result = scipy.sparse.linalg.spsolve(R, QB)
 
@@ -111,24 +113,28 @@
 or leave them in their directory and call it as a module.
 
 
 # Deploy
 
 1. Change the version in:
 
+    ```
     sparseqr/__init__.py
-    setup.py 
-    pyproject.toml 
+    setup.py
+    pyproject.toml
+    ```
 
 2. Update `CHANGELOG.md`
 
 3. Run:
 
+    ```
     poetry build -f sdist
     poetry publish
+    ```
 
 # Known issues
 
 `pip uninstall sparseqr` won't remove the generated libraries. It will list them with a warning.
 
 # Tested on
```

### Comparing `sparseqr-1.2/sparseqr/__init__.py` & `sparseqr-1.2.1/sparseqr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 In solve(), the RHS can be dense or sparse.
 
 See the docstrings of the individual functions for details.
 """
 
 from __future__ import absolute_import
 
-__version__ = '1.2'
+__version__ = '1.2.1'
 
 # import the important things into the package's top-level namespace.
 from .sparseqr import qr, rz, solve, permutation_vector_to_matrix
```

### Comparing `sparseqr-1.2/sparseqr/cffi_asarray.py` & `sparseqr-1.2.1/sparseqr/cffi_asarray.py`

 * *Files identical despite different names*

### Comparing `sparseqr-1.2/sparseqr/sparseqr.py` & `sparseqr-1.2.1/sparseqr/sparseqr.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,14 +236,16 @@
         E = None
     else:
         E = asarray( ffi, chol_E[0], A.shape[1] ).copy()
 
     ## Free cholmod stuff
     cholmod_free_dense( chol_Z[0] )
     cholmod_free_sparse( chol_R[0] )
+    cholmod_free_sparse( chol_A )
+    cholmod_free_dense(  chol_b )
 
     return scipy_Z, scipy_R, E, rank
 
 
 def qr( A, tolerance = None, economy = None ):
     '''
     Given a sparse matrix A,
@@ -338,14 +340,15 @@
         # E[0:A.shape[1]] = list( chol_E[0][0:A.shape[1]] )
         ## UPDATE: I can do this without going through list() or making two extra copies.
         E = asarray( ffi, chol_E[0], A.shape[1] ).copy()
 
     ## Free cholmod stuff
     cholmod_free_sparse( chol_Q[0] )
     cholmod_free_sparse( chol_R[0] )
+    cholmod_free_sparse( chol_A )
     ## Apparently we don't need to do this. (I get a malloc error.)
     # lib.cholmod_l_free( A.shape[1], ffi.sizeof("SuiteSparse_long"), chol_E, cc )
 
     return scipy_Q, scipy_R, E, rank
 
 
 def solve( A, b, tolerance = None ):
```

### Comparing `sparseqr-1.2/sparseqr/sparseqr_gen.py` & `sparseqr-1.2.1/sparseqr/sparseqr_gen.py`

 * *Files identical despite different names*

### Comparing `sparseqr-1.2/test/test.py` & `sparseqr-1.2.1/test/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,35 +21,46 @@
 # Solve an overdetermined linear system  A x = b  in the least-squares sense
 #
 # The same routine also works for the usual non-overdetermined case.
 #
 A = scipy.sparse.rand( 20, 10, density = 0.1 )  # 20 equations, 10 unknowns
 b = numpy.random.random(20)  # one RHS, dense, but could also have many (in shape (20,k))
 x = sparseqr.solve( A, b, tolerance = 0 )
+## Call `rz()`:
+sparseqr.rz( A, b, tolerance = 0 )
 
 # Solve a linear system  M x = B  via QR decomposition
 #
 # This approach is slow due to the explicit construction of Q, but may be
 # useful if a large number of systems need to be solved with the same M.
 #
 M = scipy.sparse.rand( 10, 10, density = 0.1 )
 Q, R, E, rank = sparseqr.qr( M )
 r = rank  # r could be min(M.shape) if M is full-rank
 
 # The system is only solvable if the lower part of Q.T @ B is all zero:
 print( "System is solvable if this is zero (unlikely for a random matrix):", abs( (( Q.tocsc()[:,r:] ).T ).dot( B ) ).sum() )
 
+# Systems with large non-square matrices can benefit from "economy" decomposition.
+M = scipy.sparse.rand( 20, 5, density=0.1 )
+B = scipy.sparse.rand( 20, 5, density = 0.1 )
+Q, R, E, rank = sparseqr.qr( M )
+print("Q shape (should be 20x20):", Q.shape)
+print("R shape (should be 20x5):", R.shape)
+Q, R, E, rank = sparseqr.qr( M, economy=True )
+print("Q shape (should be 20x5):", Q.shape)
+print("R shape (should be 5x5):", R.shape)
+
 # Use CSC format for fast indexing of columns.
 R = R.tocsc()[:r,:r]
 Q = Q.tocsc()[:,:r]
 QB = (Q.T).dot(B).tocsc()  # for best performance, spsolve() wants the RHS to be in CSC format.
 result = scipy.sparse.linalg.spsolve(R, QB)
 
 # Recover a solution (as a dense array):
 x = numpy.zeros( ( M.shape[1], B.shape[1] ), dtype = result.dtype )
 x[:r] = result.todense()
 x[E] = x.copy()
 
 # Recover a solution (as a sparse matrix):
 x = scipy.sparse.vstack( ( result.tocoo(), scipy.sparse.coo_matrix( ( M.shape[1] - rank, B.shape[1] ), dtype = result.dtype ) ) )
 x.row = E[ x.row ]
-
```

### Comparing `sparseqr-1.2/PKG-INFO` & `sparseqr-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sparseqr
-Version: 1.2
+Version: 1.2.1
 Summary: Python wrapper for SuiteSparseQR
 License: Public Domain CC0
 Author: Yotam Gingold
 Author-email: yotam@yotamgingold.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cffi (>=1.0,<2.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: scipy (>=1.0,<2.0)
```

