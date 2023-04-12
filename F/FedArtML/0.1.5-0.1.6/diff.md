# Comparing `tmp/FedArtML-0.1.5.tar.gz` & `tmp/FedArtML-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FedArtML-0.1.5.tar", last modified: Tue Mar 14 09:08:20 2023, max compression
+gzip compressed data, was "dist\FedArtML-0.1.6.tar", last modified: Wed Apr 12 13:51:16 2023, max compression
```

## Comparing `FedArtML-0.1.5.tar` & `FedArtML-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 09:08:20.000000 FedArtML-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-03-14 09:08:20.000000 FedArtML-0.1.5/FedArtML.egg-info/
--rw-rw-rw-   0        0        0     1533 2023-03-14 09:08:20.000000 FedArtML-0.1.5/FedArtML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-14 09:08:20.000000 FedArtML-0.1.5/FedArtML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 09:08:20.000000 FedArtML-0.1.5/FedArtML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-14 09:08:20.000000 FedArtML-0.1.5/FedArtML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-14 09:08:20.000000 FedArtML-0.1.5/FedArtML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1533 2023-03-14 09:08:20.000000 FedArtML-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      754 2023-03-12 08:52:53.000000 FedArtML-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 09:08:20.000000 FedArtML-0.1.5/fedartml/
--rw-rw-rw-   0        0        0      178 2022-11-24 21:44:10.000000 FedArtML-0.1.5/fedartml/__init__.py
--rw-rw-rw-   0        0        0    39090 2023-03-14 08:54:06.000000 FedArtML-0.1.5/fedartml/fl_interactive_plots.py
--rw-rw-rw-   0        0        0    12400 2023-03-14 08:34:51.000000 FedArtML-0.1.5/fedartml/fl_split_as_federated_data.py
--rw-rw-rw-   0        0        0     4601 2023-03-14 08:45:11.000000 FedArtML-0.1.5/fedartml/function_base.py
--rw-rw-rw-   0        0        0       42 2023-03-14 09:08:20.000000 FedArtML-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-03-14 09:03:37.000000 FedArtML-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:51:16.000000 FedArtML-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-04-12 13:51:16.000000 FedArtML-0.1.6/FedArtML.egg-info/
+-rw-rw-rw-   0        0        0     3713 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3713 2023-04-12 13:51:16.000000 FedArtML-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2838 2023-04-12 13:08:21.000000 FedArtML-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 13:51:16.000000 FedArtML-0.1.6/fedartml/
+-rw-rw-rw-   0        0        0      178 2022-11-24 21:44:10.000000 FedArtML-0.1.6/fedartml/__init__.py
+-rw-rw-rw-   0        0        0    40870 2023-04-12 13:30:25.000000 FedArtML-0.1.6/fedartml/fl_interactive_plots.py
+-rw-rw-rw-   0        0        0    20216 2023-04-12 13:37:42.000000 FedArtML-0.1.6/fedartml/fl_split_as_federated_data.py
+-rw-rw-rw-   0        0        0     5701 2023-03-30 06:01:03.000000 FedArtML-0.1.6/fedartml/function_base.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:51:16.000000 FedArtML-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-04-12 13:49:49.000000 FedArtML-0.1.6/setup.py
```

### Comparing `FedArtML-0.1.5/fedartml/fl_interactive_plots.py` & `FedArtML-0.1.6/fedartml/fl_interactive_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Importing libraries
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticker
 import numpy as np
 import pandas as pd
 from ipywidgets import interact, Layout, IntSlider, FloatLogSlider, FloatSlider
-from numpy.random import dirichlet
 
 from fedartml.function_base import jensen_shannon_distance, hellinger_distance, earth_movers_distance, get_spaced_colors
 from fedartml.fl_split_as_federated_data import SplitAsFederatedData
 from sklearn import preprocessing
 
 
 class InteractivePlots:
@@ -21,19 +20,22 @@
         labels : array-like
             The target values (class labels in classification).
         random_state : int
             Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
             output across multiple function calls.
         colors : list
             Colors list used to plot. Must have a length of 7 positions.
