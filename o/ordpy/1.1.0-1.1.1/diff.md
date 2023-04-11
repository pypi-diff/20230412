# Comparing `tmp/ordpy-1.1.0.tar.gz` & `tmp/ordpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ordpy-1.1.0.tar", last modified: Mon Jan  9 15:54:10 2023, max compression
+gzip compressed data, was "ordpy-1.1.1.tar", last modified: Tue Apr 11 22:51:24 2023, max compression
```

## Comparing `ordpy-1.1.0.tar` & `ordpy-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-01-09 15:54:10.473414 ordpy-1.1.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1098 2023-01-09 15:37:59.000000 ordpy-1.1.0/LICENSE
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    11299 2023-01-09 15:54:10.473414 ordpy-1.1.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    10753 2023-01-09 15:37:59.000000 ordpy-1.1.0/README.rst
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-01-09 15:54:10.473414 ordpy-1.1.0/ordpy/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-01-09 15:37:59.000000 ordpy-1.1.0/ordpy/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    95933 2023-01-09 15:37:59.000000 ordpy-1.1.0/ordpy/ordpy.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-01-09 15:54:10.473414 ordpy-1.1.0/ordpy.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    11299 2023-01-09 15:54:10.000000 ordpy-1.1.0/ordpy.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      201 2023-01-09 15:54:10.000000 ordpy-1.1.0/ordpy.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-01-09 15:54:10.000000 ordpy-1.1.0/ordpy.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        6 2023-01-09 15:54:10.000000 ordpy-1.1.0/ordpy.egg-info/top_level.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      125 2023-01-09 15:38:24.000000 ordpy-1.1.0/pyproject.toml
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      588 2023-01-09 15:54:10.473414 ordpy-1.1.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1310 2023-01-09 15:37:59.000000 ordpy-1.1.0/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-11 22:51:24.334302 ordpy-1.1.1/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1098 2023-01-09 15:37:59.000000 ordpy-1.1.1/LICENSE
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    11305 2023-04-11 22:51:24.334302 ordpy-1.1.1/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    10760 2023-04-11 22:32:54.000000 ordpy-1.1.1/README.rst
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-11 22:51:24.334302 ordpy-1.1.1/ordpy/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-01-09 15:37:59.000000 ordpy-1.1.1/ordpy/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    95644 2023-04-11 22:23:00.000000 ordpy-1.1.1/ordpy/ordpy.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-11 22:51:24.334302 ordpy-1.1.1/ordpy.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    11305 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      201 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        6 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      123 2023-04-11 22:22:56.000000 ordpy-1.1.1/pyproject.toml
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      588 2023-04-11 22:51:24.334302 ordpy-1.1.1/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1310 2023-04-11 22:37:31.000000 ordpy-1.1.1/setup.py
```

### Comparing `ordpy-1.1.0/LICENSE` & `ordpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ordpy-1.1.0/PKG-INFO` & `ordpy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for data analysis with permutation entropy and ordinal networks methods.
 Home-page: https://github.com/arthurpessa/ordpy
 Author: Arthur A. B. Pessa and Haroldo V. Ribeiro
 Author-email: arthur_pessa@hotmail.com, hvr@dfi.uem.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -283,12 +283,12 @@
    Contrasting chaos with noise via local versus global 
    information quantifiers. Physics Letters A, 376, 1577–1583.
 
 .. [#zunino2022] Zunino L., Olivares, F., Ribeiro H. V. & Rosso, O. A. (2022). 
    Permutation Jensen-Shannon distance: A versatile and fast symbolic tool
    for complex time-series analysis. Physical Review E, 105, 045310.
 
-.. [#bandt] Bandt, C. (2022). Statistics and modelling of order patterns in
-   univariate series. arXiv:2212.14386.
+.. [#bandt] Bandt, C. (2023). Statistics and contrasts of order patterns in
+   univariate time series, Chaos, 33, 033124.
 
 .. [#bandt_wittfeld] Bandt, C., & Wittfeld, K. (2022). Two new parameters for 
    the ordinal analysis of images. arXiv:2212.14643.
```

### Comparing `ordpy-1.1.0/README.rst` & `ordpy-1.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -269,12 +269,12 @@
    Contrasting chaos with noise via local versus global 
    information quantifiers. Physics Letters A, 376, 1577–1583.
 
 .. [#zunino2022] Zunino L., Olivares, F., Ribeiro H. V. & Rosso, O. A. (2022). 
    Permutation Jensen-Shannon distance: A versatile and fast symbolic tool
    for complex time-series analysis. Physical Review E, 105, 045310.
 
-.. [#bandt] Bandt, C. (2022). Statistics and modelling of order patterns in
-   univariate series. arXiv:2212.14386.
+.. [#bandt] Bandt, C. (2023). Statistics and contrasts of order patterns in
+   univariate time series, Chaos, 33, 033124.
 
 .. [#bandt_wittfeld] Bandt, C., & Wittfeld, K. (2022). Two new parameters for 
-   the ordinal analysis of images. arXiv:2212.14643.
+   the ordinal analysis of images. arXiv:2212.14643.
```

### Comparing `ordpy-1.1.0/ordpy/ordpy.py` & `ordpy-1.1.1/ordpy/ordpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
    Contrasting chaos with noise via local versus global 
    information quantifiers. Physics Letters A, 376, 1577–1583.
 
 .. [#zunino2022] Zunino L., Olivares, F., Ribeiro H. V. & Rosso, O. A. (2022). 
    Permutation Jensen-Shannon distance: A versatile and fast symbolic tool
    for complex time-series analysis. Physical Review E, 105, 045310.
 
-.. [#bandt] Bandt, C. (2022). Statistics and modelling of order patterns in
-   univariate series. arXiv:2212.14386.
+.. [#bandt] Bandt, C. (2023). Statistics and contrasts of order patterns in
+   univariate time series, Chaos, 33, 033124.
 
 .. [#bandt_wittfeld] Bandt, C., & Wittfeld, K. (2022). Two new parameters for 
    the ordinal analysis of images. arXiv:2212.14643.
 
 .. [#rosso_curvas] Martin, M. T., Plastino, A., & Rosso, O. A. (2006). 
    Generalized Statistical Complexity Measures: Geometrical and 
    Analytical Properties, Physica A, 369, 439–462.
@@ -382,15 +382,15 @@
                 ]
             )            
         symbols = np.apply_along_axis(np.argsort, 2, partitions)
     
     return symbols
 
 
-def ordinal_distribution(data, dx=3, dy=1, taux=1, tauy=1, return_missing=False, tie_precision=None):
+def ordinal_distribution(data, dx=3, dy=1, taux=1, tauy=1, return_missing=False, tie_precision=None, ordered=False):
     """
     Applies the Bandt and Pompe\\ [#bandt_pompe]_ symbolization approach to obtain 
     a probability distribution of ordinal patterns (permutations) from data.
     
     Parameters
     ----------
     data : array 
@@ -409,20 +409,23 @@
     return_missing: boolean
                     If `True`, it returns ordinal patterns not appearing in the 
                     symbolic sequence obtained from **data**. If `False`, these
                     missing patterns (permutations) are omitted (default: `False`).
     tie_precision : None, int
                     If not `None`, **data** is rounded with `tie_precision`
                     decimal numbers (default: `None`).
+    ordered: boolean
+                    If `True`, it returns ordinal patterns not appearing in the 
+                    symbolic sequence obtained from **data**. If `False`, these
+                    missing patterns (permutations) are omitted (default: `False`).
     Returns
     -------
      : tuple
        Tuple containing two arrays, one with the ordinal patterns occurring in data 
        and another with their corresponding probabilities.
-
     Examples
     --------
     >>> ordinal_distribution([4,7,9,10,6,11,3], dx=2)
     (array([[0, 1],
             [1, 0]]),
      array([0.66666667, 0.33333333]))
     >>>
@@ -446,33 +449,30 @@
             [0, 2, 1, 3],
             [1, 3, 2, 0]]),
      array([0.5 , 0.25, 0.25]))
     """
     def setdiff(a, b):
         """
         Searches for elements (subarrays) in `a` that are not contained in `b` [*]_. 
-
         Parameters
         ----------    
         a : tuples, lists or arrays
             Array in the format :math:`[[x_{21}, x_{22}, x_{23}, \\ldots, x_{2m}], 
             \\ldots, [x_{n1}, x_{n2}, x_{n3}, ..., x_{nm}]]`.
         b : tuples, lists or arrays
             Array in the format :math:`[[x_{21}, x_{22}, x_{23}, \\ldots, x_{2m}], 
             \\ldots, [x_{n1}, x_{n2}, x_{n3}, ..., x_{nm}]]`.
         
         Returns
         -------
         : array
             An array containing the elements in `a` that are not contained in `b`.
-
         Notes
         -----
         .. [*] This function was adapted from https://stackoverflow.com/questions/8317022/get-intersecting-rows-across-two-2d-numpy-arrays
-
         Examples
         --------
         >>> a = ((0,1,2), (0,1,2), (1,0,2), (2,0,1))
         >>> b = [[0,2,1], [0,1,2], [0,1,2]] 
         >>> setdiff(a, b)
         array([[1, 0, 2],
             [2, 0, 1]])
@@ -496,24 +496,40 @@
         symbols = symbols.reshape(-1, dx*dy) #we reshape the symbols array to facilitate the application of np.unique below.
     else:
         pass
     
     symbols, symbols_count = np.unique(symbols, return_counts=True, axis=0)
     probabilities          = symbols_count/symbols_count.sum()
 
+    
     if return_missing==False:
         return symbols, probabilities
     
     else:
-        all_symbols   = np.asarray(list(itertools.permutations(range(dx*dy))), dtype='int')
-        miss_symbols  = setdiff(all_symbols, symbols)
-        symbols       = np.concatenate((symbols, miss_symbols)).astype('int')
-        probabilities = np.concatenate((probabilities, np.zeros(miss_symbols.__len__())))
-        
-        return symbols, probabilities
+        if len(probabilities)==np.math.factorial(dx*dy):
+            return symbols, probabilities
+        else:
+            if ordered==True:
+                all_symbols           = np.asarray(list(itertools.permutations(range(dx*dy))), dtype='int')
+                all_probs             = np.full(math.factorial(dx*dy), 0.)
+
+                _, ncols              = all_symbols.shape
+                dtype                 = {'names':['f{}'.format(i) for i in range(ncols)], 'formats': ncols*[all_symbols.dtype]}
+                logifilter            = np.isin(all_symbols.view(dtype), symbols.view(dtype)).flatten()
+                all_probs[logifilter] = probabilities 
+                
+                return all_symbols, all_probs
+            
+            else:
+                all_symbols   = np.asarray(list(itertools.permutations(range(dx*dy))), dtype='int')
+                miss_symbols  = setdiff(all_symbols, symbols)
+                symbols       = np.concatenate((symbols, miss_symbols)).astype('int')
+                probabilities = np.concatenate((probabilities, np.zeros(miss_symbols.__len__())))
+
+                return symbols, probabilities
 
 
 def permutation_entropy(data, dx=3, dy=1, taux=1, tauy=1, base=2, normalized=True, probs=False, tie_precision=None):
     """
     Calculates the Shannon entropy using an ordinal distribution obtained from
     data\\ [#bandt_pompe]_\\ :sup:`,`\\ [#ribeiro_2012]_.
     
@@ -2148,20 +2164,18 @@
     probs : boolean
             If `True`, it assumes **data** is an ordinal probability distribution.
             If `False`, **data** is expected to be a one- or two-dimensional array
             (default: `False`). 
     tie_precision : None, int
                     If not `None`, **data** is rounded with `tie_precision`
                     decimal numbers (default: `None`).
-
     Returns
     -------
      : tuple
        Values of normalized permutation entropy and Fisher information.
-
     Examples
     --------
     >>> fisher_shannon([4,7,9,10,6,11,3], dx=2)
     (0.9182958340544896, 0.028595479208968325)
     >>>
     >>> p = ordinal_distribution([4,7,9,10,6,11,3], dx=2, return_missing=True)[1]
     >>> fisher_shannon(p, dx=2, probs=True)
@@ -2176,46 +2190,35 @@
     >>> fisher_shannon([[1,2,1,4],[8,3,4,5],[6,7,5,6]], dx=3, dy=2)
     (0.2107070115500801, 1.0)    
     """  
     if not probs:
         if dx*dy>10:
             warnings.warn("Large values of embedding dimension may lead to memory allocation problems.")                
         else: pass
-        
-        symbols, probabilities = ordinal_distribution(data, dx, dy, taux, tauy, return_missing=False, tie_precision=tie_precision)
-        h                      = permutation_entropy(probabilities, dx, dy, taux, tauy, probs=True, tie_precision=tie_precision)        
-        
+      
+        symbols, probabilities = ordinal_distribution(data, dx, dy, taux, tauy, return_missing=True, tie_precision=tie_precision, ordered=True)
+
         #In case not all possible permutations occur in **data**, we assign zero probability the non-occurring states. 
         #This is necessary to calculate the Fisher information measure
         if (probabilities==1.).sum()==1.:
-            return h, 1.
-        elif len(probabilities)==dx*dy:
-            all_probs = probabilities
-        else:
-            all_symbols           = np.asarray(list(itertools.permutations(range(dx*dy))), dtype='int')
-            all_probs             = np.full(math.factorial(dx*dy), 0.)
-
-            _, ncols              = all_symbols.shape
-            dtype                 = {'names':['f{}'.format(i) for i in range(ncols)], 'formats': ncols*[all_symbols.dtype]}
-            logifilter            = np.isin(all_symbols.view(dtype), symbols.view(dtype)).flatten()
-            all_probs[logifilter] = probabilities            
-
+            return 0., 1.
+        else: 
+            h = permutation_entropy(probabilities, dx, dy, taux, tauy, probs=True, tie_precision=tie_precision)
     else:
         warnings.warn("Be mindful the correct calculation of Fisher information depends on all possible permutations " + 
                       "given the embedding dimensions dx and dy, not only on the permutations occurring in data.")
 
-        all_probs = np.asarray(data)
-        h         = permutation_entropy(all_probs, dx, dy, taux, tauy, probs=True, tie_precision=tie_precision)
+        if (probabilities==1.).sum()==1.:
+            return 0., 1.
+        else:
+            h = permutation_entropy(probabilities, dx, dy, taux, tauy, probs=True, tie_precision=tie_precision)
         
-        if (all_probs==1.).sum()==1.:
-            return h, 1.
-
-    return h, np.sum(np.diff(np.sqrt(all_probs[::-1]))**2.)/2  #F = F_0 \sum_{i = 1}^{N - 1} (\sqrt{p_{i+1}} - \sqrt{p_{i}})^2, with F_0=1/2
-
+    return h, np.sum(np.diff(np.sqrt(probabilities[::-1]))**2.)/2  #F = F_0 \sum_{i = 1}^{N - 1} (\sqrt{p_{i+1}} - \sqrt{p_{i}})^2, with F_0=1/2
     
+   
 def permutation_js_distance(data, dx=3, dy=1, taux=1, tauy=1, base='e', normalized=True, tie_precision=None):
     """
     Calculates the permutation Jensen-Shannon distance\\ [#zunino2022]_ between 
     multiple time series (or channels of a multivariate time series) or 
     multiple matrices (images) using ordinal distributions obtained from data.
     
     Parameters
@@ -2267,36 +2270,33 @@
     else: pass
     
     logfunc                         = np.log if base=="e" else np.log2
     num_of_channels                 = len(data)
     sum_of_entropies, probabilities = 0., []
 
     for channel_ in data:
-        symbols, probs     = ordinal_distribution(channel_, dx=dx, dy=dy, taux=taux, tauy=tauy, return_missing=True, tie_precision=tie_precision)
+        symbols, probs    = ordinal_distribution(channel_, dx=dx, dy=dy, taux=taux, tauy=tauy, return_missing=True, tie_precision=tie_precision, ordered=True)
 
-        symbols_as_strings = np.apply_along_axis(np.array2string, 1, symbols, separator='')
-        mask_probs         = np.apply_along_axis(np.argsort,      0, symbols_as_strings)
-
-        probabilities.append(probs[mask_probs])
-        sum_of_entropies  += -np.sum(probs[probs>0]*logfunc(probs[probs>0]))/num_of_channels
+        probabilities.append(probs)
+        sum_of_entropies += -np.sum(probs[probs>0]*logfunc(probs[probs>0]))/num_of_channels
 
     sum_of_distros = np.sum(probabilities, axis=0)/num_of_channels
     entropy_of_sum = -np.sum(sum_of_distros[sum_of_distros>0]*logfunc(sum_of_distros[sum_of_distros>0]))
     distance       = entropy_of_sum - sum_of_entropies
     is_it_nan      = np.isnan(np.sqrt(distance))        
 
     if is_it_nan==True or num_of_channels==1: #added `is_it_nan` after having problems calculating the square root of very small negative numbers caused by floating-point representation problems in Python.
         return 0                              #the second boolean check basically covers the case only one series is provided.
     else:
         if normalized==True:
             return np.sqrt(distance/logfunc(num_of_channels))
         else:
             return np.sqrt(distance)
 
-
+         
 def permutation_contrasts(data, taux=1, tie_precision=None):
     """
     Calculates the four pattern (permutation) contrasts [#bandt]_ 
     of a time series (with dx=3) using an ordinal distribution 
     obtained from data.
     
     Parameters
@@ -2327,34 +2327,31 @@
     >>>
     >>> permutation_contrasts([5,2,3,4,2,7,4])
     (0.2, 0.2, 0.0, 0.0)
     >>>
     >>> permutation_contrasts([5, 2, 3, 4, 2, 7, 4], taux=2)
     (0.0, 0.666, 0.333, 0.333)
     """
-    dict_symbols = dict([('[012]', 0),('[021]', 1),('[102]', 2),
-                         ('[120]', 3),('[201]', 4),('[210]', 5)])
+    dict_symbols = dict([('[012]', 0),('[021]', 1),('[102]', 2), ('[120]', 3),('[201]', 4),('[210]', 5)])
     
     symbols                = ordinal_sequence(data, dx=3, dy=1, taux=taux, tauy=1, overlapping=True, tie_precision=tie_precision)
     symbols, symbols_count = np.unique(symbols, return_counts=True, axis=0)
     probabilities          = symbols_count/symbols_count.sum()
-    symbols                = np.apply_along_axis(np.argsort, 1, symbols) #sort the permutations once again so they correspond to the ones used by Bandt and Wittfeld.
 
-
-    symbols         = np.apply_along_axis(np.array2string, 1, symbols, separator='')
-    indices         = np.fromiter(map(dict_symbols.get, symbols), dtype='int')
-    all_probs       = np.fromiter((probabilities[np.argwhere(indices==type_).flatten()].sum() for type_ in range(6)), dtype='float')            
-
-    up_down_balance = all_probs[0] - all_probs[5] #p012 - p210
-    persistence     = all_probs[0] + all_probs[5] #p012 + p210
-    rot_asymetry    = all_probs[2] + all_probs[3] - all_probs[1] - all_probs[4] #p102 + p120 - p021 - p201
-    updown_scaling  = all_probs[1] + all_probs[2] - all_probs[3] - all_probs[4] #p021 + p102 - p120 - p201
+    symbols                            = np.apply_along_axis(np.array2string, 1, symbols, separator='')
+    indices                            = np.fromiter(map(dict_symbols.get, symbols), dtype='int')
+    p123, p132, p213, p312, p231, p321 = np.fromiter((probabilities[np.argwhere(indices==type_).flatten()].sum() for type_ in range(6)), dtype='float')            
+
+    up_down_balance = p123 - p321
+    persistence     = p123 + p321
+    rot_asymmetry   = p213 + p231 - p132 - p312
+    updown_scaling  = p132 + p213 - p231 - p312
     
-    return up_down_balance, persistence, rot_asymetry, updown_scaling
-
+    return up_down_balance, persistence, rot_asymmetry, updown_scaling
+   
 
 def smoothness_structure(data, taux=1, tauy=1, tie_precision=None):
     """
     Calculates the smoothness and curve structure\\ [#bandt_wittfeld]_ 
     of an image (with embedding parameters dx=dy=2) using an ordinal
     distribution obtained from data.
     
@@ -2384,27 +2381,26 @@
     >>>
     >>> smoothness_structure([[1,2,1,4],[8,3,4,5],[6,7,5,6]], taux=2, tauy=1)
     (-0.0833, 0.75)
     >>>
     >>> smoothness_structure([[1,2,1,4],[8,3,4,5],[6,7,5,6]], taux=2, tauy=2)
     (-0.333, 1.0)
     """
-    #These permutations correspond to a different sorting process laid out in the paper by Bandt and Wittfeld
-    dict_types  = dict([('[0123]', 0),('[0132]', 1),('[0213]', 0),('[0231]', 2),
-                        ('[0312]', 1),('[0321]', 2),('[1023]', 1),('[1032]', 0),
-                        ('[1203]', 1),('[1230]', 2),('[1302]', 0),('[1320]', 2),
-                        ('[2013]', 2),('[2031]', 0),('[2103]', 2),('[2130]', 1),
-                        ('[2301]', 0),('[2310]', 1),('[3012]', 2),('[3021]', 1),
-                        ('[3102]', 2),('[3120]', 0),('[3201]', 1),('[3210]', 0)])
+
+    dict_types  = dict([('[0123]', 0),('[0132]', 1),('[0213]', 0),('[0231]', 1),
+                        ('[0312]', 2),('[0321]', 2),('[1023]', 1),('[1032]', 0),
+                        ('[1203]', 2),('[1230]', 2),('[1302]', 0),('[1320]', 1),
+                        ('[2013]', 1),('[2031]', 0),('[2103]', 2),('[2130]', 2),
+                        ('[2301]', 0),('[2310]', 1),('[3012]', 2),('[3021]', 2),
+                        ('[3102]', 1),('[3120]', 0),('[3201]', 1),('[3210]', 0)])
 
     symbols                = ordinal_sequence(data, dx=2, dy=2, taux=taux, tauy=tauy, overlapping=True, tie_precision=tie_precision)
     symbols                = symbols.reshape(-1, 4) #reshape the symbols array to facilitate the application of np.unique below
     symbols, symbols_count = np.unique(symbols, return_counts=True, axis=0)
     probabilities          = symbols_count/symbols_count.sum()
-    symbols                = np.apply_along_axis(np.argsort, 1, symbols) #resort the permutations so they correspond to the ones used by Bandt and Wittfeld.
 
     probs_types = np.full(shape=3, fill_value=0.)
     symbols     = np.apply_along_axis(np.array2string, 1, symbols, separator='')
     indices     = np.fromiter(map(dict_types.get, symbols), dtype='int')
     probs_types = np.fromiter((probabilities[np.argwhere(indices==type_).flatten()].sum() for type_ in range(3)), dtype='float')
 
     smoothness  = probs_types[0] - 1/3
```

### Comparing `ordpy-1.1.0/ordpy.egg-info/PKG-INFO` & `ordpy-1.1.1/ordpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for data analysis with permutation entropy and ordinal networks methods.
 Home-page: https://github.com/arthurpessa/ordpy
 Author: Arthur A. B. Pessa and Haroldo V. Ribeiro
 Author-email: arthur_pessa@hotmail.com, hvr@dfi.uem.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -283,12 +283,12 @@
    Contrasting chaos with noise via local versus global 
    information quantifiers. Physics Letters A, 376, 1577–1583.
 
 .. [#zunino2022] Zunino L., Olivares, F., Ribeiro H. V. & Rosso, O. A. (2022). 
    Permutation Jensen-Shannon distance: A versatile and fast symbolic tool
    for complex time-series analysis. Physical Review E, 105, 045310.
 
-.. [#bandt] Bandt, C. (2022). Statistics and modelling of order patterns in
-   univariate series. arXiv:2212.14386.
+.. [#bandt] Bandt, C. (2023). Statistics and contrasts of order patterns in
+   univariate time series, Chaos, 33, 033124.
 
 .. [#bandt_wittfeld] Bandt, C., & Wittfeld, K. (2022). Two new parameters for 
    the ordinal analysis of images. arXiv:2212.14643.
```

### Comparing `ordpy-1.1.0/setup.cfg` & `ordpy-1.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ordpy
-version = 1.1.0
+version = 1.1.1
 url = https://github.com/arthurpessa/ordpy
 author = Arthur A. B. Pessa and Haroldo V. Ribeiro
 author_email = arthur_pessa@hotmail.com, hvr@uem.dfi.br
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `ordpy-1.1.0/setup.py` & `ordpy-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ordpy",
-    version="1.1.0",
+    version="1.1.1",
     author="Arthur A. B. Pessa and Haroldo V. Ribeiro",
     author_email="arthur_pessa@hotmail.com, hvr@dfi.uem.br",
     description="A Python package for data analysis with permutation entropy and ordinal networks methods.",
     long_description=long_description,
     long_description_content_type="text/x-rst; charset=UTF-8",
     url="https://github.com/arthurpessa/ordpy",
     packages=setuptools.find_packages(),
```

