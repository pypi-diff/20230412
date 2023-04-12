# Comparing `tmp/costcalc2-0.9.0.tar.gz` & `tmp/costcalc2-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "costcalc2-0.9.0.tar", last modified: Fri Nov 18 18:30:47 2022, max compression
+gzip compressed data, was "costcalc2-0.9.1.tar", last modified: Wed Apr 12 21:35:01 2023, max compression
```

## Comparing `costcalc2-0.9.0.tar` & `costcalc2-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 18:30:47.031016 costcalc2-0.9.0/
--rw-rw-rw-   0        0        0    35803 2022-09-24 15:09:32.000000 costcalc2-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      972 2022-11-18 18:30:47.031016 costcalc2-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      293 2022-09-29 23:21:18.000000 costcalc2-0.9.0/README.md
--rw-rw-rw-   0        0        0     1159 2022-11-18 18:29:38.000000 costcalc2-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-18 18:30:47.031016 costcalc2-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-18 18:30:46.963820 costcalc2-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-18 18:30:46.988970 costcalc2-0.9.0/src/costcalc/
--rw-rw-rw-   0        0        0      192 2022-11-18 18:22:30.000000 costcalc2-0.9.0/src/costcalc/__init__.py
--rw-rw-rw-   0        0        0     2960 2022-11-18 18:26:15.000000 costcalc2-0.9.0/src/costcalc/constants.py
--rw-rw-rw-   0        0        0    28622 2022-11-18 18:26:15.000000 costcalc2-0.9.0/src/costcalc/core.py
--rw-rw-rw-   0        0        0     1675 2022-11-18 18:26:15.000000 costcalc2-0.9.0/src/costcalc/exceptions.py
--rw-rw-rw-   0        0        0    16673 2022-11-18 18:26:15.000000 costcalc2-0.9.0/src/costcalc/frontends.py
--rw-rw-rw-   0        0        0    13339 2022-11-18 18:26:15.000000 costcalc2-0.9.0/src/costcalc/helper.py
-drwxrwxrwx   0        0        0        0 2022-11-18 18:30:47.027405 costcalc2-0.9.0/src/costcalc2.egg-info/
--rw-rw-rw-   0        0        0      972 2022-11-18 18:30:46.000000 costcalc2-0.9.0/src/costcalc2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2022-11-18 18:30:46.000000 costcalc2-0.9.0/src/costcalc2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 18:30:46.000000 costcalc2-0.9.0/src/costcalc2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2022-11-18 18:30:46.000000 costcalc2-0.9.0/src/costcalc2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-18 18:30:46.000000 costcalc2-0.9.0/src/costcalc2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 21:35:01.261421 costcalc2-0.9.1/
+-rw-rw-rw-   0        0        0    35803 2022-09-24 15:09:32.000000 costcalc2-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1367 2023-04-12 21:35:01.260444 costcalc2-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-04-12 17:36:28.000000 costcalc2-0.9.1/README.md
+-rw-rw-rw-   0        0        0     1159 2023-04-12 21:30:05.000000 costcalc2-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:35:01.261421 costcalc2-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 21:35:01.235536 costcalc2-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 21:35:01.242421 costcalc2-0.9.1/src/costcalc/
+-rw-rw-rw-   0        0        0       85 2023-04-12 17:36:28.000000 costcalc2-0.9.1/src/costcalc/__init__.py
+-rw-rw-rw-   0        0        0     2600 2023-04-12 17:36:28.000000 costcalc2-0.9.1/src/costcalc/constants.py
+-rw-rw-rw-   0        0        0    39033 2023-04-12 21:28:48.000000 costcalc2-0.9.1/src/costcalc/core.py
+-rw-rw-rw-   0        0        0     2950 2023-04-12 17:36:28.000000 costcalc2-0.9.1/src/costcalc/exceptions.py
+-rw-rw-rw-   0        0        0    15272 2023-04-12 17:36:28.000000 costcalc2-0.9.1/src/costcalc/frontends.py
+-rw-rw-rw-   0        0        0     9710 2023-04-12 21:28:48.000000 costcalc2-0.9.1/src/costcalc/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:35:01.258422 costcalc2-0.9.1/src/costcalc2.egg-info/
+-rw-rw-rw-   0        0        0     1367 2023-04-12 21:35:01.000000 costcalc2-0.9.1/src/costcalc2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-12 21:35:01.000000 costcalc2-0.9.1/src/costcalc2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:35:01.000000 costcalc2-0.9.1/src/costcalc2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-04-12 21:35:01.000000 costcalc2-0.9.1/src/costcalc2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 21:35:01.000000 costcalc2-0.9.1/src/costcalc2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 21:35:01.259452 costcalc2-0.9.1/tests/
+-rw-rw-rw-   0        0        0     6758 2023-04-12 17:35:52.000000 costcalc2-0.9.1/tests/test_core.py
```

### Comparing `costcalc2-0.9.0/LICENSE` & `costcalc2-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `costcalc2-0.9.0/PKG-INFO` & `costcalc2-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: costcalc2
-Version: 0.9.0
+Version: 0.9.1
 Summary: Calculate raw material costs for chemical synthetic route
 Author-email: Ryan Nelson <rnelsonchem@gmail.com>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/rnelsonchem/costcalc2
 Keywords: Chemical,Synthesis,Route,Cost,Pricing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,20 +12,28 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-# costcalc
+# costcalc2
 
-*costcalc* is a Python library for calculating the overall raw materials costs 
-of a user-defined synthetic route. This package is intended for Python 
-versions >= 3.
+*costcalc2* is a Python library for calculating the overall raw materials costs 
+of a user-defined synthetic route. 
 
 ## Requirements
 
 * Python >= 3
 * Numpy >= 1.0
 * Pandas >= 1.0
 * Matplotlib >= 3.0
 * Openpyxl >= 3.0
+
+# Web Application and Documentation
+
+A minimal [working web application](https://costcalc.rnelsonchem.com/) is
+available for running cost calculations without installing this package.
+However, for users that are interested in writing programs using `costcalc2`,
+there is an [annotated Jupyter
+notebook](https://gist.github.com/rnelsonchem/5f38f9f6261591a158ed06c643fe09e7)
+that demonstrates a common use case and most of the methods.
```

### Comparing `costcalc2-0.9.0/pyproject.toml` & `costcalc2-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2263 6f73 7463 616c  .name = "costcal
 00000070: 6332 220d 0a76 6572 7369 6f6e 203d 2022  c2"..version = "