+        distance : str
+            Distance to use for measuring heterogeneity (non-IID-ness) of the label's distribution among clients.
+            Possible choices: "jensen-shannon", "hellinger", "earth_movers".
         **plot_kwargs : dict
             Keyword arguments used for customizing plots (inherited from matplotlib.pyplot).
     """
 
-    def __init__(self, labels, random_state=None, colors=None, distance ="jensen-shannon", **plot_kwargs):
+    def __init__(self, labels, random_state=None, colors=None, distance="jensen-shannon", **plot_kwargs):
         if colors is None:
             colors = ["#00cfcc", "#e6013b", "#007f88", "#00cccd", "#69e0da", "darkblue", "#FFFFFF"]
         self.labels = labels
         self.n_classes = len(np.unique(labels))
         self.random_state = random_state
         self.colors = colors
         self.distance = distance
@@ -42,15 +44,15 @@
     def stacked_distr_dirichlet(self, Alpha, Local_Nodes):
         """
         Create an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
 
             Parameters
             ----------
             Alpha : slider
-                Parameter of the Dirichlet distribution (length k for sample of length k).
+                Concentration parameter of the Dirichlet distribution.
             Local_Nodes : slider
                 Number of local nodes (clients) used in the federated learning paradigm.
 
             Raises
             ------
 
             Returns
@@ -71,26 +73,29 @@
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
 
         # Get random Dirichlet distribution
         lbl_distro_clients_pctg, lbl_distro_clients_num, lbl_distro_clients_idx, num_per_node = \
-            SplitAsFederatedData.dirichlet_method(self, labels_encoded, Local_Nodes, alpha=Alpha
-                                                  , random_state=self.random_state)
+            SplitAsFederatedData.dirichlet_method(self, labels_encoded, Local_Nodes, alpha=Alpha,
+                                                  random_state=self.random_state)
         # Calculate desired distance
         if self.distance == "jensen-shannon":
             dist_select = jensen_shannon_distance(lbl_distro_clients_pctg)
             text_dist = "Jensen-Shannon"
         elif self.distance == "hellinger":
             dist_select = hellinger_distance(lbl_distro_clients_pctg)
             text_dist = "Hellinger"
-        else:
+        elif self.distance == "earth_movers":
             dist_select = earth_movers_distance(lbl_distro_clients_pctg)
             text_dist = "Earth Mover’s"
+        else:
+            raise ValueError("Distance '" + self.distance + "' not implemented. Available distances are: ["
+                                                            "'jensen-shannon', 'hellinger', 'earth_movers']")
 
         # Defne dataframe to plot
         df_simul = pd.DataFrame(lbl_distro_clients_pctg).reset_index()
         df_simul = df_simul * 100
         df_simul['index'] = (df_simul['index'] / 100 + 1).astype(int)
         df_simul.columns = ['Local Node'] + list(np.unique(self.labels))
 
