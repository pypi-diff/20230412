# Comparing `tmp/inviz-0.0.4.tar.gz` & `tmp/inviz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.4.tar", last modified: Fri Apr  7 21:00:19 2023, max compression
+gzip compressed data, was "inviz-0.0.5.tar", last modified: Tue Apr 11 23:59:16 2023, max compression
```

## Comparing `inviz-0.0.4.tar` & `inviz-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 21:00:19.304737 inviz-0.0.4/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-04-07 20:46:41.000000 inviz-0.0.4/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-04-07 20:46:41.000000 inviz-0.0.4/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2606 2023-04-07 21:00:19.304737 inviz-0.0.4/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2036 2023-04-07 20:46:41.000000 inviz-0.0.4/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 21:00:19.304737 inviz-0.0.4/inviz/
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 21:00:19.304737 inviz-0.0.4/inviz/inviz.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2606 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      227 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       98 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/top_level.txt
--rwxrwxr-x   0 maamari   (1000) maamari   (1000)     9387 2023-04-07 20:46:42.000000 inviz-0.0.4/inviz/inviz.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-04-07 21:00:19.304737 inviz-0.0.4/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1162 2023-04-07 20:59:46.000000 inviz-0.0.4/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-11 23:59:16.950293 inviz-0.0.5/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-04-11 23:56:04.000000 inviz-0.0.5/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-04-11 23:56:04.000000 inviz-0.0.5/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     4045 2023-04-11 23:59:16.950293 inviz-0.0.5/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     3475 2023-04-11 23:56:04.000000 inviz-0.0.5/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-11 23:59:16.950293 inviz-0.0.5/inviz/
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-11 23:59:16.950293 inviz-0.0.5/inviz/inviz.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     4045 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      227 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       98 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/top_level.txt
+-rwxrwxr-x   0 maamari   (1000) maamari   (1000)     9933 2023-04-11 23:56:05.000000 inviz-0.0.5/inviz/inviz.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-04-11 23:59:16.950293 inviz-0.0.5/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1162 2023-04-11 23:58:38.000000 inviz-0.0.5/setup.py
```

### Comparing `inviz-0.0.4/LICENSE` & `inviz-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.4/inviz/inviz.py` & `inviz-0.0.5/inviz/inviz.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from classy import Class
 import matplotlib.pyplot as plt
 import copy
 
 hv.extension('bokeh')
 hv.Store.set_current_backend('bokeh')
 pn.extension('tabulator')
+pn.extension(loading_spinner='dots', loading_color='#00aa41', sizing_mode="stretch_width")
 pn.extension()
 
 # read in the .paramnames file and put it into list format
 def load_params(filename):
     params_list = []
     with open(filename, 'r') as f:
         for line in f:
@@ -35,15 +36,15 @@
 def load_data(filename, column_names):
     data = np.loadtxt(filename)
     df = pd.DataFrame(data[:,2:], columns=column_names)
     return df
 
 
 # generate a scatter plot using the key dimensions from a holoviews.Dataset object, with the CLASS output displayed alongside it
-def viz(dataset, dataframe):
+def viz(data, data_classy_input, data_classy_CDM, class_enabled):
     # function for generating the scatter plot, given 2 dimensions as x and y axes, and an additional dimension to colormap
     # to the points on the plot. Also has an option to show or hide the colormap
     def plot_data(kdim1, kdim2, colordim, showcmap):
         if showcmap == True:
             cmapping = opts.Points(color=dim(colordim),
                 colorbar=True,
                 cmap='Viridis')
@@ -52,20 +53,20 @@
         hover = HoverTool(tooltips=None)
         popts = opts.Points(
             toolbar='above',
             #line_color='black',
             #alpha=0.75, selection_alpha=1, nonselection_alpha=0.1,
             tools=[hover, 'box_select','lasso_select','tap'],
             size=7)
-        points = hv.Points(dataframe, kdims=[kdim1, kdim2]).opts(popts, cmapping)
+        points = hv.Points(data, kdims=[kdim1, kdim2]).opts(popts, cmapping)
         return points
     
     
     # setting Panel widgets for user interaction
-    variables = dataframe.columns.values.tolist()
+    variables = data.columns.values.tolist()
     var1 = pn.widgets.Select(value=variables[0], name='Horizontal Axis', options=variables)
     var2 = pn.widgets.Select(value=variables[1], name='Vertical Axis', options=variables)
     cmap_var = pn.widgets.Select(value=variables[2], name='Colormapped Parameter', options=variables)
     cmap_option = pn.widgets.Checkbox(value=True, name='Show Colormap', align='end')
     
     # bind the widget values to the plotting function so it gets called every time the user interacts with the widget
     # call the bound plotting function inside a holoview DynamicMap object for interaction
