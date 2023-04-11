# Comparing `tmp/sarabande-0.4.0.tar.gz` & `tmp/sarabande-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarabande-0.4.0.tar", last modified: Mon Apr  3 21:27:40 2023, max compression
+gzip compressed data, was "sarabande-0.5.0.tar", last modified: Tue Apr  4 14:32:58 2023, max compression
```

## Comparing `sarabande-0.4.0.tar` & `sarabande-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-03 21:27:40.951758 sarabande-0.4.0/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2023-04-03 19:32:46.000000 sarabande-0.4.0/LICENSE
--rw-r--r--   0 jamessunseri   (501) staff       (20)      106 2023-04-03 19:32:46.000000 sarabande-0.4.0/MANIFEST.in
--rw-r--r--   0 jamessunseri   (501) staff       (20)     5581 2023-04-03 21:27:40.951864 sarabande-0.4.0/PKG-INFO
--rw-r--r--   0 jamessunseri   (501) staff       (20)     4389 2023-04-03 19:32:46.000000 sarabande-0.4.0/README.md
--rw-r--r--   0 jamessunseri   (501) staff       (20)      116 2023-04-03 19:32:46.000000 sarabande-0.4.0/pyproject.toml
--rw-r--r--   0 jamessunseri   (501) staff       (20)       12 2023-04-03 19:32:46.000000 sarabande-0.4.0/requirements.txt
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-03 21:27:40.950863 sarabande-0.4.0/sarabande/
--rw-r--r--   0 jamessunseri   (501) staff       (20)  2300096 2023-04-03 19:32:46.000000 sarabande-0.4.0/sarabande/CG_Coeffs.npy
--rw-r--r--   0 jamessunseri   (501) staff       (20)      151 2023-04-03 19:32:46.000000 sarabande-0.4.0/sarabande/__init__.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     3080 2023-04-03 19:32:46.000000 sarabande-0.4.0/sarabande/boot_up.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)    20271 2023-04-03 19:52:32.000000 sarabande-0.4.0/sarabande/calc_PCF.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     8432 2023-04-03 19:32:46.000000 sarabande-0.4.0/sarabande/main.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)    17256 2023-04-03 19:32:46.000000 sarabande-0.4.0/sarabande/utils.py
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-03 21:27:40.951647 sarabande-0.4.0/sarabande.egg-info/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     5581 2023-04-03 21:27:40.000000 sarabande-0.4.0/sarabande.egg-info/PKG-INFO
--rw-r--r--   0 jamessunseri   (501) staff       (20)      338 2023-04-03 21:27:40.000000 sarabande-0.4.0/sarabande.egg-info/SOURCES.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2023-04-03 21:27:40.000000 sarabande-0.4.0/sarabande.egg-info/dependency_links.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       10 2023-04-03 21:27:40.000000 sarabande-0.4.0/sarabande.egg-info/top_level.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2023-04-03 21:27:40.952124 sarabande-0.4.0/setup.cfg
--rw-r--r--   0 jamessunseri   (501) staff       (20)     2219 2023-04-03 19:45:12.000000 sarabande-0.4.0/setup.py
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-04 14:32:58.527683 sarabande-0.5.0/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2023-04-03 19:32:46.000000 sarabande-0.5.0/LICENSE
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      106 2023-04-03 19:32:46.000000 sarabande-0.5.0/MANIFEST.in
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     5581 2023-04-04 14:32:58.527764 sarabande-0.5.0/PKG-INFO
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     4389 2023-04-03 19:32:46.000000 sarabande-0.5.0/README.md
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      116 2023-04-03 19:32:46.000000 sarabande-0.5.0/pyproject.toml
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       12 2023-04-03 19:32:46.000000 sarabande-0.5.0/requirements.txt
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-04 14:32:58.526744 sarabande-0.5.0/sarabande/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)  2300096 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/CG_Coeffs.npy
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      151 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/__init__.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     3080 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/boot_up.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)    22357 2023-04-04 14:30:55.000000 sarabande-0.5.0/sarabande/calc_PCF.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     8432 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/main.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)    17256 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/utils.py
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-04 14:32:58.527565 sarabande-0.5.0/sarabande.egg-info/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     5581 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/PKG-INFO
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      338 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/SOURCES.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/dependency_links.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       10 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/top_level.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2023-04-04 14:32:58.527996 sarabande-0.5.0/setup.cfg
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     2219 2023-04-04 14:32:07.000000 sarabande-0.5.0/setup.py
```

### Comparing `sarabande-0.4.0/LICENSE` & `sarabande-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sarabande-0.4.0/PKG-INFO` & `sarabande-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarabande
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tool for measuring 3/4 PCFs on discrete periodic data.
 Home-page: https://github.com/James11222/sarabande/
 Author: James Sunseri
 Author-email: jamessunseri@berkeley.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/sarabande/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `sarabande-0.4.0/README.md` & `sarabande-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sarabande-0.4.0/sarabande/CG_Coeffs.npy` & `sarabande-0.5.0/sarabande/CG_Coeffs.npy`

 * *Files identical despite different names*