@@ -103,17 +108,17 @@
                                           {'title': 'Classes', 'title_fontsize': 14, 'loc': 'center left',
                                            'bbox_to_anchor': (1.0, 0.5), 'fontsize': 12}))
         plt.xlabel(**self.plot_kwargs.get('stack_xlabel_kwargs', {'xlabel': 'Local Node', 'fontsize': 20}))
         plt.ylabel(**self.plot_kwargs.get('stack_ylabel_kwargs', {'ylabel': 'Participation (%)', 'fontsize': 20}))
         plt.title(**self.plot_kwargs.get('stack_title_kwargs',
                                          {'label': "Label's classes distribution across local nodes", 'fontsize': 25}))
         plt.text(s=text_dist + " dist. = " + str(round(dist_select, 2)),
-                 **self.plot_kwargs.get('stack_text_JSD_kwargs', {'x': -0.3, 'y': 103.5, 'fontsize': 20,
-                                                                  'backgroundcolor': self.colors[2],
-                                                                  'color': self.colors[6]}))
+                 **self.plot_kwargs.get('stack_text_DIST_kwargs', {'x': -0.3, 'y': 103.5, 'fontsize': 20,
+                                                                   'backgroundcolor': self.colors[2],
+                                                                   'color': self.colors[6]}))
         plt.show()
 
         return ()
 
     def show_stacked_distr_dirichlet(self, **slider_kwargs):
         """
         Show an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
@@ -131,25 +136,23 @@
             The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
 
             See Also
             --------
 
             References
             ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust
-            Model Fusion in Federated Learning
+            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
                    https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
 
             Examples
             --------
             >>> from fedartml import InteractivePlots
             >>> from keras.datasets import mnist
             >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_labels = train_y
-            >>> my_plot = InteractivePlots(labels = my_labels)
+            >>> my_plot = InteractivePlots(labels = train_y)
             >>> my_plot.show_stacked_distr_dirichlet()
         """
         interact(self.stacked_distr_dirichlet,
                  Alpha=FloatLogSlider(**slider_kwargs.get('alpha_slider_kwargs',
                                                           {'min': -2, 'max': 3, 'value': 1000, 'readout_format': '.4'}),
                                       layout=Layout(
                                           **slider_kwargs.get('alpha_slider_lout_kwargs', {'width': '1000px'}))),
@@ -162,15 +165,15 @@
     def scatter_distr_dirichlet(self, Alpha, Local_Nodes):
         """
         Create an interactive scatter plot (with sliders) per each local node (client) and label's classes.
 
             Parameters
             ----------
             Alpha : slider
-                Parameter of the Dirichlet distribution (length k for sample of length k).
+                Concentration parameter of the Dirichlet distribution.
             Local_Nodes : slider
                 Number of local nodes (clients) used in the federated learning paradigm.
 
             Raises
             ------
 
             Returns
@@ -191,26 +194,29 @@
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
 
         # Get random Dirichlet distribution
         lbl_distro_clients_pctg, lbl_distro_clients_num, lbl_distro_clients_idx, num_per_node = \
-            SplitAsFederatedData.dirichlet_method(self, labels_encoded, Local_Nodes, alpha=Alpha
-                                                  , random_state=self.random_state)
+            SplitAsFederatedData.dirichlet_method(self, labels_encoded, Local_Nodes, alpha=Alpha,
+                                                  random_state=self.random_state)
         # Calculate desired distance
         if self.distance == "jensen-shannon":
             dist_select = jensen_shannon_distance(lbl_distro_clients_pctg)
             text_dist = "Jensen-Shannon"
         elif self.distance == "hellinger":
             dist_select = hellinger_distance(lbl_distro_clients_pctg)
             text_dist = "Hellinger"
-        else:
+        elif self.distance == "earth_movers":
             dist_select = earth_movers_distance(lbl_distro_clients_pctg)
             text_dist = "Earth Mover’s"
+        else:
+            raise ValueError("Distance '" + self.distance + "' not implemented. Available distances are: ["
+                                                            "'jensen-shannon', 'hellinger', 'earth_movers']")
 
         # Defne dataframe to plot
         df_simul = pd.DataFrame(num_per_node).reset_index()
         df_simul['index'] = (df_simul['index'] + 1).astype(int)
         df_simul.columns = ['Local Node'] + list(np.unique(self.labels))
         df_simul_long = pd.melt(df_simul, id_vars='Local Node',
                                 value_vars=list(df_simul.columns[df_simul.columns != 'Local Node']))
@@ -226,15 +232,15 @@
                                                                                   'color': self.colors[0]}))
         plt.xlabel(**self.plot_kwargs.get('scatter_xlabel_kwargs', {'xlabel': 'Local Node', 'fontsize': 20}))
         plt.ylabel(**self.plot_kwargs.get('scatter_ylabel_kwargs', {'ylabel': 'Classes', 'fontsize': 20}))
         plt.title(**self.plot_kwargs.get('scatter_title_kwargs',
                                          {'label': "Number of examples across classes and local nodes",
                                           'fontsize': 25}))
         plt.text(s=text_dist + " dist. = " + str(round(dist_select, 2)),
-                 **self.plot_kwargs.get('scatter_text_JSD_kwargs',
+                 **self.plot_kwargs.get('scatter_text_DIST_kwargs',
                                         {'x': 0.6, 'y': len(np.unique(self.labels)), 'fontsize': 20,
                                          'backgroundcolor': self.colors[2], 'color': self.colors[6]}))
         plt.gca().xaxis.set_major_locator(mticker.MultipleLocator(1))
 
         plt.show()
 
         return ()
@@ -256,26 +262,24 @@
             The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
 
             See Also
             --------
 
             References
             ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust
-            Model Fusion in Federated Learning
+            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
                    https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
 
             Examples
             --------
             >>> from fedartml import InteractivePlots
             >>> from keras.datasets import mnist
             >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_labels = train_y
-            >>> my_plot = InteractivePlots(labels = my_labels)
-            >>> my_plot.show_stacked_distr_dirichlet()
+            >>> my_plot = InteractivePlots(labels = train_y)
+            >>> my_plot.show_scatter_distr_dirichlet()
         """
         interact(self.scatter_distr_dirichlet,
                  Alpha=FloatLogSlider(**slider_kwargs.get('alpha_slider_kwargs',
                                                           {'min': -2, 'max': 3, 'value': 1000, 'readout_format': '.4'}),
                                       layout=Layout(
                                           **slider_kwargs.get('alpha_slider_lout_kwargs', {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
@@ -287,15 +291,15 @@
     def bar_divided_distr_dirichlet(self, Alpha, Local_Nodes):
         """
         Create an interactive bar plot (with sliders) divided per each local node (client).
 
             Parameters
             ----------
             Alpha : slider
-                Parameter of the Dirichlet distribution (length k for sample of length k).
+                Concentration parameter of the Dirichlet distribution.
             Local_Nodes : slider
                 Number of local nodes (clients) used in the federated learning paradigm.
 
             Raises
             ------
 
             Returns
@@ -316,27 +320,30 @@
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
 
         # Get random Dirichlet distribution
         lbl_distro_clients_pctg, lbl_distro_clients_num, lbl_distro_clients_idx, num_per_node = \
-            SplitAsFederatedData.dirichlet_method(self, labels_encoded, Local_Nodes, alpha=Alpha
-                                                  , random_state=self.random_state)
-
+            SplitAsFederatedData.dirichlet_method(self, labels_encoded, Local_Nodes, alpha=Alpha,
+                                                  random_state=self.random_state)
         # Calculate desired distance
         if self.distance == "jensen-shannon":
             dist_select = jensen_shannon_distance(lbl_distro_clients_pctg)
             text_dist = "Jensen-Shannon"
         elif self.distance == "hellinger":
             dist_select = hellinger_distance(lbl_distro_clients_pctg)
             text_dist = "Hellinger"
-        else:
+        elif self.distance == "earth_movers":
             dist_select = earth_movers_distance(lbl_distro_clients_pctg)
             text_dist = "Earth Mover’s"
+        else:
+            raise ValueError("Distance '" + self.distance + "' not implemented. Available distances are: ["
+                                                            "'jensen-shannon', 'hellinger', 'earth_movers']")
+
         # Defne dataframe to plot
         df_simul = pd.DataFrame(num_per_node)
         df_simul = df_simul.div(df_simul.sum(axis=1), axis=0).reset_index()
         df_simul = df_simul * 100
         df_simul['index'] = (df_simul['index'] / 100 + 1).astype(int)
         df_simul.columns = ['Local Node'] + list(np.unique(self.labels))
         df_simul_long = pd.melt(df_simul, id_vars='Local Node',
@@ -368,15 +375,15 @@
             plt.yticks(**self.plot_kwargs.get('bar_div_yticks_kwargs', {'fontsize': 30}))
             plt.xlim(
                 **self.plot_kwargs.get('bar_div_xlim_kwargs', {'left': 0, 'right': max(df_simul_long['value']) + 1}))
 
             # Increase counter
             cont += 1
 
-        f.text(**self.plot_kwargs.get('bar_div_text_kwargs',
+        f.text(**self.plot_kwargs.get('bar_div_text_DIST_kwargs',
                                       {'x': 0.5, 'y': 0.97, 'ha': 'center', 'va': 'top', 'fontsize': 60,
                                        's': text_dist + " dist. = " + str(round(dist_select, 2)),
                                        'color': self.colors[6], 'backgroundcolor': self.colors[2]}))
         plt.show()
 
         return ()
 
@@ -397,26 +404,24 @@
             The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
 
             See Also
             --------
 
             References
             ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust
-            Model Fusion in Federated Learning
+            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
                    https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
 
             Examples
             --------
             >>> from fedartml import InteractivePlots
             >>> from keras.datasets import mnist
             >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_labels = train_y
-            >>> my_plot = InteractivePlots(labels = my_labels)
-            >>> my_plot.show_stacked_distr_dirichlet()
+            >>> my_plot = InteractivePlots(labels = train_y)
+            >>> my_plot.show_bar_divided_distr_dirichlet()
         """
         interact(self.bar_divided_distr_dirichlet,
                  Alpha=FloatLogSlider(**slider_kwargs.get('alpha_slider_kwargs',
                                                           {'min': -2, 'max': 3, 'value': 1000, 'readout_format': '.4'}),
                                       layout=Layout(
                                           **slider_kwargs.get('alpha_slider_lout_kwargs', {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
@@ -428,15 +433,15 @@
     def stacked_distr_percent_noniid(self, Pctg_NonIID, Local_Nodes):
         """
         Create an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
 
             Parameters
             ----------
             Pctg_NonIID : slider
-                Percentage (between o and 100) desired of Non IID for the federated data.
+                Percentage (between o and 100) desired of non-IID-ness for the federated data.
             Local_Nodes : slider
                 Number of local nodes (clients) used in the federated learning paradigm.
 
             Raises
             ------
 
             Returns
@@ -457,26 +462,29 @@
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
 
         # Get Percentage of NonIID method
         lbl_distro_clients_pctg, lbl_distro_clients_num, lbl_distro_clients_idx, num_per_node = \
-            SplitAsFederatedData.percent_noniid_method(self, labels_encoded, Local_Nodes, pct_noniid=Pctg_NonIID
-                                                       , random_state=self.random_state)
+            SplitAsFederatedData.percent_noniid_method(self, labels_encoded, Local_Nodes, pct_noniid=Pctg_NonIID,
+                                                       random_state=self.random_state)
         # Calculate desired distance
         if self.distance == "jensen-shannon":
             dist_select = jensen_shannon_distance(lbl_distro_clients_pctg)
             text_dist = "Jensen-Shannon"
         elif self.distance == "hellinger":
             dist_select = hellinger_distance(lbl_distro_clients_pctg)
             text_dist = "Hellinger"
-        else:
+        elif self.distance == "earth_movers":
             dist_select = earth_movers_distance(lbl_distro_clients_pctg)
             text_dist = "Earth Mover’s"
+        else:
+            raise ValueError("Distance '" + self.distance + "' not implemented. Available distances are: ["
+                                                            "'jensen-shannon', 'hellinger', 'earth_movers']")
 
         # Defne dataframe to plot
         df_simul = pd.DataFrame(lbl_distro_clients_pctg).reset_index()
         df_simul = df_simul * 100
         df_simul['index'] = (df_simul['index'] / 100 + 1).astype(int)
         df_simul.columns = ['Local Node'] + list(np.unique(self.labels))
 
@@ -489,17 +497,17 @@
                                           {'title': 'Classes', 'title_fontsize': 14, 'loc': 'center left',
                                            'bbox_to_anchor': (1.0, 0.5), 'fontsize': 12}))
         plt.xlabel(**self.plot_kwargs.get('stack_xlabel_kwargs', {'xlabel': 'Local Node', 'fontsize': 20}))
         plt.ylabel(**self.plot_kwargs.get('stack_ylabel_kwargs', {'ylabel': 'Participation (%)', 'fontsize': 20}))
         plt.title(**self.plot_kwargs.get('stack_title_kwargs',
                                          {'label': "Label's classes distribution across local nodes", 'fontsize': 25}))
         plt.text(s=text_dist + " dist. = " + str(round(dist_select, 2)),
-                 **self.plot_kwargs.get('stack_text_JSD_kwargs', {'x': -0.3, 'y': 103.5, 'fontsize': 20,
-                                                                  'backgroundcolor': self.colors[2],
-                                                                  'color': self.colors[6]}))
+                 **self.plot_kwargs.get('stack_text_DIST_kwargs', {'x': -0.3, 'y': 103.5, 'fontsize': 20,
+                                                                   'backgroundcolor': self.colors[2],
+                                                                   'color': self.colors[6]}))
         plt.show()
 
         return ()
 
     def show_stacked_distr_percent_noniid(self, **slider_kwargs):
         """
         Show an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
@@ -510,54 +518,54 @@
                 Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
 
             Raises
             ------
 
             Returns
             -------
-            The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
+            The return keyword is empty. The function shows the sliders for Pctg_noniid and number of local nodes
+            (clients).
 
             See Also
             --------
 
             References
             ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust
-            Model Fusion in Federated Learning
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+            .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
 
             Examples
             --------
             >>> from fedartml import InteractivePlots
             >>> from keras.datasets import mnist
             >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_labels = train_y
-            >>> my_plot = InteractivePlots(labels = my_labels)
-            >>> my_plot.show_stacked_distr_dirichlet()
+            >>> my_plot = InteractivePlots(labels = train_y)
+            >>> my_plot.show_stacked_distr_percent_noniid()
         """
         interact(self.stacked_distr_percent_noniid,
                  Pctg_NonIID=FloatSlider(**slider_kwargs.get('pctg_noniid_slider_kwargs',
-                                                                {'min': 0, 'max': 100, 'value': 0,
-                                                                 'readout_format': '.4'}),
-                                            layout=Layout(
-                                                **slider_kwargs.get('pctg_noniid_slider_lout_kwargs', {'width': '1000px'}))),
+                                                             {'min': 0, 'max': 100, 'value': 0,
+                                                              'readout_format': '.4'}),
+                                         layout=Layout(
+                                             **slider_kwargs.get('pctg_noniid_slider_lout_kwargs',
+                                                                 {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
                                                                                        'value': 4}),
                                        layout=Layout(
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def scatter_distr_percent_noniid(self, Pctg_NonIID, Local_Nodes):
         """
         Create an interactive scatter plot (with sliders) per each local node (client) and label's classes.
 
             Parameters
             ----------
-            Alpha : slider
-                Parameter of the Dirichlet distribution (length k for sample of length k).
+            Pctg_NonIID : slider
+                Percentage (between o and 100) desired of non-IID-ness for the federated data.
             Local_Nodes : slider
                 Number of local nodes (clients) used in the federated learning paradigm.
 
             Raises
             ------
 
             Returns
@@ -578,26 +586,29 @@
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
 
         # Get Percentage of NonIID method
         lbl_distro_clients_pctg, lbl_distro_clients_num, lbl_distro_clients_idx, num_per_node = \
-            SplitAsFederatedData.percent_noniid_method(self, labels_encoded, Local_Nodes, pct_noniid=Pctg_NonIID
-                                                       , random_state=self.random_state)
+            SplitAsFederatedData.percent_noniid_method(self, labels_encoded, Local_Nodes, pct_noniid=Pctg_NonIID,
+                                                       random_state=self.random_state)
         # Calculate desired distance
         if self.distance == "jensen-shannon":
             dist_select = jensen_shannon_distance(lbl_distro_clients_pctg)
             text_dist = "Jensen-Shannon"
         elif self.distance == "hellinger":
             dist_select = hellinger_distance(lbl_distro_clients_pctg)
             text_dist = "Hellinger"
-        else:
+        elif self.distance == "earth_movers":
             dist_select = earth_movers_distance(lbl_distro_clients_pctg)
             text_dist = "Earth Mover’s"
+        else:
+            raise ValueError("Distance '" + self.distance + "' not implemented. Available distances are: ["
+                                                            "'jensen-shannon', 'hellinger', 'earth_movers']")
 
         # Defne dataframe to plot
         df_simul = pd.DataFrame(num_per_node).reset_index()
         df_simul['index'] = (df_simul['index'] + 1).astype(int)
         df_simul.columns = ['Local Node'] + list(np.unique(self.labels))
         df_simul_long = pd.melt(df_simul, id_vars='Local Node',
                                 value_vars=list(df_simul.columns[df_simul.columns != 'Local Node']))
@@ -613,15 +624,15 @@
                                                                                   'color': self.colors[0]}))
         plt.xlabel(**self.plot_kwargs.get('scatter_xlabel_kwargs', {'xlabel': 'Local Node', 'fontsize': 20}))
         plt.ylabel(**self.plot_kwargs.get('scatter_ylabel_kwargs', {'ylabel': 'Classes', 'fontsize': 20}))
         plt.title(**self.plot_kwargs.get('scatter_title_kwargs',
                                          {'label': "Number of examples across classes and local nodes",
                                           'fontsize': 25}))
         plt.text(s=text_dist + " dist. = " + str(round(dist_select, 2)),
-                 **self.plot_kwargs.get('scatter_text_JSD_kwargs',
+                 **self.plot_kwargs.get('scatter_text_DIST_kwargs',
                                         {'x': 0.6, 'y': len(np.unique(self.labels)), 'fontsize': 20,
                                          'backgroundcolor': self.colors[2], 'color': self.colors[6]}))
         plt.gca().xaxis.set_major_locator(mticker.MultipleLocator(1))
 
         plt.show()
 
         return ()
@@ -636,54 +647,54 @@
                 Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
 
             Raises
             ------
 
             Returns
             -------
-            The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
+            The return keyword is empty. The function shows the sliders for Pctg_NonIID and number of local nodes
+            (clients).
 
             See Also
             --------
 
             References
             ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust
-            Model Fusion in Federated Learning
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+            .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
 
             Examples
             --------
             >>> from fedartml import InteractivePlots
             >>> from keras.datasets import mnist
             >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_labels = train_y
-            >>> my_plot = InteractivePlots(labels = my_labels)
-            >>> my_plot.show_stacked_distr_dirichlet()
+            >>> my_plot = InteractivePlots(labels = train_y)
+            >>> my_plot.show_scatter_distr_percent_noniid()
         """
         interact(self.scatter_distr_percent_noniid,
                  Pctg_NonIID=FloatSlider(**slider_kwargs.get('pctg_noniid_slider_kwargs',
-                                                                {'min': 0, 'max': 100, 'value': 0,
-                                                                 'readout_format': '.4'}),
-                                      layout=Layout(
-                                          **slider_kwargs.get('pctg_noniid_slider_lout_kwargs', {'width': '1000px'}))),
+                                                             {'min': 0, 'max': 100, 'value': 0,
+                                                              'readout_format': '.4'}),
+                                         layout=Layout(
+                                             **slider_kwargs.get('pctg_noniid_slider_lout_kwargs',
+                                                                 {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
                                                                                        'value': 4}),
                                        layout=Layout(
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def bar_divided_distr_percent_noniid(self, Pctg_NonIID, Local_Nodes):
         """
         Create an interactive bar plot (with sliders) divided per each local node (client).
 
             Parameters
             ----------
-            Alpha : slider
-                Parameter of the Dirichlet distribution (length k for sample of length k).
+            Pctg_NonIID : slider
+                Percentage (between o and 100) desired of non-IID-ness for the federated data.
             Local_Nodes : slider
                 Number of local nodes (clients) used in the federated learning paradigm.
 
             Raises
             ------
 
             Returns
@@ -704,27 +715,29 @@
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
 
         # Get Percentage of NonIID method
         lbl_distro_clients_pctg, lbl_distro_clients_num, lbl_distro_clients_idx, num_per_node = \
-            SplitAsFederatedData.percent_noniid_method(self, labels_encoded, Local_Nodes, pct_noniid=Pctg_NonIID
-                                                       , random_state=self.random_state)
-
+            SplitAsFederatedData.percent_noniid_method(self, labels_encoded, Local_Nodes, pct_noniid=Pctg_NonIID,
+                                                       random_state=self.random_state)
         # Calculate desired distance
         if self.distance == "jensen-shannon":
             dist_select = jensen_shannon_distance(lbl_distro_clients_pctg)
             text_dist = "Jensen-Shannon"
         elif self.distance == "hellinger":
             dist_select = hellinger_distance(lbl_distro_clients_pctg)
             text_dist = "Hellinger"
-        else:
+        elif self.distance == "earth_movers":
             dist_select = earth_movers_distance(lbl_distro_clients_pctg)
             text_dist = "Earth Mover’s"
+        else:
+            raise ValueError("Distance '" + self.distance + "' not implemented. Available distances are: ["
+                                                            "'jensen-shannon', 'hellinger', 'earth_movers']")
 
         # Defne dataframe to plot
         df_simul = pd.DataFrame(num_per_node)
         df_simul = df_simul.div(df_simul.sum(axis=1), axis=0).reset_index()
         df_simul = df_simul * 100
         df_simul['index'] = (df_simul['index'] / 100 + 1).astype(int)
         df_simul.columns = ['Local Node'] + list(np.unique(self.labels))
@@ -757,15 +770,15 @@
             plt.yticks(**self.plot_kwargs.get('bar_div_yticks_kwargs', {'fontsize': 30}))
             plt.xlim(
                 **self.plot_kwargs.get('bar_div_xlim_kwargs', {'left': 0, 'right': max(df_simul_long['value']) + 1}))
 
             # Increase counter
             cont += 1
 
-        f.text(**self.plot_kwargs.get('bar_div_text_kwargs',
+        f.text(**self.plot_kwargs.get('bar_div_text_DIST_kwargs',
                                       {'x': 0.5, 'y': 0.97, 'ha': 'center', 'va': 'top', 'fontsize': 60,
                                        's': text_dist + " dist. = " + str(round(dist_select, 2)),
                                        'color': self.colors[6], 'backgroundcolor': self.colors[2]}))
         plt.show()
 
         return ()
 
@@ -779,38 +792,38 @@
                 Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
 
             Raises
             ------
 
             Returns
             -------
-            The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
+            The return keyword is empty. The function shows the sliders for Pctg_NonIID and number of local nodes
+            (clients).
 
             See Also
             --------
 
             References
             ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust
-            Model Fusion in Federated Learning
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+            .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
 
             Examples
             --------
             >>> from fedartml import InteractivePlots
             >>> from keras.datasets import mnist
             >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_labels = train_y
-            >>> my_plot = InteractivePlots(labels = my_labels)
-            >>> my_plot.show_stacked_distr_dirichlet()
+            >>> my_plot = InteractivePlots(labels = train_y)
+            >>> my_plot.show_bar_divided_distr_percent_noniid()
         """
         interact(self.bar_divided_distr_percent_noniid,
                  Pctg_NonIID=FloatSlider(**slider_kwargs.get('pctg_noniid_slider_kwargs',
                                                              {'min': 0, 'max': 100, 'value': 0,
-                                                                 'readout_format': '.4'}),
+                                                              'readout_format': '.4'}),
                                          layout=Layout(
-                                          **slider_kwargs.get('pctg_noniid_slider_lout_kwargs', {'width': '1000px'}))),
+                                             **slider_kwargs.get('pctg_noniid_slider_lout_kwargs',
+                                                                 {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
                                                                                        'value': 4}),
                                        layout=Layout(
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
```

### Comparing `FedArtML-0.1.5/setup.py` & `FedArtML-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="FedArtML",
-    version="0.1.5",
+    version="0.1.6",
     description="Federated learning for Artificial Intelligence and Machine Learning library ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
-    author="Daniel Mauricio Jimenez Gutierrez",
+    author="Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti",
     author_email="jimenezgutierrez@diag.uniroma1.it",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