-00000080: 302e 392e 3022 0d0a 0d0a 6465 7363 7269  0.9.0"....descri
+00000080: 302e 392e 3122 0d0a 0d0a 6465 7363 7269  0.9.1"....descri
 00000090: 7074 696f 6e20 3d20 2243 616c 6375 6c61  ption = "Calcula
 000000a0: 7465 2072 6177 206d 6174 6572 6961 6c20  te raw material 
 000000b0: 636f 7374 7320 666f 7220 6368 656d 6963  costs for chemic
 000000c0: 616c 2073 796e 7468 6574 6963 2072 6f75  al synthetic rou
 000000d0: 7465 220d 0a6b 6579 776f 7264 7320 3d20  te"..keywords = 
 000000e0: 5b20 2243 6865 6d69 6361 6c22 2c20 2253  [ "Chemical", "S
 000000f0: 796e 7468 6573 6973 222c 2022 526f 7574  ynthesis", "Rout
```

### Comparing `costcalc2-0.9.0/src/costcalc/constants.py` & `costcalc2-0.9.1/src/costcalc/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-'''Constants that can be ported to the different modules.
+'''Constants that are used across different modules.
 '''
-# This is a blank variable for import, see __init__
-_blank = None
-
-# Setting the display to print function
-# This gets changed for Jupyter Notebook/IPython sessions, so that DataFrames
-# are displayed in a fancier format
-try:
-    from IPython.display import display as disp
-    from IPython.display import Javascript
-except:
-    disp = print
-
 # Column name mapper: This is setting variable names for many of the important
 # DataFrame columns. 
 # Reactions Table Columns
 RXN_STP = 'Step' # The step labels
 RXN_CPD = 'Compound' # The compound names column, same for materials table
 RXN_EQ = 'Equiv' # Molar equivalents of reagent
 RXN_MS = 'Mass' # Mass of material used, typically kg, just be consistent
```

### Comparing `costcalc2-0.9.0/src/costcalc/core.py` & `costcalc2-0.9.1/src/costcalc/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,133 @@
-'''
-Chemical Reaction Cost Calculation and Excel Export Algorithms.
-Adapted from the Excel spreadsheets prepared by Saeed Ahmad, PhD.
-(C) Ryan Nelson
-'''
-import time
-
 import numpy as np
 import pandas as pd
 
 from .constants import *
 from .exceptions import *
 
 class CoreCost(object):
     def __init__(self, materials, rxns, final_prod, disp_err_df=False):
+        '''Core class for calculating route costs and PMI.
+
+        Parameters
+        ----------
+        materials : DataFrame
+            A DataFrame containing  materials properties. At a minimum, this
+            table must include the materials used in the route; however, it
+            can contain an arbitrary number of additional materials as well,
+            as long as the names are unique. This DataFrame must contain the
+            following columns:
+
+                * Compound : str, the compound names.
+                * MW : float, the compound molecular weights.
+                * Density : float, the density (g/mL) of the compound.
+                Although this column must be present, density values are only
+                necessary for reaction solvents.
+                * Cost : float, the cost/price of the compound in $/kg. Can be
+                left blank for unknown costs, like intermediates and final
+                products
+                * Notes : str, optional notes about the compound.
+
+            As noted above, the `Cost` column can be left blank for materials
+            that will have their costs calculated. However, placeholder prices
+            can be put here, if desired. These prices will be ignored if the
+            compounds RM cost is being calculated in the route.
+
+        rxns : DataFrame
+            A DataFrame containing reaction information. This DataFrame must
+            contain the following columns:
+
+                * Step : str, a unique identifier for each step such as "1" or
+                "1a"
+                * Compound: str, the compound names
+                * Equiv : float, the equivalents used for each compound, for
+                reaction products, this value should be the fractional yield
+                (e.g. 75% yield is 0.75 equiv)
+                * Mass : float, (Optional), the mass of material used. This is
+                used to calculate equivalents. If used, the first compound
+                for each reaction must be the limiting reagent.
+                * Volumes : float, volume equivalents of solvent (L/kg)
+                * Relative : str, the compound name to use as the reference
+                for converting solvent volumes to kg. This must correspond to
+                one of the Compound strs for the step
+                * Sol Recyc : float, fractional percentage of solvent that can
+                be recycled. E.g. 75% of solvent can be recycled = 0.75
+                * Cost step : str, the "Step" where compound costs are
+                calculated. For reaction products, this will be the current
+                "Step". This is used to trace the reaction network.
+                * OPEX : float, a $/kg-step charge that is (optionally) added
+                to the final raw-material cost of a reaction product. Is only
+                valid for reaction products.
+
+        final_prod : str
+            Name of the final product in the route.
+
+        disp_err_df : Boolean (False)
+            If a `CostError` exception is raised, this controls whether the
+            offending section of the DataFrame will be printed along with the
+            error. This is useful for debugging, but is typically set to
+            False, so that potentially sensitive information is not printed to
+            the error logs.
+
+        Attributes
+        ----------
+        final_prod : str
+            The name of the overall final product of this route.
+            
+        rxns : DataFrame
+            A DataFrame describing the reactions defined for the route. 
+            
+        materials : DataFrame
+            A DataFrame describing all of the known materials. This will contain
+            all of the materials from both the `materials_file` and the
+            `alt_mat_file`.
+            
+        cost : float
+            The final cost of the described route. This value is only present
+            after the `calc_cost` method is called. 
+            
+        fulldata : DataFrame
+            A combined DataFrame containing all of the reaction, material, and
+            costing related values for the given route. 
+
+        pmi : DataFrame
+            A DataGrame containing the PMI for each reaction and the overall
+            route. There will be an extra column with names used for sorting
+            purposes; this column can be ignored.
+
+        Notes
+        -----
+        Some automated value correction is done on the input DataFrames, such
+        as removing blank lines and extra whitespace in compound names.
+        However, other common errors will raise `CostError` exceptions, and
+        these problems will require manual error correction from the user.
+        '''
         # We need to store the input values/DataFrames
         self.rxns = rxns
         self.materials = materials
         self.final_prod = final_prod        
         self._disp_err_df = disp_err_df
 
-        # Correct typical input problems. This needs to be done before the
-        # setup method below, because it can affect the combining of the two
-        # tables
+        # Correct typical input problems. 
         self._problem_correct()
 
-        # Combine the reaction/materials sheets, add the new columns
+        # Combine the reaction/materials sheets, add new columns
         self.rxn_data_setup()
 
         # Look for other common errors in the input. Throw an error if found
         # These errors must be manually fixed by the user, which is why they
         # are not covered in problem correction method
         self._sanity_check()
 
     def _problem_correct(self, ):
+        '''Correct typical input problems in the input DataFrames.
+
+        These are problems that tend to cause problems before merging using
+        `rxn_data_setup` method, so they are automatically modified here. 
+        '''
         rxn = self.rxns.copy()
         mat = self.materials.copy()
         # Drop lines that are still empty, these cause all sorts of
         # problems. Assume rxn/materials tables should have compound names
         # for valid entries
         rxn = rxn[ ~rxn[RXN_CPD].isna() ]
         mat = mat[ ~mat[RXN_CPD].isna() ]
@@ -53,16 +144,18 @@
         self.materials = mat.copy()
 
     def rxn_data_setup(self, ):
         '''Setup the full data set for the upcoming cost calculations. 
         
         This method merges the materials and reaction sheets into a combined
         DataFrame called `fulldata`. It also serves as a "reset" of sorts
-        after a costing calculation, if you want to start over with a
-        different costing model.
+        after a costing calculation, because it uses the input materials and
+        reactions DataFrames to rebuild the `fulldata` table. This is
+        important if you are modifiying values, for example, and you want to
+        put the system back into its starting point. 
         '''
         # Merge the materials and reaction DataFrames. A few columns are
         # dropped, which are not necessary for calculations. The merge happens
         # on the rxns DataFrame ('right'), which means that missing materials
         # will be fairly obvious (no MW, e.g.).
         mat_keeps = [RXN_CPD, MAT_MW, MAT_DEN, MAT_CST, NOTES]
 
@@ -119,14 +212,18 @@
         fulldata = fulldata.sort_index()
         # Remove sorting index, drop column
         fulldata = fulldata.reset_index('idx_col').drop('idx_col', axis=1)
         
         # Save the full data set
         self.fulldata = fulldata
 
+        # Add a modified variable placeholder. This will store modified
+        # values for the helper functions
+        self._mod_vals = []
+
         # Add the empty columns
         self._column_clear()
 
     def _column_clear(self, excel=False):
         '''Clear out calculated values.
 
         This method will reset all the calculated values in the `fulldata`
@@ -146,20 +243,27 @@
 
         # For dynamic Excel
         if excel or self.fulldata.columns.str.contains(SUFFIX).any():
             excel_cols = [DYN_CST, DYN_RKG, DYN_RRMC, DYN_RRMP, DYN_PKG,
                     DYN_PRMC, DYN_PRMP,]
             self.fulldata[ excel_cols ] = ''
 
+        # Change modified values that were set by helper functions
+        for mod in self._mod_vals:
+            self._set_val(*mod)
+
     def _sanity_check(self, ):
         '''Run some sanity checks on the DataFrames to catch common errors.
 
-        Some of the errors are tricky, and the error output is unhelpful.
-        These are some checks that will throw some "sane" errors if things are
-        not correct.
+        Any problems found here will raise custom `CostError` exceptions. (See
+        `costcalc.expections` module for the `CostError` expection class and
+        error text.) Some of the errors are tricky, and the typical Python
+        error output is unhelpful. These errors will require user
+        intervention, unlike the issues corrected by the `_problem_correct`
+        method. 
         ''' 
         # Check for a missing material -- Everything should have a MW
         # If not, this may suggest that there is a line that should not be
         # empty
         mw_mask = self.fulldata[MAT_MW].isna()
         if mw_mask.any():
             err_line = err_lines['miss_mw'] 
@@ -223,14 +327,24 @@
         if len(bad) > 0:
             err_line = err_lines['mis_rel']
             df = self.fulldata.loc[bad, sol_cols]
             raise CostError(err_line, df, self._disp_err_df)
         
     def calc_cost(self, excel=False):
         '''Calculate the cost of the route. 
+
+        This is the main costing method. This will fill in the `fulldata`
+        DataFrame with the appropriate values, and it will set a new class
+        attribute `cost`, which is the total RM cost of the final product.
+
+        Parameters
+        ----------
+        excel : boolean (False)
+            If True, the calculations will output Excel-formated equation
+            strings. By default (False), the output will be numerical values.
         '''
         # Save a time stamp so it can be displayed later
         self._now = pd.Timestamp.now('US/Eastern').strftime('%Y-%m-%d %H:%M')
         # Prep the DataFrame
         self._column_clear(excel=excel)
         # Set a column of unique row labels
         nrows = self.fulldata.shape[0]
@@ -248,25 +362,29 @@
         This is the workhorse function of the whole process, but is not meant
         to be called on its own. Typically, you'll want to call `calc_cost` to
         get the costing information.
         
         Parameters
         ----------
         prod : str
-            The name of the reaction to cost. This should also be the name of
-            the final product for that reaction.
+            The name of the product for a particular reaction.
 
         step : str
-            The step number for which to calculate the cost. Even though the
-            step numbers are numbers, this needs to be given as a string.
+            The step ID for which to calculate the cost. Because the step
+            labels can be numbers (e.g. step 1) and/or letters (e.g. step 1a),
+            this parameter is handled as a string.
 
         amp : float, optional (default = 1.0)
             This number is an amplifier that increases some of the values,
             e.g. masses of materials, based on how much material is being used
-            for the overall final product.   
+            to make 1 kg of the overall final product.   
+
+        excel : boolean (False)
+            Whether to output numerical values (False) or Excel-formatted
+            equation strings (True).
         '''
         # Select out the reaction of interest from the full data set. Saves
         # some typing. (Make this a copy to enusre it isn't given as a view.)
         data = self.fulldata.loc[step].copy()
 
         # Kg of nonsolvent materials used per equivalent
         data[RXN_KG] = data[RXN_EQ]*data[MAT_MW]
@@ -518,15 +636,26 @@
 
     def _excel_pmi(self, col):
         # A function for creating the dynamic Excel cells for PMI
         cells = [f'{ECOLS[RXN_KG]}{i}' for i in col]
         return "=SUM(" + ','.join(cells) + ")"
 
     def results(self, style='compact'):
-        '''Preps an output DataFrame for the results method.
+        '''Returns a formatted/simplified full output DataFrame.
+
+        The `fulldata` attribute contains a number of potentially unnecessary
+        columns that need to be filtered out for presentation purposes. This
+        also combines the PMI data as well, so everything is in one table.
+
+        Parameters
+        ----------
+        style : str ('compact')
+            By default, this returns a minimal representation of the system
+            ('compact'); however, a more complete set of columns can be
+            returned if the value `'full'` is passed as the parameter here.
         '''
         # For compact display, these are the most important columns
         comp_col = [MAT_CST, RXN_EQ,] 
         if self.fulldata.Volumes.any():
             comp_col.extend([RXN_VOL, RXN_RCY,])
         if self.fulldata.OPEX.any():
             comp_col.append(RXN_OPX) 
@@ -556,15 +685,15 @@
         fd = self.fulldata.reset_index()
         pmi = self.pmi.reset_index()
         
         # Concats the fulldata and pmi based on step. The groupby function
         # will sort by "Step" as it processes things. This will need to be
         # modified if this behavior is undesired, but as is, it is not trivial
         # to make this fix. The apply function doubles up the "Step" column.
-        # So one needs to be removed.
+        # So one needs to be dropped.
         gb = fd.groupby(RXN_STP)
         concated = gb.apply(self.__fd_pmi_concat, pmi)
         concated = concated.drop(RXN_STP, axis=1)\
                             .reset_index()\
                             .drop('level_1', axis=1)
         
         # Reset the index and return the DF. No sorting is necessary here.
@@ -581,17 +710,21 @@
         pmi_mask = pmi[RXN_STP] == step
         pmi_small = pmi[pmi_mask]
         # Combine the route step info with the PMI. In this way, the pmi will
         # be at the end.
         return pd.concat([df, pmi_small], ignore_index=True)
 
     def excel(self, ):
-        '''Prepare a DataFrame for Excel export.
+        '''Return an Excel-formatted DataFrame.
 
-        See `excel_save` method for the docstring info.
+        This table will have equation strings rather than numerical values,
+        and it can be saved to disk using the `DataFrame.to_excel` method, if
+        desired. Because the table contains equation strings, the Excel file
+        will be fully dynamic, in that value changes will cause a
+        recalculation of the entire sheet.
         '''
         # Run the cost calculation again, but using the excel keyword
         self.calc_cost(excel=True)
 
         # Combine the fulldata and pmi DataFrames
         fd = self._df_combine()
         # Move the Notes columns to the end of the combined DataFrame
@@ -629,8 +762,87 @@
         
         # Rerun the cost calculation without the excel stuff to get rid of all
         # the other columns
         self.calc_cost(excel=False)
 
         return fd
 
+    def value_mod(self, cpd, val, val_type='Cost', step=None):
+        '''Manually set a value for a given material.
+
+        This is useful for creating alternative models without having to
+        import completely new reactions and materials tables. The original
+        input tables are not modified, so the model can be reset with the
+        `rxn_data_setup` method. 
+
+        Parameters
+        ----------
+        cpd : str
+            This the compound name for which the value will be modified.
+
+        val : int, float
+            This is the modified value for the parameter.
+
+        val_type : str, optional (Default = 'Cost')
+            This is the column name for the parameter that you'll be changing.
+            This must be for a non-calculated column, such as 'Cost', 'Equiv',
+            'OPEX', etc.
+
+        step : None, int, optional (Default = None)
+            The reaction step number for which this value will be changed. If
+            this is `None` (default), then all the values for the given
+            compound (`cpd`) will be set to the same value. This is mostly
+            important for something like `val_type`='Equiv'. Clearly, you
+            would only want to change the number of equivalents for a specific
+            reaction. If this parameter is left as `None`, the equivalents for
+            a given compound in all reactions will be set to the same value.
+        
+        Note
+        ----
+        This method will *NOT* recalculate the cost; this must be done as a
+        separate step. This behavior is by design so that several `value_mod`
+        method calls can be made, if necessary, before the costs are
+        recaclulated.
+        '''
+        # Store the values
+        self._mod_vals.append( (cpd, val, val_type, step) )
+        # This will clear out the old calculation data and set the modified
+        # value. Keeps folks from getting confused b/c previously calculated
+        # values appear unchanged.
+        self._column_clear()
+
+    def _set_val(self, cpd, val, val_type, step):
+        '''Set a modified value in the `fulldata` DataFrame.
+
+        The modified values are set using the `value_mod` method, which adds
+        the values to a `_mod_vals` list. This function cycles through that
+        list, changing the associated values.
+        '''
+        # The first one sets all values w/ the compound name. The second one
+        # sets only a value for a specific reaction.
+        if not step:
+            cells = (slice(None), cpd)
+        else: 
+            # The step needs to be a string, not in int as might be expected
+            cells = (str(step), cpd)
+        
+        # Does this position actually exist???
+        try:
+            self.fulldata.loc[cells, val_type]
+        except KeyError:
+            # If not, remove the values from the list and throw an error
+            self._mod_vals.pop()
+            if not step:
+                err = '"' + cpd + '"'
+            else:
+                err = 'Step "' + str(step) + '", "' + cpd + '"'
+            print('Oops! ' + err + " doesn't exist. Check") 
+            print("your reactions to find the correct Step/Compound.")
+            raise 
+            
+        self.fulldata.loc[cells, val_type] = val
+        # The "Cost calc" flag must be set to np.nan when setting a cost. 
+        # This is necessary for % RM cost calcs, e.g.
+        if val_type == 'Cost':
+            self.fulldata.loc[cells, RXN_CST] = np.nan
+
```

### Comparing `costcalc2-0.9.0/src/costcalc/exceptions.py` & `costcalc2-0.9.1/src/costcalc/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,60 @@
 from .constants import *
 
+# Setting the display function
+# This gets changed for Jupyter Notebook/IPython sessions, so that DataFrames
+# are displayed in a fancier format
+try:
+    from IPython.display import display as disp
+except:
+    disp = print
+
 class CostError(Exception):
+    '''A custom exception for catching common input errors.
+
+    In addition to error-type specific messages, this also captures and
+    optionally displays the offending portions of the input DataFrames. 
+
+    Parameters
+    ----------
+    message : str
+        The error message to display. See `err_lines` dictionary for the
+        custom messages.
+
+    df : DataFrame (None)
+        The bad portion of the input DataFrame.
+
+    disp_df : Boolean (False)
+        A flag that determines whether the bad DataFrame information is
+        displayed along with the error message. Although this is useful for
+        debugging, this parameter is set to False by default, because this
+        could print sensitive information to the error logs.
+
+
+    Notes
+    -----
+    See the `err_lines` dictionary defined below for the text of the various
+    error messages. See the `CoreCost._sanity_check` method for the checks
+    that are run.
+    '''
     def __init__(self, message, df=None, disp_df=False):
         self.message = message
         self.df = df
         self.disp_df = disp_df
         super().__init__(message)
 
     def __str__(self, ):
         if self.disp_df:
             print(self.message)
             print('See the following entries:')
             disp(self.df)
         return self.message
 
 
+# A dictionary containing custom error messages for common input errors
 err_lines = {
     'miss_mw': 'Missing MW error! \n'\
             'This most commonly happens for 1 of 2 reasons:\n'\
             '1. A reaction compound is not defined in the '\
             'materials table.\n'\
             '2. The compound names in reaction/materials '\
             'tables do not match *exactly* (even white space).',
```

### Comparing `costcalc2-0.9.0/src/costcalc/frontends.py` & `costcalc2-0.9.1/src/costcalc/frontends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,94 +1,78 @@
 import urllib.parse as parse
 
 import numpy as np
 import pandas as pd
 
 from .core import CoreCost
-from .helper import HelperFuncs
 from .constants import *
 
+# Setting the display function
+# This gets changed for Jupyter Notebook/IPython sessions, so that DataFrames
+# are displayed in a fancier format
+try:
+    from IPython.display import display as disp
+    from IPython.display import Javascript
+except:
+    disp = print
+
 # Set pandas to display lots of DataFrame rows so things don't get cut out
 pd.options.display.max_rows = 1000
 # For future reference -- Can't use this in conjunction with "fillna" becuase
 # the DF doesn't display correctly 
 # Set Pandas precision
 #pd.set_option('precision', 2)
 
 class ExcelCost(CoreCost):
-    '''Costing class designed for local Excel/csv spreadsheets.
+    '''Costing class designed for reading data from Excel/csv spreadsheets.
 
-    This can also act as the base class for other subclasses.
+    The Excel/csv files require specific columns to be present. See the
+    `CoreCost` class doc string for more information.
 
     Parameters
     ----------
     materials_file : str
         The name/path of the materials list file. Can be xlsx or csv.
 
     rxn_file : str
-        The name/path of the file defining the reactions. can be xlsx or csv.
-
-    alt_mat_file : str, optional (default = None)
-        The name/path of an optional, secondary materials sheet.  sheet. This
-        is useful if you have separate master and user materials sheets, for
-        example. Can be an xlsx or csv.
+        The name/path of the file defining the reactions. Can be xlsx or csv.
+        Both `rxn_file` and `materials_file` can be the same file.
 
     final_prod : str
-        Defines the final product name for costing calculations. This should
-        be the same name as in the material/reaction sheet.
+        The name of the final product for route. 
 
     materials_sheet : int, str, optional (default = 0)
-        The sheet to pull out of the materials spreadsheet. The default
-        (0) is the first sheet in the spreadsheet. You could use a
-        different number or a name if you want a different sheet from the
+        The sheet in the Excel file that contains the materials information.
+        The default (0) is the first sheet in the spreadsheet. You could use a
+        different number or a name (str) if you want a different sheet from the
         spreadsheet.
 
     rxn_sheet : int, str, optional (default = 0)
-        See `materials_sheet` description, except this is for the reaction
-        Google Sheet.
+        See `materials_sheet` description, except this is for the sheet
+        defining the reactions.
+
+    alt_mat_file : str, optional (default = None)
+        The name/path of an optional, secondary materials sheet. This is
+        useful if you have separate master and route-specific materials
+        sheets, for example. Can be an xlsx or csv.
 
     alt_mat_sheet : int, str, optional (default = 0)
         The sheet number/name for the secondary materials sheet. See
         `materials_sheet` description. 
 
-    Attributes
-    ----------
-    final_prod : str
-        The name of the overall final product of this route.
-        
-    rxns : DataFrame
-        A DataFrame describing the original reactions in the given route. This 
-        is idential to the reactions Google Sheet, and is not changed by any 
-        of the helper functions in this class.
-        
-    materials : DataFrame
-        A DataFrame describing all of the known materials. This will contain
-        all of the materials from both of the given materials Google Sheets.
-        
-    cost : Numpy Float64
-        The final cost of the described route. This value *will* include OPEX
-        for the final reaction, if that value is given. 
-        
-    fulldata : DataFrame
-        A DataFrame containing all the costing related values for the given 
-        route. If the cost for the route has been calculated and an OPEX was 
-        given, the product "Cost" values *will* include this additional OPEX 
-        cost. The "RM cost/kg rxn" value will be the cost without the OPEX.
-
-    pmi : DataFrame
-        A DataGrame containing the PMI for each reaction and the overall
-        route. There will be an extra column with a bunch of weird names. This
-        is necessary for sorting and can be ignored.
+    dis_err_df : boolean (False)
+        If a `CostError` exception is raised, this controls whether the
+        offending section of the DataFrame will be printed along with the
+        error. This is useful for debugging, but is typically set to False, so
+        that potentially sensitive information is not printed to the error
+        logs.
 
     Notes
     -----
-    If there is a missing material or reaction, you'll get a printed
-    error. Materials that are marked as being cost calculated will have
-    their costs deleted, so they will need reactions defined in order to
-    reset their costs.
+    See the `CoreCost` class doc string for additional information. 
     '''
     def __init__(self, materials_file, rxn_file, final_prod,
             materials_sheet=0, rxn_sheet=0, 
             alt_mat_file=None, alt_mat_sheet=0,
             disp_err_df = True):
         # Set up the reaction DataFrame
         self._rxn_file = rxn_file
@@ -194,53 +178,56 @@
         # Display the correct format of data based on the kwargs
         if decimals:
             disp(fd.round(decimals).fillna(fill))
         else:
             disp(fd.fillna(fill))
 
     def excel(self, fname, ):
-        '''Save the costing DataFrame as an Excel file.
+        '''Save the costing DataFrame as a dynamic Excel file.
 
         Parameters
         ----------
         fname : str, ExcelWriter
             The name you want to give to the Excel file, or an ExcelWriter
-            object to send multiple to the same file. See
+            object to send multiple costing sheets to the same file. See
             `pandas.DataFrame.to_excel` documentation for details.
 
         '''
         # Get the process DataFrame
         fd = super(ExcelCost, self).excel()
 
         # Create the excel file. Can only save with the date and not the time
         fd.to_excel(fname, 
                     sheet_name='As of ' + self._now.split()[0], )
             
 
-class ExcelCostAdv(ExcelCost, HelperFuncs):
-    pass
-
-
 class ColabCost(ExcelCost):
     '''Costing class designed for the Colab Python environment.
 
+    The materials and reaction information must be in Google Sheet format; the
+    urls below are the URL values for those sheets. The user must have read
+    access for the sheets to be able to use them. 
+
     Parameters
     ----------
     materials_url : str
-        The Google Sheet key to a materials list. This value can be found
-        in the URL of the sheet.
+        The URL to the Google sheet containing the materials list. 
 
     rxn_url : str
-        The Google Sheet key to the reaction list. This value can be found
-        in the URL of the sheet.
+        The URL to the Google sheet containing the reaction information. 
 
     alt_mat_url : str, optional (default = None)
-        A Google Sheet key for an optional, secondary materials sheet.
-        This is useful if you have separate master and user materials
-        sheets, for example.
+        The URL to the Google sheet containing an optional, secondary
+        materials list.  This is useful if you have separate master and user
+        materials sheets, for example.
+
+    Notes
+    -----
+    This is subclass of `ExcelCost` and `CoreCost`, so see those class
+    docstrings for more information.
 
     '''
     def __init__(self, materials_url, rxn_url, final_prod, materials_sheet=0,
             rxn_sheet=0, alt_mat_url=None, alt_mat_sheet=0):
         # Do some imports that are only possible in the Colab environment
         # This should prevent these from running in a non-Colab environment
         from google.auth import default
@@ -281,15 +268,16 @@
         num_cols = [MAT_MW, MAT_DEN, MAT_CST] 
         for nc in num_cols:
             mats[nc] = pd.to_numeric(mats[nc])
 
         return mats
         
     def _rxn_read(self, ):
-        '''Read a Google Sheet of reaction info.
+        '''Read a Google Sheet containing reaction info and convert it to a
+        DataFrame.
         '''
         rxns = self._get_sheet_vals(self._rxn_file,
                                      self._rxn_sheet)
 
         # Set some rxns columns to numeric values. Everything is read from a
         # Google sheet as strings
         num_cols = [RXN_EQ, RXN_VOL, RXN_RCY, RXN_OPX]
@@ -298,15 +286,15 @@
             num_cols.append(RXN_MS)
         for nc in num_cols:
             rxns[nc] = pd.to_numeric(rxns[nc])
         
         return rxns
         
     def _get_sheet_vals(self, key, sheet):
-        '''General code for getting Google Sheet values and returning a 
+        '''General code for obtaining Google Sheet values and returning a 
         DataFrame.
         '''
         # Check if the `key` is a URL. If so, pull apart the url and grab the
         # part of the path that is the key to the spreadsheet.
         if key.startswith('http'):
             url_frag = parse.urlparse(key)
             key = url_frag.path.split('/')[3]
@@ -336,44 +324,30 @@
         val_df = val_df[mask]
         
         return val_df
 
     def results(self, style='compact', decimals=2, fill='-'):
         '''Print the results of the costing calculation.
 
-        Parameters
-        ----------
-        style : str, optional (Default = 'compact')
-            This sets the style of the displayed costing DataFrame.
-            `'compact'` prints a DataFrame that has been truncated slightly.
-            `'full'` prints the entire DataFrame.
-
-        decimals : int or None, optional (Default = 2)
-            How many decimal places to show in the table. Set this to `None`
-            if you want full precision.
-
-        fill : str or None, optional (Default = '-')
-            Fill NaN values with this string. This makes the table a little
-            easier to read. Set this to `None` if you want to see the table
-            with the typical NaN labels.
+        See the `ExcelCost.results` method doc string for details on the
+        function parameters.
         '''
         # This makes the max Colab output window very large, so that
         # DataFrames are not put into separate scroll windows, which is very
         # annoying for users. Unfortunately, I need to copy/paste the doc
         # string for results method, though...
         # See: https://github.com/googlecolab/colabtools/issues/541
         iframe_h = 'google.colab.output.setIframeHeight(0, true, {\n'\
                    '  maxHeight: 5000,\n'\
                    '})'
         disp(Javascript(iframe_h)) 
         # Call results method from ExcelCost
         super(ColabCost, self).results(style=style, decimals=decimals,
                                        fill=fill)
 
-
     def excel(self, fname):
         '''Download the costing DataFrame as an Excel file.
 
         Parameters
         ----------
         fname : str
             The name you want to give to the Excel file.
@@ -381,18 +355,14 @@
         '''
         super(ColabCost, self).excel(fname, )
 
         # Use the Colab function for downloading the file from the server
         files.download(fname)
         
 
-class ColabCostAdv(ColabCost, HelperFuncs):
-    pass
-
-
 class WebAppCost(ExcelCost):
     '''Costing class designed for the Streamlit Web App environment.
 
     This is largely the same as the `ExcelCost` class, so see that method for
     a more complete docstring. 
     '''
     def __init__(self, materials_file, rxn_file, final_prod,
@@ -401,28 +371,23 @@
             disp_err_df=False):
 
         super(WebAppCost, self).__init__(materials_file, rxn_file, final_prod,
                 materials_sheet, rxn_sheet, alt_mat_file, alt_mat_sheet,
                 disp_err_df)
 
     def results(self, style='compact', decimals=2, fill=np.nan):
-        '''Print the results of the costing calculation.
+        '''Returns the results of the costing calculation.
+
+        See the `ExcelCost.results` method for additional documentation. This
+        is largely the same as that method except for the optional `fill`
+        keyword argument below.
 
         Parameters
         ----------
-        style : str, optional (Default = 'compact')
-            This sets the style of the displayed costing DataFrame.
-            `'compact'` prints a DataFrame that has been truncated slightly.
-            `'full'` prints the entire DataFrame.
-
-        decimals : int or None, optional (Default = 2)
-            How many decimal places to show in the table. Set this to `None`
-            if you want full precision.
-
-        fill : str or None, optional (Default = np.nan)
+        fill : str, None, or Numpy.nan (Default = Numpy.nan)
             Fill NaN values with this string. This makes the table a little
             easier to read. Set this to `None` if you want to see the table
             with the typical NaN labels.
         '''
         # Use the CoreCost.results method to get the initial results DataFrame
         fd = super(ExcelCost, self).results(style)
```

### Comparing `costcalc2-0.9.0/src/costcalc/helper.py` & `costcalc2-0.9.1/src/costcalc/helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,331 +1,259 @@
-# Import everything from the core file to get all of the column variable
-# definitions
-from .core import CoreCost
 from .constants import *
 
+import numpy as np
+import pandas as pd
 import matplotlib.pyplot as plt
 
-# Set up some plotting stuff for the notebooks
-plt.style.use('ggplot')
-plt.rc('figure', dpi=150)
-
-
-class HelperFuncs(CoreCost):
-    def rxn_data_setup(self, ):
-        # Add a modified variable placeholder. This will store modified
-        # values for later processing
-        self._mod_vals = []
-
-        super(HelperFuncs, self).rxn_data_setup()
-
-    def _column_clear(self, excel=False):
-        '''Clear out calculated values.
-
-        This method will reset all the calculated values in the `fulldata`
-        DataFrame. This is perhaps not strictly necessary, but it should help
-        to avoid unwanted errors in recalculations due to old data still being
-        present. This is not the same as a reset, though, because manually
-        modified values with `value_mod` method will be re-modified. 
-        '''
-        super(HelperFuncs, self)._column_clear(excel)
-
-        # Modify stored mod variables
-        for mod in self._mod_vals:
-            self._set_val(*mod)
-
-
-    def _set_val(self, cpd, val, val_type, step):
-        '''Set a modified value in the `fulldata` DataFrame
-        '''
-        # The first one sets all values w/ the compound name. The second one
-        # sets only a value for a specific reaction.
-        if not step:
-            cells = (slice(None), cpd)
-        else: 
-            # The step needs to be a string, not in int as might be expected
-            cells = (str(step), cpd)
+def value_scan(model, cpd, start, stop, npts, val_type='Cost', step=None):
+    '''Scan a range of values for a given material.
+    
+    Parameters
+    ----------
+    model : CoreCost or subclass
+        This is the costing model instance that will be modified.
         
-        # Does this position actually exist???
-        try:
-            self.fulldata.loc[cells, val_type]
-        except KeyError:
-            # If not, remove the values from the list and throw an error
-            self._mod_vals.pop()
-            if not step:
-                err = '"' + cpd + '"'
-            else:
-                err = 'Step "' + str(step) + '", "' + cpd + '"'
-            print('Oops! ' + err + " doesn't exist. Check") 
-            print("your reactions to find the correct Step/Compound.")
-            raise 
-            
-        self.fulldata.loc[cells, val_type] = val
-        # The "Cost calc" flag must be set to np.nan when setting a cost. 
-        # This is necessary for % RM cost calcs, e.g.
-        if val_type == 'Cost':
-            self.fulldata.loc[cells, RXN_CST] = np.nan
-
-    def value_mod(self, cpd, val, val_type='Cost', step=None):
-        '''Manually set a value for a given material.
-
-        Parameters
-        ----------
-        cpd : str
-            This the compound name for which the value will be modified.
-
-        val : int, float
-            This is the modified value for the parameter.
-
-        val_type : str, optional (Default = 'Cost')
-            This is the column name for the parameter that you'll be changing.
-            This must be for a non-calculated column, such as 'Cost', 'Equiv',
-            'OPEX', etc.
-
-        step : None, int, optional (Default = None)
-            The reaction step number for which this value will be changed. If
-            this is `None` (default), then all the values for the given
-            compound (`cpd`) will be set to the same value. This is mostly
-            important for something like `val_type`='Equiv'. Clearly, you
-            would only want to change the number of equivalents for a specific
-            reaction. If this parameter is left as `None`, the equivalents for
-            a given compound in all reactions will be set to the same value.
-        
-        Note
-        ----
-        This method will *NOT* recalculate the cost; this must be done as a
-        separate step.
-        '''
-        # Store the values
-        self._mod_vals.append( (cpd, val, val_type, step) )
-        # This will clear out the old calculation data and set the modified
-        # value. Keeps folks from getting confused b/c calculated values are
-        # unchanged.
-        self._column_clear()
-            
-    def value_scan(self, cpd, start, stop, npts, val_type='Cost', step=None):
-        '''Scan a range of values for a given material.
-        
-        Parameters
-        ----------
-        See `value_mod` method description, except for the following.
-
-        start : int, float
-            The starting value for the scan.
-
-        stop : int, float
-            The ending value for the scan.
-
-        npts : int
-            The numbers of points to calculate the costs between `start` and
-            `stop`
-
-        Returns
-        -------
-        Pandas DataFrame
-            This DataFrame has 'Values' and 'Costs' columns for the input
-            values and output costs, repectively. 
-
-        Notes
-        -----
-        Although this method recalculates the cost for every value, it does
-        not modify the original `fulldata` or `cost` attributes. 
-        '''
-        # Create the values array
-        vals = np.linspace(start, stop, npts)
-       
-        # I need a copy of the full data set in order to reset for each
-        # iteration. Otherwise, I was noticing some issues.
-        fd_copy = self.fulldata.copy()
-        all_costs = []
-        for val in vals:
-            self.value_mod(cpd, val, val_type, step)
-            self.calc_cost()
-            all_costs.append(self.cost)
-            # Reset the full data set 
-            self.fulldata = fd_copy.copy()
-            # Pop out the mod value, otherwise this list will get really long
-            self._mod_vals.pop()
-
-        # Reset the final cost
-        self.cost = self.fulldata.loc[(self._fp_idx, self.final_prod), 
-                                  'RM cost/kg rxn']
-        
-        return pd.DataFrame({'Values':vals, 'Costs':all_costs})
+    cpd : str
+        This the compound name for which the value will be modified.
 
-    def plot_scan(self, cpd, start, stop, npts, val_type='Cost', step=None, 
-                legend=None):
-        '''Plot a range of values.
-
-        Parameters
-        ----------
-        See `value_scan` method description, except for the following.
-
-        legend : bool, str
-            This will add a legend to the plot. If you use the value `True`,
-            the compound name will be added to the legend. Otherwise, you can
-            pass a custom string if you want that to be in the legend instead.
-
-        '''
-        # Calculate all the costs for the given values
-        costs = self.value_scan(cpd, start, stop, npts, val_type=val_type,
-                            step=step)
-        
-        # If legend is selected, make sure the label is set properly
-        if legend == True:
-            label = cpd
-        else:
-            label = legend
-
-        # Plot the values
-        plt.plot(costs['Values'], costs['Costs'], 'o', label=label)
-        # Generate the legend, if requested
-        if legend:
-            plt.legend()
-
-
-    def swap(self, cpd_old, cpd_new, step=None):
-        '''Swap one compound for another in the route.
-
-        Parameters
-        ----------
-        cpd_old : str
-            This is the name of the compound that you want to remove from the
-            route costing.
-
-        cpd_new : str or Cost class
-            This can either be the name of the new compound to add into the
-            route or a Cost class instance, such as ExcelCost. If it is just a
-            name, the material properties will be pulled out of the materials
-            database. If the Cost class instance is used, the the final
-            product information will be pulled from there. (In that case,
-            then, the `cost_calc` method must have been run on that instance
-            to define the final cost of that material.
-
-        step : int or None, optional (default = None)
-            This is the step number for which to do the swap. The default
-            (None) is to swap all instances of the particular compound.
-
-        Note
-        ----
-            If you swap out a compound that was marked to have its cost
-            calculated, this method will switch off this feature, which is
-            most likely what was intended. 
-        '''
-        # If the new compound is a string, look in the materials database
-        if isinstance(cpd_new, str):
-            mat_mask = self.materials.Compound == cpd_new
-            # Throw an error if it is not there
-            if not mat_mask.any():
-                raise ValueError("Oops! Your new compound isn't in the"
-                                " materials list.")
-            # There should only be one entry, so we'll select that one
-            mat_vals = self.materials[mat_mask].iloc[0]
-            # Set some values that will be used for updating
-            cpd_name = cpd_new
-            mw = mat_vals[MAT_MW]
-            density = mat_vals[MAT_DEN]
-            cost = mat_vals[MAT_CST]
-        
-        # If the new compound is a costing instance...
-        elif isinstance(cpd_new, (ExcelCost, ColabCost)):
-            # The value selection is a little different
-            cpd_name = cpd_new.final_prod
-            cpd_loc = (cpd_new._fp_idx, cpd_new.final_prod)
-            mw = cpd_new.fulldata.loc[cpd_loc, MAT_MW]
-            density = cpd_new.fulldata.loc[cpd_loc, MAT_DEN]
-            cost = cpd_new.fulldata.loc[cpd_loc, MAT_CST]
-        
-        # Else you've added the wrong kind of new compound
-        else:
-            raise ValueError("Oops!! Your new compound is not "
-                            "of the correct type.")
-
-        # Process the fulldata array
-        # First, remove the MultiIndex
-        fd_rst = self.fulldata.reset_index()
-        # Check for the requested compound
-        cpd_mask = fd_rst[RXN_CPD] == cpd_old
-        # If a particular step is chosen, select only that step
-        if step:
-            cpd_mask = cpd_mask & (fd_rst[RXN_STP] == str(step))
-
-        if not cpd_mask.any():
-            raise ValueError("Oops! '" + cpd_old + "' isn't in your "
-                            "current route.")
-        # Swap out the compound names
-        fd_rst.loc[cpd_mask, RXN_CPD] = cpd_name
-        # Reset index and fulldata attribute
-        self.fulldata = fd_rst.set_index([RXN_STP, RXN_CPD])
-
-        # Set the values using `value_mod`
-        self.value_mod(cpd_name, mw, val_type='MW', step=step)
-        self.value_mod(cpd_name, density, val_type='Density', step=step)
-        self.value_mod(cpd_name, cost, step=step)
-
-    def sensitivity(self, col='Equiv', frac=0.1, decimals=2):
-        '''Do a sensitivity analysis for the equivalents of reagents.
-
-        Parameters
-        ----------
-        col : str, optional (Default = 'Equiv')
-            Which column from the `fulldata` DataFrame should be used for the
-            sensitivity analysis. 
-
-        frac : float, optional (Default = 0.1)
-            Fractional percentage to increase/decrease the values by before
-            recosting. The default is 0.1, which is the same as +/- 10%. 
-
-        decimals : int or None, optional (Default = 2)
-            How many decimal places to display. If `None`, the full precision
-            DataFrame will be displayed.
-        '''
-        # Make a new DF for sensitivity analysis
-        # Make values that are a certain percent above and below the current
-        # numbers
-        sens = self.fulldata[[col]].dropna()
-        sens['Val low'] = sens[col]*(1 - frac)
-        sens['Val high'] = sens[col]*(1 + frac)
+    start : int, float
+        The starting value for the scan.
+
+    stop : int, float
+        The ending value for the scan.
+
+    npts : int
+        The numbers of points to calculate the costs between `start` and
+        `stop`
+
+    val_type : str, optional (Default = 'Cost')
+        This is the column name for the parameter that you'll be changing.
+        This must be for a non-calculated column, such as 'Cost', 'Equiv',
+        'OPEX', etc.
+
+    step : None, int, optional (Default = None)
+        The reaction step number for which this value will be changed. If
+        this is `None` (default), then all the values for the given
+        compound (`cpd`) will be set to the same value. This is mostly
+        important for something like `val_type`='Equiv'. Clearly, you
+        would only want to change the number of equivalents for a specific
+        reaction. If this parameter is left as `None`, the equivalents for
+        a given compound in all reactions will be set to the same value.
+
+    Returns
+    -------
+    Pandas DataFrame
+        This DataFrame has 'Values' and 'Costs' columns for the input
+        values and output costs, repectively. 
+
+    Notes
+    -----
+    Although this method recalculates the cost for every value, it does
+    not modify the original `fulldata` or `cost` attributes. 
+    '''
+    # Create the values array
+    vals = np.linspace(start, stop, npts)
+   
+    # I need a copy of the full data set in order to reset for each
+    # iteration. Otherwise, I was noticing some issues.
+    fd_copy = model.fulldata.copy()
+    all_costs = []
+    for val in vals:
+        model.value_mod(cpd, val, val_type, step)
+        model.calc_cost()
+        all_costs.append(model.cost)
+        # Reset the full data set 
+        model.fulldata = fd_copy.copy()
+        # Pop out the mod value, otherwise this list will get really long
+        model._mod_vals.pop()
+
+    # Reset the final cost
+    model.cost = model.fulldata.loc[(model._fp_idx, model.final_prod), 
+                              'RM cost/kg rxn']
+    
+    return pd.DataFrame({'Values':vals, 'Costs':all_costs})
+
+
+def plot_scan(model, cpd, start, stop, npts, val_type='Cost', step=None, 
+            legend=None):
+    '''Plot a range of values.
+
+    Parameters
+    ----------
+    See `value_scan` method description, except for the following.
+
+    legend : bool, str
+        This will add a legend to the plot. If you use the value `True`,
+        the compound name will be added to the legend. Otherwise, you can
+        pass a custom string if you want that to be in the legend instead.
+
+    '''
+    # Calculate all the costs for the given values
+    costs = value_scan(model, cpd, start, stop, npts, val_type=val_type,
+                        step=step)
+    
+    # If legend is selected, make sure the label is set properly
+    if legend == True:
+        label = cpd
+    else:
+        label = legend
+
+    # Plot the values
+    plt.plot(costs['Values'], costs['Costs'], 'o', label=label)
+    # Generate the legend, if requested
+    if legend:
+        plt.legend()
+
+
+def swap(model, cpd_old, cpd_new, step=None):
+    '''Swap one compound for another in the route.
+
+    Parameters
+    ----------
+    model : CoreCost or subclass
+        This is the costing model instance that will be modified.
         
-        # Re-run the costing under the current conditions, which resets the
-        # cost and fulldata variables. 
-        self.calc_cost()
-        # Make copies of these values so they don't change
-        cost_save = self.cost
-        fd_save = self.fulldata.copy()
-
-        # Loop through the values and calculate the cost if these values
-        # increase or decease by the percent given
-        for step_cpd, vals in sens.iterrows():
-            step, cpd = step_cpd
-            # Low values
-            self.value_mod(cpd, vals['Val low'], val_type=col, step=step)
-            self.calc_cost()
-            cost_low = self.cost
-            cost_low_per = (cost_low*100./cost_save) - 100
-            # Just to be safe - Drop the modified value
-            self._mod_vals.pop()
-
-            # High values
-            self.value_mod(cpd, vals['Val high'], val_type=col, step=step)
-            self.calc_cost()
-            cost_high = self.cost
-            cost_high_per = (cost_high*100./cost_save) - 100
-            self._mod_vals.pop()
-
-            # Set the values in the sensitivity DataFrame
-            sens.loc[(step, cpd), 'Cost low'] = cost_low
-            sens.loc[(step, cpd), 'Cost high'] = cost_high
-            sens.loc[(step, cpd), '% low'] = cost_low_per
-            sens.loc[(step, cpd), '% high'] = cost_high_per
-
-            # Reset the original values.  This is necessary so the next step
-            # in the loop starts from the original position.
-            self.cost = cost_save
-            self.fulldata = fd_save.copy()
+    cpd_old : str
+        This is the name of the compound that you want to remove from the
+        route costing.
+
+    cpd_new : str or Cost class
+        This can either be the name of the new compound to add into the
+        route or a Cost class instance, such as ExcelCost. If it is just a
+        name, the material properties will be pulled out of the materials
+        database. If the Cost class instance is used, the the final
+        product information will be pulled from there. (In that case,
+        then, the `cost_calc` method must have been run on that instance
+        to define the final cost of that material.
+
+    step : int or None, optional (default = None)
+        This is the step number for which to do the swap. The default
+        (None) is to swap all instances of the particular compound.
+
+    Note
+    ----
+        If you swap out a compound that was marked to have its cost
+        calculated, this method will switch off this feature, which is
+        most likely what was intended. 
+    '''
+    # If the new compound is a string, look in the materials database
+    if isinstance(cpd_new, str):
+        mat_mask = model.materials.Compound == cpd_new
+        # Throw an error if it is not there
+        if not mat_mask.any():
+            raise ValueError("Oops! Your new compound isn't in the"
+                            " materials list.")
+        # There should only be one entry, so we'll select that one
+        mat_vals = model.materials[mat_mask].iloc[0]
+        # Set some values that will be used for updating
+        cpd_name = cpd_new
+        mw = mat_vals[MAT_MW]
+        density = mat_vals[MAT_DEN]
+        cost = mat_vals[MAT_CST]
+    
+    # If the new compound is a costing instance...
+    elif isinstance(cpd_new, (ExcelCost, ColabCost)):
+        # The value selection is a little different
+        cpd_name = cpd_new.final_prod
+        cpd_loc = (cpd_new._fp_idx, cpd_new.final_prod)
+        mw = cpd_new.fulldata.loc[cpd_loc, MAT_MW]
+        density = cpd_new.fulldata.loc[cpd_loc, MAT_DEN]
+        cost = cpd_new.fulldata.loc[cpd_loc, MAT_CST]
+    
+    # Else you've added the wrong kind of new compound
+    else:
+        raise ValueError("Oops!! Your new compound is not "
+                        "of the correct type.")
+
+    # Process the fulldata array
+    # First, remove the MultiIndex
+    fd_rst = model.fulldata.reset_index()
+    # Check for the requested compound
+    cpd_mask = fd_rst[RXN_CPD] == cpd_old
+    # If a particular step is chosen, select only that step
+    if step:
+        cpd_mask = cpd_mask & (fd_rst[RXN_STP] == str(step))
+
+    if not cpd_mask.any():
+        raise ValueError("Oops! '" + cpd_old + "' isn't in your "
+                        "current route.")
+    # Swap out the compound names
+    fd_rst.loc[cpd_mask, RXN_CPD] = cpd_name
+    # Reset index and fulldata attribute
+    model.fulldata = fd_rst.set_index([RXN_STP, RXN_CPD])
+
+    # Set the values using `value_mod`
+    model.value_mod(cpd_name, mw, val_type='MW', step=step)
+    model.value_mod(cpd_name, density, val_type='Density', step=step)
+    model.value_mod(cpd_name, cost, step=step)
+
+
+def sensitivity(model, col='Equiv', frac=0.1, decimals=2):
+    '''Do a sensitivity analysis for the equivalents of reagents.
+
+    Parameters
+    ----------
+    model : CoreCost or subclass
+        This is the costing model instance that will be modified.
         
-        if decimals:
-            return sens.round(decimals)
-        else:
-            return sens
+    col : str, optional (Default = 'Equiv')
+        Which column from the `fulldata` DataFrame should be used for the
+        sensitivity analysis. 
+
+    frac : float, optional (Default = 0.1)
+        Fractional percentage to increase/decrease the values by before
+        recosting. The default is 0.1, which is the same as +/- 10%. 
+
+    decimals : int or None, optional (Default = 2)
+        How many decimal places to display. If `None`, the full precision
+        DataFrame will be displayed.
+    '''
+    # Make a new DF for sensitivity analysis
+    # Make values that are a certain percent above and below the current
+    # numbers
+    sens = model.fulldata[[col]].dropna()
+    sens['Val low'] = sens[col]*(1 - frac)
+    sens['Val high'] = sens[col]*(1 + frac)
+    
+    # Re-run the costing under the current conditions, which resets the
+    # cost and fulldata variables. 
+    model.calc_cost()
+    # Make copies of these values so they don't change
+    cost_save = model.cost
+    fd_save = model.fulldata.copy()
+
+    # Loop through the values and calculate the cost if these values
+    # increase or decease by the percent given
+    for step_cpd, vals in sens.iterrows():
+        step, cpd = step_cpd
+        # Low values
+        model.value_mod(cpd, vals['Val low'], val_type=col, step=step)
+        model.calc_cost()
+        cost_low = model.cost
+        cost_low_per = (cost_low*100./cost_save) - 100
+        # Just to be safe - Drop the modified value
+        model._mod_vals.pop()
+
+        # High values
+        model.value_mod(cpd, vals['Val high'], val_type=col, step=step)
+        model.calc_cost()
+        cost_high = model.cost
+        cost_high_per = (cost_high*100./cost_save) - 100
+        model._mod_vals.pop()
+
+        # Set the values in the sensitivity DataFrame
+        sens.loc[(step, cpd), 'Cost low'] = cost_low
+        sens.loc[(step, cpd), 'Cost high'] = cost_high
+        sens.loc[(step, cpd), '% low'] = cost_low_per
+        sens.loc[(step, cpd), '% high'] = cost_high_per
+
+        # Reset the original values.  This is necessary so the next step
+        # in the loop starts from the original position.
+        model.cost = cost_save
+        model.fulldata = fd_save.copy()
+    
+    if decimals:
+        return sens.round(decimals)
+    else:
+        return sens
```

### Comparing `costcalc2-0.9.0/src/costcalc2.egg-info/PKG-INFO` & `costcalc2-0.9.1/src/costcalc2.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: costcalc2
-Version: 0.9.0
+Version: 0.9.1
 Summary: Calculate raw material costs for chemical synthetic route
 Author-email: Ryan Nelson <rnelsonchem@gmail.com>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/rnelsonchem/costcalc2
 Keywords: Chemical,Synthesis,Route,Cost,Pricing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,20 +12,28 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-# costcalc
+# costcalc2
 
-*costcalc* is a Python library for calculating the overall raw materials costs 
-of a user-defined synthetic route. This package is intended for Python 
-versions >= 3.
+*costcalc2* is a Python library for calculating the overall raw materials costs 
+of a user-defined synthetic route. 
 
 ## Requirements
 
 * Python >= 3
 * Numpy >= 1.0
 * Pandas >= 1.0
 * Matplotlib >= 3.0
 * Openpyxl >= 3.0
+
+# Web Application and Documentation
+
+A minimal [working web application](https://costcalc.rnelsonchem.com/) is
+available for running cost calculations without installing this package.
+However, for users that are interested in writing programs using `costcalc2`,
+there is an [annotated Jupyter
+notebook](https://gist.github.com/rnelsonchem/5f38f9f6261591a158ed06c643fe09e7)
+that demonstrates a common use case and most of the methods.
```