### Comparing `sarabande-0.4.0/sarabande/boot_up.py` & `sarabande-0.5.0/sarabande/boot_up.py`

 * *Files identical despite different names*

### Comparing `sarabande-0.4.0/sarabande/calc_PCF.py` & `sarabande-0.5.0/sarabande/calc_PCF.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from subprocess import call
 import time
 import pkg_resources
 import concurrent.futures
 from sarabande.utils import *
 
 def calc_zeta(measure_obj, verbose_flag=True, skip_prepare=False, parallelized=True, 
-              checking_install=False, calc_bin_overlaps=False, calc_odd_modes=False):
+              checking_install=False, calc_bin_overlaps=False, calc_odd_modes=False, calc_disconnected=False):
     """
     This function is where the core algorithms take place for measuring the 3/4 PCFs 
     either projected or not projected. In total there are 4 options
 
     - projected 3PCF        - projected 4PCF
     - full 3PCF             - full 4PCF
     
@@ -18,15 +18,16 @@
         measure_obj (class: measure): an object that carries the necessary values and data structures to compute 3/4 PCFs
         normalize (bool, optional): flag to determine whether we would like to normalize by the bin volume(s). Defaults to True.
         verbose_flag (bool, optional): flag to walk the user through the full calculation process. Defaults to True.
         skip_prepare (bool, optional): Flag to determine whether or not we should skip preparing the data (if you already ran the calculation). Defaults to False.
         parallelized (bool): when True the Full 4PCF is computed using a parallelized version of the algorithm. 
         We make this an optional flag because concurrent.futures in python is not the most reliable package across machines.
         calc_bin_overlaps (bool): A flag to determine whether any overlap bins should be computed (ex. any possibility where bi = bj (= bk))
-        calc_odd_modes (bool): A flag to determine if sarabande should calculate the odd modes where l1 + l2 + l3 is odd.
+        calc_odd_modes (bool): A flag to determine if we should calculate the odd modes where l1 + l2 + l3 is odd.
+        calc_disconnected (bool): a flag to determine if we should compute the disconnected piece of the 4PCF.
 
 
     Raises:
         AssertionError: in order to calculate the full 4PCF one has to save a boundsandnumber file (this comes from creating radial bins in one of the utility functions.)
 
     Returns:
         No Returns, instead we add the zeta attribute to the measure_obj.
@@ -276,15 +277,15 @@
                 return 1
 
             #mapping function
             global load_almb
             def load_almb(index_list):
                 l_1, l_2, l_3, m_1, m_2, m_3, b_1, b_2, b_3 = index_list
 
-                coupling_w = measure_obj.density_field_data * (-1)**(l_1 + l_2 + l_3) * CG_Coefficients[l_1,l_2,l_3,m_1,m_2,m_3]
+                coupling_phase = (-1)**(l_1 + l_2 + l_3) * CG_Coefficients[l_1,l_2,l_3,m_1,m_2,m_3]
 
                 if m_1 < 0:
                     a_lmb_1 = (-1)**m_1 * (np.load(measure_obj.save_dir + measure_obj.save_name+'conv_data_kernel_'+measure_obj.kernel_name+'_'+
                                                 str(l_1)+'_'+str(-m_1)+'_bin_'+str(b_1)+'.npy').astype(np.complex128)).conjugate()                                  
                 else:
                     a_lmb_1 = np.load(measure_obj.save_dir + measure_obj.save_name+'conv_data_kernel_'+measure_obj.kernel_name+'_'+str(l_1)+
                                                     '_'+str(m_1)+'_bin_'+str(b_1)+'.npy').astype(np.complex128)
@@ -295,25 +296,41 @@
                 else:
                     a_lmb_2 = np.load(measure_obj.save_dir + measure_obj.save_name+'conv_data_kernel_'+measure_obj.kernel_name+'_'+str(l_2)+
                                                         '_'+str(m_2)+'_bin_'+str(b_2)+'.npy').astype(np.complex128)
 
                 a_lmb_3 = np.load(measure_obj.save_dir + measure_obj.save_name+'conv_data_kernel_'+measure_obj.kernel_name+'_'+str(l_3)+
                                                         '_'+str(m_3)+'_bin_'+str(b_3)+'.npy').astype(np.complex128)
 
-                if calc_odd_modes == True:
-                    return [[l_1, l_2, l_3, b_1, b_2, b_3], np.sum(2 * S(m_3) * coupling_w * (a_lmb_1 * a_lmb_2 * a_lmb_3))]
+
+                
+
+                if calc_disconnected == True:
+                    disconnected_piece = 2 * S(m_3) * coupling_phase * (np.sum(measure_obj.density_field_data * a_lmb_1) * np.sum(a_lmb_2 * a_lmb_3)
+                                                                      + np.sum(measure_obj.density_field_data * a_lmb_2) * np.sum(a_lmb_3 * a_lmb_1) 
+                                                                      + np.sum(measure_obj.density_field_data * a_lmb_3) * np.sum(a_lmb_1 * a_lmb_2))
                 else:
-                    return [[l_1, l_2, l_3, b_1, b_2, b_3], np.sum(2 * S(m_3) * coupling_w * np.real(a_lmb_1 * a_lmb_2 * a_lmb_3))]
+                    disconnected_piece = 0
+
+                if calc_odd_modes == True and (l1 + l2 + l3)%2 != 0:
+                    full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * (a_lmb_1 * a_lmb_2 * a_lmb_3))
+                else:
+                    full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * np.real(a_lmb_1 * a_lmb_2 * a_lmb_3))
+                    disconnected_piece = np.real(disconnected_piece)
+                                                
+
+                
+                return [[l_1, l_2, l_3, b_1, b_2, b_3], full_piece, disconnected_piece]
 
             #initialize final storage array
             ell_max = measure_obj.ell_max
             nbins = measure_obj.nbins
             if hasattr(measure_obj, 'boundsandnumber') == False:
                 raise AssertionError("You need to run measure_obj.create_radial_bins() first!")
             zeta = np.zeros((ell_max+1, ell_max+1, ell_max+1,nbins, nbins, nbins)) + 0j
+            zeta_disconnected = np.zeros((ell_max+1, ell_max+1, ell_max+1,nbins, nbins, nbins)) + 0j
 
             #load in Modified Clebsch-Gordon Coefficients / Wigner-3j Coefficients + Phase
             stream = pkg_resources.resource_stream(__name__, 'CG_Coeffs.npy')
             CG_Coefficients = np.load(stream)
 
             #create a look up table for parallel mapping
             indeces = []
@@ -344,14 +361,15 @@
                 
             else:
                 results = list(map(load_almb, indeces))
 
             for j in range(len(results)):
                 l_1, l_2, l_3, b_1, b_2, b_3 = results[j][0]
                 zeta[l_1, l_2, l_3, b_1, b_2, b_3] += results[j][1] 
+                zeta_disconnected[l_1, l_2, l_3, b_1, b_2, b_3] += results[j][2] 
                     
 
             #----------------
             # Symmetrization
             #----------------
             for l1 in range(0,ell_max+1):
                 for l2 in range(0,ell_max+1):
@@ -364,28 +382,44 @@
                                     this_4pcf = zeta[l1,l2,l3,b1,b2,b3]
                                     zeta[l3,l1,l2,b3,b1,b2] = this_4pcf
                                     zeta[l2,l3,l1,b2,b3,b1] = this_4pcf
                                     zeta[l1,l3,l2,b1,b3,b2] = this_4pcf
                                     zeta[l2,l1,l3,b2,b1,b3] = this_4pcf
                                     zeta[l3,l2,l1,b3,b2,b1] = this_4pcf
 
+                                    if calc_disconnected == True:
+                                        this_4pcf_disconnected = zeta_disconnected[l1,l2,l3,b1,b2,b3]
+                                        zeta_disconnected[l3,l1,l2,b3,b1,b2] = this_4pcf_disconnected
+                                        zeta_disconnected[l2,l3,l1,b2,b3,b1] = this_4pcf_disconnected
+                                        zeta_disconnected[l1,l3,l2,b1,b3,b2] = this_4pcf_disconnected
+                                        zeta_disconnected[l2,l1,l3,b2,b1,b3] = this_4pcf_disconnected
+                                        zeta_disconnected[l3,l2,l1,b3,b2,b1] = this_4pcf_disconnected
+
+
+
             #---------------
             # Normalization
             #---------------
             if measure_obj.normalize:  
                 binvolume = measure_obj.boundsandnumber[1,0:nbins]
                 V_cell = (measure_obj.boxsize / measure_obj.ld_one_d)**3
                 bin_volumes = (binvolume[:,None, None] * binvolume[None,:, None] * binvolume[None, None, :]) * V_cell**3
                 normalize_coeff = 1 / (measure_obj.N_gal * bin_volumes * measure_obj.nbar**3) 
                 normed_zeta = zeta * normalize_coeff
                 measure_obj.zeta = normed_zeta
+
+                if calc_disconnected == True:
+                    normed_zeta_disconnected = zeta_disconnected * normalize_coeff
+                    measure_obj.zeta_disconnected = normed_zeta_disconnected
+
             else:
                 if checking_install == False: 
                     print("your zeta coefficients are not properly normalized.")
                 measure_obj.zeta = zeta  
+                measure_obj.zeta_disconnected = zeta_disconnected
 
             finish=time.time()
             if checking_install == False:
                 print("Finished Calculating 4PCF in {0:0.4f} seconds".format(finish-start))
 
         #------------
         #  Clean Up
```

### Comparing `sarabande-0.4.0/sarabande/main.py` & `sarabande-0.5.0/sarabande/main.py`

 * *Files identical despite different names*

### Comparing `sarabande-0.4.0/sarabande/utils.py` & `sarabande-0.5.0/sarabande/utils.py`

 * *Files identical despite different names*

### Comparing `sarabande-0.4.0/sarabande.egg-info/PKG-INFO` & `sarabande-0.5.0/sarabande.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarabande
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tool for measuring 3/4 PCFs on discrete periodic data.
 Home-page: https://github.com/James11222/sarabande/
 Author: James Sunseri
 Author-email: jamessunseri@berkeley.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/sarabande/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `sarabande-0.4.0/setup.py` & `sarabande-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='sarabande',  # Required
-    version='0.4.0',  # Required
+    version='0.5.0',  # Required
     description='Tool for measuring 3/4 PCFs on discrete periodic data.',  # Optional
     long_description=(here / 'README.md').read_text(encoding='utf-8'),  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/James11222/sarabande/',  # Optional
 
     author='James Sunseri',  # Optional
```