@@ -73,28 +74,30 @@
     points_dmap = hv.DynamicMap(interactive_points, kdims=[]).opts(width=500, height=400, framewise=True)
     
     # define a stream to get a list of all the points the user has selected on the plot
     selection = streams.Selection1D(source=points_dmap)
     
     # function to generate a table of all the selected points
     def make_table(kdim1, kdim2, colordim):
-        table = hv.DynamicMap(lambda index: hv.Table(dataframe.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
+        table = hv.DynamicMap(lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
         # formatting the table using plot hooks and a holoviews Options object
         def hook(plot, element):
             plot.handles['table'].autosize_mode = "none"
             for column in plot.handles['table'].columns:
                 column.width = 100
             
         table_options = opts.Table(height=300, width=1000, hooks=[hook])
         return table.opts(table_options).relabel('Selected Points')
     
     
     # generate the table
     selected_table = pn.bind(make_table, kdim1=var1, kdim2=var2, colordim=cmap_var)
     
+    #table_stream = streams.Selection1D(source=selected_table)
+    
     # function to run CLASS on data from the selection. 
     # first create an empty plot to handle the null selection case
     empty_plot = hv.Curve(np.random.rand(0, 2))
     def run_class_on_selection(index):
         if not index:
             empty_pk = empty_plot.relabel('P(k) Residuals - no selection').opts(
                 xlabel=r'$$k~[h/\mathrm{Mpc}]$$', 
@@ -104,39 +107,40 @@
                 ylabel=r"$$(C_{\ell}^{TT} - C_{\ell, CDM}^{TT})/C_{\ell, CDM}^{TT}*100~[\%]$$")
             empty_cl_ee = empty_plot.relabel('Lensed Cl_EE Residuals - no selection').opts(
                 xlabel=r"$$\ell$$", 
                 ylabel=r"$$(C_{\ell}^{EE} - C_{\ell, CDM}^{EE})/C_{\ell, CDM}^{EE}*100~[\%]$$")
             empty_layout = empty_pk + empty_cl_tt + empty_cl_ee            
             return empty_layout
 
-        # the Selection1D stream returns a dict. turn it into a list
-        sel = df.iloc[index]
-        sel_dict_list = sel.to_dict('records')
-        CDM_dict_list = []
+        # the Selection1D stream returns an index number. index into the approprate dataframe and turn it into a dictionary for CLASS to read
+        selection = data_classy_input.iloc[index]
+        selection_CDM = data_classy_CDM.iloc[index]
+        sel_dict_list = selection.to_dict('records')
+        CDM_dict_list = selection_CDM.to_dict('records')
         
         # remove nuisance parameters and add some project-specific ones. in the future these will be defined by the user
-        for i in range(len(sel_dict_list)):
-            entries_to_remove1 = ('z_reio', 'A_s', 'sigma8', '100theta_s', 'A_cib_217', 'xi_sz_cib', 'A_sz', 'ps_A_100_100', 'ps_A_143_143', 'ps_A_143_217', 'ps_A_217_217', 'ksz_norm', 
-                                 'gal545_A_100', 'gal545_A_143', 'gal545_A_143_217', 'gal545_A_217', 'galf_TE_A_100', 'galf_TE_A_100_143', 'galf_TE_A_100_217', 'galf_TE_A_143', 'galf_TE_A_143_217', 
-                                 'galf_TE_A_217', 'calib_100T', 'calib_217T', 'A_planck' )
-            for j in entries_to_remove1:
-                sel_dict_list[i].pop(j, None)
-
-            sel_dict_list[i]['omega_b'] = sel_dict_list[i]['omega_b']*1e-2
-            sel_dict_list[i]['sigma_dmeff'] = sel_dict_list[i]['sigma_dmeff']*1e-25
-            sel_dict_list[i]['h'] = (sel_dict_list[i].pop('H0'))*1e-2
-            sel_dict_list[i].update({"omega_cdm":1e-15, "npow_dmeff": 0, "Vrel_dmeff": 0, "dmeff_target": "baryons", "m_dmeff": 1e-3})
-
-        for k in range(len(sel_dict_list)):
-            params_CDM = copy.deepcopy(sel_dict_list[k])
-            entries_to_remove2 = ('sigma_dmeff', 'npow_dmeff', 'Vrel_dmeff', 'dmeff_target', 'm_dmeff')
-            for l in entries_to_remove2:
-                params_CDM.pop(l, None)
-            params_CDM['omega_cdm'] = params_CDM.pop('omega_dmeff')
-            CDM_dict_list.append(params_CDM)
+#         for i in range(len(sel_dict_list)):
+#             entries_to_remove1 = ('z_reio', 'A_s', 'sigma8', '100theta_s', 'A_cib_217', 'xi_sz_cib', 'A_sz', 'ps_A_100_100', 'ps_A_143_143', 'ps_A_143_217', 'ps_A_217_217', 'ksz_norm', 
+#                                  'gal545_A_100', 'gal545_A_143', 'gal545_A_143_217', 'gal545_A_217', 'galf_TE_A_100', 'galf_TE_A_100_143', 'galf_TE_A_100_217', 'galf_TE_A_143', 'galf_TE_A_143_217', 
+#                                  'galf_TE_A_217', 'calib_100T', 'calib_217T', 'A_planck' )
+#             for j in entries_to_remove1:
+#                 sel_dict_list[i].pop(j, None)
+
+#             sel_dict_list[i]['omega_b'] = sel_dict_list[i]['omega_b']*1e-2
+#             sel_dict_list[i]['sigma_dmeff'] = sel_dict_list[i]['sigma_dmeff']*1e-25
+#             sel_dict_list[i]['h'] = (sel_dict_list[i].pop('H0'))*1e-2
+#             sel_dict_list[i].update({"omega_cdm":1e-15, "npow_dmeff": 0, "Vrel_dmeff": 0, "dmeff_target": "baryons", "m_dmeff": 1e-3})
+
+#         for k in range(len(sel_dict_list)):
+#             params_CDM = copy.deepcopy(sel_dict_list[k])
+#             entries_to_remove2 = ('sigma_dmeff', 'npow_dmeff', 'Vrel_dmeff', 'dmeff_target', 'm_dmeff')
+#             for l in entries_to_remove2:
+#                 params_CDM.pop(l, None)
+#             params_CDM['omega_cdm'] = params_CDM.pop('omega_dmeff')
+#             CDM_dict_list.append(params_CDM)
 
         # run class on the user's selection
         cosmo = Class()
         cosmo.set(sel_dict_list[0])
         cosmo.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
         cosmo.compute()
 
@@ -161,15 +165,15 @@
         Pk_CDM = []
         h = cosmo_CDM.h()
         for k in kk:
             Pk_CDM.append(cosmo_CDM.pk(k*h,0.)*h**3)
 
         lensed_cl_CDM = cosmo_CDM.lensed_cl(2500)
 
-        # compute residuals and plot them
+        # compute residuals
         pk_residuals = (np.array(Pk1) - np.array(Pk_CDM))/np.array(Pk_CDM)*100
         cl_tt_residuals = (lensed_cl['tt'][2:] - lensed_cl_CDM['tt'][2:])/(lensed_cl_CDM['tt'][2:])*100
         cl_ee_residuals = (lensed_cl['ee'][2:] - lensed_cl_CDM['ee'][2:])/(lensed_cl_CDM['ee'][2:])*100
 
         plot_pk_residuals = hv.Curve((kk, pk_residuals)).relabel('P(k) Residuals').opts(
             xlabel=r'$$k~[h/\mathrm{Mpc}]$$', 
             ylabel=r'$$(P(k)-P_{CDM}(k))/P_{CDM}(k)*100~[\%]$$')
@@ -181,16 +185,18 @@
         plot_cl_ee_residuals = hv.Curve((l,cl_ee_residuals)).relabel('Cl_EE Residuals').opts(
             xlabel=r"$$\ell$$", 
             ylabel=r"$$(C_{\ell}^{EE}-C_{\ell, CDM}^{EE})/C_{\ell, CDM}^{EE}*100~[\%]$$")
         
         layout = (plot_pk_residuals + plot_cl_tt_residuals + plot_cl_ee_residuals)
         return layout
     
-
-    classy_output = hv.DynamicMap(run_class_on_selection, streams=[selection]).opts(
-        opts.Curve(color='black', logx=True, width=500, height=400, padding=0.1, framewise=True),
-        opts.Layout(shared_axes=False))
-
     # put it all together using Panel
-    points_display = pn.Column(pn.Row(var1, var2, cmap_var, cmap_option), pn.Row(points_dmap, selected_table))
-    dashboard = pn.Column(points_display, classy_output)
+    dashboard = pn.Column(pn.Row(var1, var2, cmap_var, cmap_option), pn.Row(points_dmap, selected_table))
+
+    if class_enabled == True:
+        classy_output = hv.DynamicMap(run_class_on_selection, streams=[selection]).opts(
+            opts.Curve(color='black', logx=True, width=500, height=400, padding=0.1, framewise=True),
+            opts.Layout(shared_axes=False))
+        classy_output_pane = pn.panel(classy_output)
+        # pn.param.set_values(classy_output_pane, loading=True)
+        dashboard = pn.Column(dashboard, classy_output_pane)
     return dashboard
```

### Comparing `inviz-0.0.4/setup.py` & `inviz-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.4",
+    version = "0.0.5",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
```

