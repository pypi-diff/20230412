# Comparing `tmp/richvalues-3.0.8.tar.gz` & `tmp/richvalues-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.8.tar", last modified: Tue Apr 11 15:18:01 2023, max compression
+gzip compressed data, was "richvalues-3.0.9.tar", last modified: Tue Apr 11 22:48:32 2023, max compression
```

## Comparing `richvalues-3.0.8.tar` & `richvalues-3.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 15:18:01.312888 richvalues-3.0.8/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 15:18:01.312888 richvalues-3.0.8/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.8/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 15:17:56.000000 richvalues-3.0.8/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 15:18:01.308888 richvalues-3.0.8/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   146269 2023-04-11 15:16:45.000000 richvalues-3.0.8/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 15:18:01.312888 richvalues-3.0.8/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 15:18:01.312888 richvalues-3.0.8/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 15:17:43.000000 richvalues-3.0.8/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 22:48:32.340209 richvalues-3.0.9/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 22:48:32.340209 richvalues-3.0.9/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.9/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 22:47:59.000000 richvalues-3.0.9/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 22:48:32.336209 richvalues-3.0.9/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   146680 2023-04-11 22:48:24.000000 richvalues-3.0.9/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 22:48:32.336209 richvalues-3.0.9/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 22:48:32.340209 richvalues-3.0.9/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 22:47:54.000000 richvalues-3.0.9/setup.py
```

### Comparing `richvalues-3.0.8/PKG-INFO` & `richvalues-3.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.8/README.md` & `richvalues-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.8/pyproject.toml` & `richvalues-3.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.8"
+version = "3.0.9"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-3.0.8/richvalues/__init__.py` & `richvalues-3.0.9/richvalues/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.0.8'
+__version__ = '3.0.9'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
@@ -748,30 +748,40 @@
             text = (str(main).replace('NaN','nan').replace('nan','...')
                     .replace('inf','$\infty$'))
         if not dollars:
             text = text.replace('$','')
         return text
    
     def __abs__(self):
-        main = copy.copy(self.main)
-        unc = copy.copy(self.unc)
+        sigmas = defaultparams['sigmas to use approximate '
+                       + 'uncertainty propagation']
+        x = copy.copy(self.main)
+        dx = copy.copy(self.unc)
         domain = copy.copy(self.domain)
-        if not self.is_interv:
-            x = abs(main)
+        x1, x2 = self.interval(sigmas=np.inf)
+        if all(np.array([x1, x2]) >= 0):
+            if (self.is_centr and self.prop_score > sigmas) or self.is_interv:
+                new_rval = self
+            else:
+                new_rval = self.function(lambda x: abs(x), domain=domain)
+        elif all(np.array([x1, x2]) <= 0):
+            new_rval = -self
         else:
-            x1, x2 = self.interval()
-            x1, x2 = abs(x1), abs(x2)
-            x = [min(x1, x2), max(x1, x2)]
-        dx = np.abs(unc)
-        domain = [abs(domain[0]), abs(domain[1])]
-        domain = [min(domain), max(domain)]
-        if np.isinf(domain[0]):
             domain[0] = 0
-        new_rval = RichValue(x, dx, domain=domain)
-        new_rval.vars = self.vars
+            if self.is_centr:
+                if self.prop_score > sigmas:
+                    x = abs(x)
+                    new_rval = RichValue(x, dx, domain=domain)
+                else:
+                    new_rval = self.function(lambda x: abs(x), domain=domain)
+            else:
+                x2 = max(np.abs([x1, x2]))
+                x1 = 0
+                new_rval = RichValue([x1, x2], dx, domain=domain)
+        new_rval.domain[0] = max(0, new_rval.domain[0])
         new_rval.expression = 'abs({})'.format(self.expression)
         return new_rval
    
     def __neg__(self):
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         domain = copy.copy(self.domain)
@@ -1188,15 +1198,15 @@
     
     @property
     def minimum_exponent_for_scientific_notation(self): return self.min_exp
     @minimum_exponent_for_scientific_notation.setter
     def minimum_exponent_for_scientific_notation(self, x): self.min_exp = x
     
     @property
-    def variables(self): return self.variable
+    def variables(self): return self.vars
     @variables.setter
     def variables(self, x): self.vars = x
     
     # Attribute acronyms.
     is_limit = is_lim
     is_interval = is_interv
     is_centered_value = is_centr
@@ -1514,58 +1524,43 @@
             'df = pd.DataFrame(data, self.index, self.columns)']
         code = '\n'.join(code)
         output = {}
         exec(code, {**{'self': self}, **globals()}, output)
         return output['df']
 
     @property    
-    def mains(self):
-        return self._attribute('mains')
+    def mains(self): return self._attribute('mains')
     @property
-    def uncs(self):
-        return self._attribute2('uncs')
+    def uncs(self): return self._attribute2('uncs')
     @property
-    def are_lolims(self):
-        return self._attribute('are_lolims')
+    def are_lolims(self): return self._attribute('are_lolims')
     @property
-    def are_uplims(self):
-        return self._attribute('are_uplims')
+    def are_uplims(self): return self._attribute('are_uplims')
     @property
-    def are_ranges(self):
-        return self._attribute('are_ranges')
+    def are_ranges(self): return self._attribute('are_ranges')
     @property
-    def domains(self):
-        return self._attribute2('domains')
+    def domains(self): return self._attribute2('domains')
     @property
-    def are_lims(self):
-        return self._attribute('are_lims')
+    def are_lims(self): return self._attribute('are_lims')
     @property
-    def are_intervs(self):
-        return self._attribute('are_intervs')
+    def are_intervs(self): return self._attribute('are_intervs')
     @property
-    def are_centrs(self):
-        return self._attribute('are_centrs')
+    def are_centrs(self): return self._attribute('are_centrs')
     @property
-    def rel_uncs(self):
-        return self._attribute2('rel_uncs')
+    def rel_uncs(self): return self._attribute2('rel_uncs')
     @property
-    def signals_noises(self):
-        return self._attribute2('signal_noises')
+    def signals_noises(self): return self._attribute2('signal_noises')
     @property
-    def ampls(self):
-        return self._attribute2('ampls')
+    def ampls(self): return self._attribute2('ampls')
     @property
-    def rel_ampls(self):
-        return self._attribute2('rel_ampls')
+    def rel_ampls(self): return self._attribute2('rel_ampls')
     @property
-    def norm_uncs(self):
-        return self._attribute2('norm_uncs')
+    def norm_uncs(self): return self._attribute2('norm_uncs')
     @property
-    def prop_scores(self):
-        return self._attribute('prop_scores')
+    def prop_scores(self): return self._attribute('prop_scores')
 
     def intervals(self):
         return self._attribute2('intervals')
     
     def flatten_attribute_output(self, attribute):
         """Separate the list elements from the output of the given attribute."""
         df = eval('self.{}'.format(attribute))
@@ -3637,8 +3632,8 @@
 function = function_with_rich_values
 array_function = function_with_rich_arrays
 distribution = distr_with_rich_values
 evaluate_distribution = evaluate_distr
 center_and_uncertainties = center_and_uncs
 is_not_a_number = is_nan = isnan
 is_infinite = is_inf = isinf
-is_finite = is_finite = isfinite
+is_finite = is_finite = isfinite
```

### Comparing `richvalues-3.0.8/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.9/richvalues.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.8/setup.py` & `richvalues-3.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.8',
+    version = '3.0.9',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues',
```

