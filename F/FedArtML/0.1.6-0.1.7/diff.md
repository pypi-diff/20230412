# Comparing `tmp/FedArtML-0.1.6.tar.gz` & `tmp/FedArtML-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FedArtML-0.1.6.tar", last modified: Wed Apr 12 13:51:16 2023, max compression
+gzip compressed data, was "dist\FedArtML-0.1.7.tar", last modified: Wed Apr 12 14:36:13 2023, max compression
```

## Comparing `FedArtML-0.1.6.tar` & `FedArtML-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 13:51:16.000000 FedArtML-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-04-12 13:51:16.000000 FedArtML-0.1.6/FedArtML.egg-info/
--rw-rw-rw-   0        0        0     3713 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 13:51:15.000000 FedArtML-0.1.6/FedArtML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3713 2023-04-12 13:51:16.000000 FedArtML-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2838 2023-04-12 13:08:21.000000 FedArtML-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 13:51:16.000000 FedArtML-0.1.6/fedartml/
--rw-rw-rw-   0        0        0      178 2022-11-24 21:44:10.000000 FedArtML-0.1.6/fedartml/__init__.py
--rw-rw-rw-   0        0        0    40870 2023-04-12 13:30:25.000000 FedArtML-0.1.6/fedartml/fl_interactive_plots.py
--rw-rw-rw-   0        0        0    20216 2023-04-12 13:37:42.000000 FedArtML-0.1.6/fedartml/fl_split_as_federated_data.py
--rw-rw-rw-   0        0        0     5701 2023-03-30 06:01:03.000000 FedArtML-0.1.6/fedartml/function_base.py
--rw-rw-rw-   0        0        0       42 2023-04-12 13:51:16.000000 FedArtML-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-04-12 13:49:49.000000 FedArtML-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:36:13.000000 FedArtML-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/
+-rw-rw-rw-   0        0        0     3725 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 14:36:13.000000 FedArtML-0.1.7/FedArtML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3725 2023-04-12 14:36:13.000000 FedArtML-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2850 2023-04-12 14:34:59.000000 FedArtML-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:36:13.000000 FedArtML-0.1.7/fedartml/
+-rw-rw-rw-   0        0        0      178 2022-11-24 21:44:10.000000 FedArtML-0.1.7/fedartml/__init__.py
+-rw-rw-rw-   0        0        0    38522 2023-04-12 14:32:47.000000 FedArtML-0.1.7/fedartml/fl_interactive_plots.py
+-rw-rw-rw-   0        0        0    19440 2023-04-12 14:30:37.000000 FedArtML-0.1.7/fedartml/fl_split_as_federated_data.py
+-rw-rw-rw-   0        0        0     5701 2023-03-30 06:01:03.000000 FedArtML-0.1.7/fedartml/function_base.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:36:13.000000 FedArtML-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-04-12 14:35:41.000000 FedArtML-0.1.7/setup.py
```

### Comparing `FedArtML-0.1.6/FedArtML.egg-info/PKG-INFO` & `FedArtML-0.1.7/FedArtML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedArtML
-Version: 0.1.6
+Version: 0.1.7
 Summary: Federated learning for Artificial Intelligence and Machine Learning library 
 Home-page: 
 Author: Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti
 Author-email: jimenezgutierrez@diag.uniroma1.it
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -68,15 +68,15 @@
 x_train_glob, x_test_glob = x_train_glob / 255.0, x_test_glob / 255.0
 
 # Instantiate a SplitAsFederatedData object
 my_federater = SplitAsFederatedData(random_state = random_state)
 
 # Get federated dataset from centralized dataset
 clients_glob_dic, list_ids_sampled_dic, miss_class_per_node, distances = my_federater.create_clients(image_list = x_train_glob, label_list = y_train_glob, 
-                                                             num_clients = 2, prefix_cli='Local_node', method = "percent_noniid", percent_noniid = 2)
+                                                             num_clients = 2, prefix_cli='Local_node', method = "percent_noniid", percent_noniid = 50)
 ```
 
 You can also check broader guides to use this tool on the [examples](https://github.com/Sapienza-University-Rome/FedArtML/tree/master/examples) folder.
 
 ### Documentation
 Find the documentation of the library on:
-https://fedartml.readthedocs.io/en/latest/
+https://fedartml.readthedocs.io/en/latest/index.html#
```

### Comparing `FedArtML-0.1.6/PKG-INFO` & `FedArtML-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedArtML
-Version: 0.1.6
+Version: 0.1.7
 Summary: Federated learning for Artificial Intelligence and Machine Learning library 
 Home-page: 
 Author: Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti
 Author-email: jimenezgutierrez@diag.uniroma1.it
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -68,15 +68,15 @@
 x_train_glob, x_test_glob = x_train_glob / 255.0, x_test_glob / 255.0
 
 # Instantiate a SplitAsFederatedData object
 my_federater = SplitAsFederatedData(random_state = random_state)
 
 # Get federated dataset from centralized dataset
 clients_glob_dic, list_ids_sampled_dic, miss_class_per_node, distances = my_federater.create_clients(image_list = x_train_glob, label_list = y_train_glob, 
-                                                             num_clients = 2, prefix_cli='Local_node', method = "percent_noniid", percent_noniid = 2)
+                                                             num_clients = 2, prefix_cli='Local_node', method = "percent_noniid", percent_noniid = 50)
 ```
 
 You can also check broader guides to use this tool on the [examples](https://github.com/Sapienza-University-Rome/FedArtML/tree/master/examples) folder.
 
 ### Documentation
 Find the documentation of the library on:
-https://fedartml.readthedocs.io/en/latest/
+https://fedartml.readthedocs.io/en/latest/index.html#
```

### Comparing `FedArtML-0.1.6/README.md` & `FedArtML-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 x_train_glob, x_test_glob = x_train_glob / 255.0, x_test_glob / 255.0
 
 # Instantiate a SplitAsFederatedData object
 my_federater = SplitAsFederatedData(random_state = random_state)
 
 # Get federated dataset from centralized dataset
 clients_glob_dic, list_ids_sampled_dic, miss_class_per_node, distances = my_federater.create_clients(image_list = x_train_glob, label_list = y_train_glob, 
-                                                             num_clients = 2, prefix_cli='Local_node', method = "percent_noniid", percent_noniid = 2)
+                                                             num_clients = 2, prefix_cli='Local_node', method = "percent_noniid", percent_noniid = 50)
 ```
 
 You can also check broader guides to use this tool on the [examples](https://github.com/Sapienza-University-Rome/FedArtML/tree/master/examples) folder.
 
 ### Documentation
 Find the documentation of the library on:
-https://fedartml.readthedocs.io/en/latest/
+https://fedartml.readthedocs.io/en/latest/index.html#
```

### Comparing `FedArtML-0.1.6/fedartml/fl_interactive_plots.py` & `FedArtML-0.1.7/fedartml/fl_interactive_plots.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 
 class InteractivePlots:
     """
     Generate simulated interactive plots (with sliders) from the labels provided in a federated learning paradigm to
     exemplify identically and non-identically distributed labels across the local nodes (clients).
 
-        Parameters
-        ----------
-        labels : array-like
-            The target values (class labels in classification).
-        random_state : int
-            Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
-            output across multiple function calls.
-        colors : list
-            Colors list used to plot. Must have a length of 7 positions.
-        distance : str
-            Distance to use for measuring heterogeneity (non-IID-ness) of the label's distribution among clients.
-            Possible choices: "jensen-shannon", "hellinger", "earth_movers".
-        **plot_kwargs : dict
-            Keyword arguments used for customizing plots (inherited from matplotlib.pyplot).
+    Parameters
+    ----------
+    labels : array-like
+        The target values (class labels in classification).
+    random_state : int
+        Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
+        output across multiple function calls.
+    colors : list
+        Colors list used to plot. Must have a length of 7 positions.
+    distance : str
+        Distance to use for measuring heterogeneity (non-IID-ness) of the label's distribution among clients.
+        Possible choices: "jensen-shannon", "hellinger", "earth_movers".
+    **plot_kwargs : dict
+        Keyword arguments used for customizing plots (inherited from matplotlib.pyplot).
     """
 
     def __init__(self, labels, random_state=None, colors=None, distance="jensen-shannon", **plot_kwargs):
         if colors is None:
             colors = ["#00cfcc", "#e6013b", "#007f88", "#00cccd", "#69e0da", "darkblue", "#FFFFFF"]
         self.labels = labels
         self.n_classes = len(np.unique(labels))
@@ -41,36 +41,24 @@
         self.distance = distance
         self.plot_kwargs = plot_kwargs
 
     def stacked_distr_dirichlet(self, Alpha, Local_Nodes):
         """
         Create an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            Alpha : slider
-                Concentration parameter of the Dirichlet distribution.
-            Local_Nodes : slider
-                Number of local nodes (clients) used in the federated learning paradigm.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the plot as output.
-
-            See Also
-            --------
-
-            References
-            ----------
-
-            Examples
-            --------
+        Parameters
+        ----------
+        Alpha : slider
+            Concentration parameter of the Dirichlet distribution.
+        Local_Nodes : slider
+            Number of local nodes (clients) used in the federated learning paradigm.
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the plot as output.
         """
         labels_encoded = self.labels
 
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
@@ -119,41 +107,35 @@
 
         return ()
 
     def show_stacked_distr_dirichlet(self, **slider_kwargs):
         """
         Show an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            **slider_kwargs: dict
-                Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
-
-            See Also
-            --------
-
-            References
-            ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
-
-            Examples
-            --------
-            >>> from fedartml import InteractivePlots
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_plot = InteractivePlots(labels = train_y)
-            >>> my_plot.show_stacked_distr_dirichlet()
+        Parameters
+        ----------
+        **slider_kwargs: dict
+            Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
+
+        References
+        ----------
+        .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
+               https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+
+        Examples
+        --------
+        >>> from fedartml import InteractivePlots
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_plot = InteractivePlots(labels = train_y)
+        >>> my_plot.show_stacked_distr_dirichlet()
         """
         interact(self.stacked_distr_dirichlet,
                  Alpha=FloatLogSlider(**slider_kwargs.get('alpha_slider_kwargs',
                                                           {'min': -2, 'max': 3, 'value': 1000, 'readout_format': '.4'}),
                                       layout=Layout(
                                           **slider_kwargs.get('alpha_slider_lout_kwargs', {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
@@ -162,36 +144,24 @@
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def scatter_distr_dirichlet(self, Alpha, Local_Nodes):
         """
         Create an interactive scatter plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            Alpha : slider
-                Concentration parameter of the Dirichlet distribution.
-            Local_Nodes : slider
-                Number of local nodes (clients) used in the federated learning paradigm.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the plot as output.
-
-            See Also
-            --------
-
-            References
-            ----------
-
-            Examples
-            --------
+        Parameters
+        ----------
+        Alpha : slider
+            Concentration parameter of the Dirichlet distribution.
+        Local_Nodes : slider
+            Number of local nodes (clients) used in the federated learning paradigm.
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the plot as output.
         """
         labels_encoded = self.labels
 
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
@@ -245,41 +215,35 @@
 
         return ()
 
     def show_scatter_distr_dirichlet(self, **slider_kwargs):
         """
         Show an interactive scatter plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            **slider_kwargs: dict
-                Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
-
-            See Also
-            --------
-
-            References
-            ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
-
-            Examples
-            --------
-            >>> from fedartml import InteractivePlots
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_plot = InteractivePlots(labels = train_y)
-            >>> my_plot.show_scatter_distr_dirichlet()
+        Parameters
+        ----------
+        **slider_kwargs: dict
+            Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
+
+        References
+        ----------
+        .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
+               https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+
+        Examples
+        --------
+        >>> from fedartml import InteractivePlots
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_plot = InteractivePlots(labels = train_y)
+        >>> my_plot.show_scatter_distr_dirichlet()
         """
         interact(self.scatter_distr_dirichlet,
                  Alpha=FloatLogSlider(**slider_kwargs.get('alpha_slider_kwargs',
                                                           {'min': -2, 'max': 3, 'value': 1000, 'readout_format': '.4'}),
                                       layout=Layout(
                                           **slider_kwargs.get('alpha_slider_lout_kwargs', {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
@@ -288,36 +252,24 @@
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def bar_divided_distr_dirichlet(self, Alpha, Local_Nodes):
         """
         Create an interactive bar plot (with sliders) divided per each local node (client).
 
-            Parameters
-            ----------
-            Alpha : slider
-                Concentration parameter of the Dirichlet distribution.
-            Local_Nodes : slider
-                Number of local nodes (clients) used in the federated learning paradigm.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the plot as output.
-
-            See Also
-            --------
-
-            References
-            ----------
-
-            Examples
-            --------
+        Parameters
+        ----------
+        Alpha : slider
+            Concentration parameter of the Dirichlet distribution.
+        Local_Nodes : slider
+            Number of local nodes (clients) used in the federated learning paradigm.
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the plot as output.
         """
         labels_encoded = self.labels
 
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
@@ -387,41 +339,35 @@
 
         return ()
 
     def show_bar_divided_distr_dirichlet(self, **slider_kwargs):
         """
         Show an interactive bar plot (with sliders) divided per each local node (client).
 
-            Parameters
-            ----------
-            **slider_kwargs: dict
-                Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
-
-            See Also
-            --------
-
-            References
-            ----------
-            .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
-
-            Examples
-            --------
-            >>> from fedartml import InteractivePlots
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_plot = InteractivePlots(labels = train_y)
-            >>> my_plot.show_bar_divided_distr_dirichlet()
+        Parameters
+        ----------
+        **slider_kwargs: dict
+            Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the sliders for Alpha and number of local nodes (clients).
+
+        References
+        ----------
+        .. [1] Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
+               https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+
+        Examples
+        --------
+        >>> from fedartml import InteractivePlots
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_plot = InteractivePlots(labels = train_y)
+        >>> my_plot.show_bar_divided_distr_dirichlet()
         """
         interact(self.bar_divided_distr_dirichlet,
                  Alpha=FloatLogSlider(**slider_kwargs.get('alpha_slider_kwargs',
                                                           {'min': -2, 'max': 3, 'value': 1000, 'readout_format': '.4'}),
                                       layout=Layout(
                                           **slider_kwargs.get('alpha_slider_lout_kwargs', {'width': '1000px'}))),
                  Local_Nodes=IntSlider(**slider_kwargs.get('loc_nodes_slider_kwargs', {'min': 1, 'max': 10, 'step': 1,
@@ -430,36 +376,24 @@
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def stacked_distr_percent_noniid(self, Pctg_NonIID, Local_Nodes):
         """
         Create an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            Pctg_NonIID : slider
-                Percentage (between o and 100) desired of non-IID-ness for the federated data.
-            Local_Nodes : slider
-                Number of local nodes (clients) used in the federated learning paradigm.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the plot as output.
-
-            See Also
-            --------
-
-            References
-            ----------
-
-            Examples
-            --------
+        Parameters
+        ----------
+        Pctg_NonIID : slider
+            Percentage (between o and 100) desired of non-IID-ness for the federated data.
+        Local_Nodes : slider
+            Number of local nodes (clients) used in the federated learning paradigm.
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the plot as output.
         """
         labels_encoded = self.labels
 
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
@@ -508,42 +442,36 @@
 
         return ()
 
     def show_stacked_distr_percent_noniid(self, **slider_kwargs):
         """
         Show an interactive stacked bar plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            **slider_kwargs: dict
-                Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the sliders for Pctg_noniid and number of local nodes
-            (clients).
-
-            See Also
-            --------
-
-            References
-            ----------
-            .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
-                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
-
-            Examples
-            --------
-            >>> from fedartml import InteractivePlots
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_plot = InteractivePlots(labels = train_y)
-            >>> my_plot.show_stacked_distr_percent_noniid()
+        Parameters
+        ----------
+        **slider_kwargs: dict
+            Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the sliders for Pctg_noniid and number of local nodes
+        (clients).
+
+        References
+        ----------
+        .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+               https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
+
+        Examples
+        --------
+        >>> from fedartml import InteractivePlots
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_plot = InteractivePlots(labels = train_y)
+        >>> my_plot.show_stacked_distr_percent_noniid()
         """
         interact(self.stacked_distr_percent_noniid,
                  Pctg_NonIID=FloatSlider(**slider_kwargs.get('pctg_noniid_slider_kwargs',
                                                              {'min': 0, 'max': 100, 'value': 0,
                                                               'readout_format': '.4'}),
                                          layout=Layout(
                                              **slider_kwargs.get('pctg_noniid_slider_lout_kwargs',
@@ -554,36 +482,24 @@
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def scatter_distr_percent_noniid(self, Pctg_NonIID, Local_Nodes):
         """
         Create an interactive scatter plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            Pctg_NonIID : slider
-                Percentage (between o and 100) desired of non-IID-ness for the federated data.
-            Local_Nodes : slider
-                Number of local nodes (clients) used in the federated learning paradigm.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the plot as output.
-
-            See Also
-            --------
-
-            References
-            ----------
-
-            Examples
-            --------
+        Parameters
+        ----------
+        Pctg_NonIID : slider
+            Percentage (between o and 100) desired of non-IID-ness for the federated data.
+        Local_Nodes : slider
+            Number of local nodes (clients) used in the federated learning paradigm.
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the plot as output.
         """
         labels_encoded = self.labels
 
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
@@ -637,42 +553,36 @@
 
         return ()
 
     def show_scatter_distr_percent_noniid(self, **slider_kwargs):
         """
         Show an interactive scatter plot (with sliders) per each local node (client) and label's classes.
 
-            Parameters
-            ----------
-            **slider_kwargs: dict
-                Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the sliders for Pctg_NonIID and number of local nodes
-            (clients).
-
-            See Also
-            --------
-
-            References
-            ----------
-            .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
-                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
-
-            Examples
-            --------
-            >>> from fedartml import InteractivePlots
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_plot = InteractivePlots(labels = train_y)
-            >>> my_plot.show_scatter_distr_percent_noniid()
+        Parameters
+        ----------
+        **slider_kwargs: dict
+            Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the sliders for Pctg_NonIID and number of local nodes
+        (clients).
+
+        References
+        ----------
+        .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+               https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
+
+        Examples
+        --------
+        >>> from fedartml import InteractivePlots
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_plot = InteractivePlots(labels = train_y)
+        >>> my_plot.show_scatter_distr_percent_noniid()
         """
         interact(self.scatter_distr_percent_noniid,
                  Pctg_NonIID=FloatSlider(**slider_kwargs.get('pctg_noniid_slider_kwargs',
                                                              {'min': 0, 'max': 100, 'value': 0,
                                                               'readout_format': '.4'}),
                                          layout=Layout(
                                              **slider_kwargs.get('pctg_noniid_slider_lout_kwargs',
@@ -683,36 +593,24 @@
                                            **slider_kwargs.get('loc_nodes_slider_lout_kwargs', {'width': '1000px'}))))
         return ()
 
     def bar_divided_distr_percent_noniid(self, Pctg_NonIID, Local_Nodes):
         """
         Create an interactive bar plot (with sliders) divided per each local node (client).
 
-            Parameters
-            ----------
-            Pctg_NonIID : slider
-                Percentage (between o and 100) desired of non-IID-ness for the federated data.
-            Local_Nodes : slider
-                Number of local nodes (clients) used in the federated learning paradigm.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the plot as output.
-
-            See Also
-            --------
-
-            References
-            ----------
-
-            Examples
-            --------
+        Parameters
+        ----------
+        Pctg_NonIID : slider
+            Percentage (between o and 100) desired of non-IID-ness for the federated data.
+        Local_Nodes : slider
+            Number of local nodes (clients) used in the federated learning paradigm.
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the plot as output.
         """
         labels_encoded = self.labels
 
         if isinstance(self.labels[0], str):
             le = preprocessing.LabelEncoder()
             le = le.fit(self.labels)
             labels_encoded = le.transform(self.labels)
@@ -782,42 +680,36 @@
 
         return ()
 
     def show_bar_divided_distr_percent_noniid(self, **slider_kwargs):
         """
         Show an interactive bar plot (with sliders) divided per each local node (client).
 
-            Parameters
-            ----------
-            **slider_kwargs: dict
-                Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
-
-            Raises
-            ------
-
-            Returns
-            -------
-            The return keyword is empty. The function shows the sliders for Pctg_NonIID and number of local nodes
-            (clients).
-
-            See Also
-            --------
-
-            References
-            ----------
-            .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
-                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
-
-            Examples
-            --------
-            >>> from fedartml import InteractivePlots
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_plot = InteractivePlots(labels = train_y)
-            >>> my_plot.show_bar_divided_distr_percent_noniid()
+        Parameters
+        ----------
+        **slider_kwargs: dict
+            Keyword arguments used for customizing sliders (inherited from ipywidgets.interact).
+
+        Returns
+        -------
+        The return keyword is empty. The function shows the sliders for Pctg_NonIID and number of local nodes
+        (clients).
+
+        References
+        ----------
+        .. [1] Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+               https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
+
+        Examples
+        --------
+        >>> from fedartml import InteractivePlots
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_plot = InteractivePlots(labels = train_y)
+        >>> my_plot.show_bar_divided_distr_percent_noniid()
         """
         interact(self.bar_divided_distr_percent_noniid,
                  Pctg_NonIID=FloatSlider(**slider_kwargs.get('pctg_noniid_slider_kwargs',
                                                              {'min': 0, 'max': 100, 'value': 0,
                                                               'readout_format': '.4'}),
                                          layout=Layout(
                                              **slider_kwargs.get('pctg_noniid_slider_lout_kwargs',
```

### Comparing `FedArtML-0.1.6/fedartml/fl_split_as_federated_data.py` & `FedArtML-0.1.7/fedartml/fl_split_as_federated_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,71 +8,65 @@
 class SplitAsFederatedData:
     """
     Creates federated data from the provided centralized data (features and labels) to exemplify identically and
     non-identically distributed labels and features across the local nodes (clients). It allows one to select between
     two methods of data federation (percent_noniid and dirichlet). It works only for classification problems
     (labels as classes).
 
-        Parameters
-        ----------
-        random_state : int
-            Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
-            output across multiple function calls.
-
-        References
-        ----------
-        .. [1] (dirichlet) Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
-               https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
-        .. [2] (percent_noniid) Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
-               https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
+    Parameters
+    ----------
+    random_state : int
+        Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
+        output across multiple function calls.
+
+    References
+    ----------
+    .. [1] (dirichlet) Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
+           https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+    .. [2] (percent_noniid) Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398). PMLR.
+           https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
     """
 
     def __init__(self, random_state=None):
         self.random_state = random_state
 
     def percent_noniid_method(self, labels, local_nodes, pct_noniid=0, random_state=None):
         """
         Create a federated dataset divided per each local node (client) using the Percentage of Non-IID (pctg_noniid)
         method.
 
-            Parameters
-            ----------
-            labels : array-like
-                The target values (class labels in classification).
-            local_nodes : array-like
-                Number of local nodes (clients) used in the federated learning paradigm.
-            pct_noniid : float
-                Percentage (between o and 100) desired of non-IID-ness for the federated data.
-            random_state : int
-                Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
-                output across multiple function calls.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            pctg_distr : array-like
-                Percentage (between 0 and 1) distribution of the classes for each local node (client).
-            num_distr : array-like
-                Numbers of distribution of the classes for each local node (client).
-            idx_distr : array-like
-                Indexes of examples (partition) taken for each local node (client).
-            num_per_node : array-like
-                Number of examples per each local node (client).
-
-            See Also
-            --------
-
-            References
-            ----------
-                .. [1] (percent_noniid) Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398).PMLR.
-                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
-            Examples
-            --------
+        Parameters
+        ----------
+        labels : array-like
+            The target values (class labels in classification).
+        local_nodes : array-like
+            Number of local nodes (clients) used in the federated learning paradigm.
+        pct_noniid : float
+            Percentage (between o and 100) desired of non-IID-ness for the federated data.
+        random_state : int
+            Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
+            output across multiple function calls.
+
+        Returns
+        -------
+        pctg_distr : array-like
+            Percentage (between 0 and 1) distribution of the classes for each local node (client).
+        num_distr : array-like
+            Numbers of distribution of the classes for each local node (client).
+        idx_distr : array-like
+            Indexes of examples (partition) taken for each local node (client).
+        num_per_node : array-like
+            Number of examples per each local node (client).
+
+        References
+        ----------
+            .. [1] (percent_noniid) Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398).PMLR.
+               https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
+        Examples
+        --------
         """
 
         # Get number of examples in the noniid part
         n_noniid = int(len(labels) * (pct_noniid / 100))
 
         # sorted_labels = sorted(labels)
         sorted_labels = labels
@@ -133,50 +127,42 @@
 
         return pctg_distr, num_distr, idx_distr, num_per_node
 
     def dirichlet_method(self, labels, local_nodes, alpha=0, random_state=None):
         """
         Create a federated dataset divided per each local node (client) using the Dirichlet (dirichlet) method.
 
-            Parameters
-            ----------
-            labels : array-like
-                The target values (class labels in classification).
-            local_nodes : array-like
-                Number of local nodes (clients) used in the federated learning paradigm.
-            alpha : float
-                Concentration parameter of the Dirichlet distribution defining the desired degree of non-IID-ness for
-                the federated data.
-            random_state : int
-                Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
-                output across multiple function calls.
-
-            Raises
-            ------
-
-            Returns
-            -------
-            pctg_distr : array-like
-                Percentage (between 0 and 1) distribution of the classes for each local node (client).
-            num_distr : array-like
-                Numbers of distribution of the classes for each local node (client).
-            idx_distr : array-like
-                Indexes of examples (partition) taken for each local node (client).
-            num_per_node : array-like
-                Number of examples per each local node (client).
-
-            See Also
-            --------
-
-            References
-            ----------
-                .. [1] (dirichlet) Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
-                    https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
-            Examples
-            --------
+        Parameters
+        ----------
+        labels : array-like
+            The target values (class labels in classification).
+        local_nodes : array-like
+            Number of local nodes (clients) used in the federated learning paradigm.
+        alpha : float
+            Concentration parameter of the Dirichlet distribution defining the desired degree of non-IID-ness for
+            the federated data.
+        random_state : int
+            Controls the shuffling applied to the generation of pseudorandom numbers. Pass an int for reproducible
+            output across multiple function calls.
+
+        Returns
+        -------
+        pctg_distr : array-like
+            Percentage (between 0 and 1) distribution of the classes for each local node (client).
+        num_distr : array-like
+            Numbers of distribution of the classes for each local node (client).
+        idx_distr : array-like
+            Indexes of examples (partition) taken for each local node (client).
+        num_per_node : array-like
+            Number of examples per each local node (client).
+
+        References
+        ----------
+            .. [1] (dirichlet) Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning
+                https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
         """
         labels = np.array(labels)
 
         min_size = 0
         num_classes = len(np.unique(labels))
         N = labels.shape[0]
         random_state_loop = random_state
@@ -225,76 +211,70 @@
 
     def create_clients(self, image_list, label_list, num_clients=5, prefix_cli='client', method="percent_noniid",
                        alpha=1000, percent_noniid=0):
         """
         Create a federated dataset divided per each local node (client) using the desired method (percent_noniid or
         dirichlet). It works only for classification problems (labels as classes).
 
-            Parameters
-            ----------
-            image_list : array-like
-                List of numpy arrays (or pandas dataframe) with images (i.e. features) from the centralized data.
-            label_list : array-like
-                The target values (class labels in classification) from the centralized data.
-            num_clients : array-like
-                Number of local nodes (clients) used in the federated learning paradigm.
-            prefix_cli : array-like
-                The clients' name prefix, e.g., client_1, client_2, etc.
-            method : array-like
-                Method to create the federated data. Possible options: "percent_noniid"(default) or "dirichlet"
-            alpha : array-like
-                Concentration parameter of the Dirichlet distribution defining the desired degree of non-IID-ness for
-                the federated data.
-            percent_noniid : array-like
-                Percentage (between o and 100) desired of non-IID-ness for the federated data.
-            Raises
-            ------
-
-            Returns
-            -------
-
-            fed_data : dict
-                Contains features (images) and labels for each local node (client) after federating the data. Includes "with_class_completion" and "without_class_completion" cases.
-            ids_list_fed_data : array-like
-                Indexes of examples (partition) taken for each local node (client).
-            num_missing_classes : array-like
-                Number of missing classes per each local node when creating the federated dataset
-            distances : array-like
-                Distances calculated while measuring heterogeneity (non-IID-ness) of the label's distribution among clients. Includes "with_class_completion" and "without_class_completion" cases.
-
-            Note: When creating federated data and setting heterogeneous distributions (i.e. high values of percent_noniid or small values of alpha), it is more likely the clients hold examples from only one class.
-            Then, two cases are returned as output for fed_data and distances:
-                - "with_class_completion": In this case, the clients are completed with one (random) example of each missing class for each client to have all the label's classes.
-                - "without_class_completion": In this case, the clients are NOT completed with one (random) example of each missing class. Consequently, summing the number of examples of each client results in the same number of total examples (number of rows in image_list).
-
-            See Also
-            --------
-
-            References
-            ----------
-                .. [1] (dirichlet) Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning0
-                   https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
-                .. [2] (percent_noniid) Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398).PMLR.
-                   https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
-            Examples
-            --------
-            >>> from fedartml import SplitAsFederatedData
-            >>> from keras.datasets import mnist
-            >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
-            >>> my_federater = SplitAsFederatedData(random_state=0)
-            >>>
-            >>> # Using percent_noniid method
-            >>> clients_glob, list_ids_sampled, miss_class_per_node, distances =
-            >>>     my_federater.create_clients(image_list=train_X, label_list=train_y, num_clients=4,
-            >>>     prefix_cli='Local_node',method="percent_noniid", percent_noniid=0)
-            >>>
-            >>> # Using dirichlet method
-            >>> clients_glob, list_ids_sampled, miss_class_per_node, distances =
-            >>>     my_federater.create_clients(image_list=train_X, label_list=train_y, num_clients=4,
-            >>>     prefix_cli='Local_node',method="dirichlet", alpha=1000)
+        Parameters
+        ----------
+        image_list : array-like
+            List of numpy arrays (or pandas dataframe) with images (i.e. features) from the centralized data.
+        label_list : array-like
+            The target values (class labels in classification) from the centralized data.
+        num_clients : array-like
+            Number of local nodes (clients) used in the federated learning paradigm.
+        prefix_cli : array-like
+            The clients' name prefix, e.g., client_1, client_2, etc.
+        method : array-like
+            Method to create the federated data. Possible options: "percent_noniid"(default) or "dirichlet"
+        alpha : array-like
+            Concentration parameter of the Dirichlet distribution defining the desired degree of non-IID-ness for
+            the federated data.
+        percent_noniid : array-like
+            Percentage (between o and 100) desired of non-IID-ness for the federated data.
+
+        Returns
+        -------
+        fed_data : dict
+            Contains features (images) and labels for each local node (client) after federating the data. Includes "with_class_completion" and "without_class_completion" cases.
+        ids_list_fed_data : array-like
+            Indexes of examples (partition) taken for each local node (client).
+        num_missing_classes : array-like
+            Number of missing classes per each local node when creating the federated dataset
+        distances : array-like
+            Distances calculated while measuring heterogeneity (non-IID-ness) of the label's distribution among clients. Includes "with_class_completion" and "without_class_completion" cases.
+
+        Note: When creating federated data and setting heterogeneous distributions (i.e. high values of percent_noniid or small values of alpha), it is more likely the clients hold examples from only one class.
+        Then, two cases are returned as output for fed_data and distances:
+            - "with_class_completion": In this case, the clients are completed with one (random) example of each missing class for each client to have all the label's classes.
+            - "without_class_completion": In this case, the clients are NOT completed with one (random) example of each missing class. Consequently, summing the number of examples of each client results in the same number of total examples (number of rows in image_list).
+
+        References
+        ----------
+            .. [1] (dirichlet) Tao Lin∗, Lingjing Kong∗, Sebastian U. Stich, Martin Jaggi. (2020). Ensemble Distillation for Robust Model Fusion in Federated Learning0
+               https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf
+            .. [2] (percent_noniid) Hsieh, K., Phanishayee, A., Mutlu, O., & Gibbons, P. (2020, November). The non-iid data quagmire of decentralized machine learning. In International Conference on Machine Learning (pp. 4387-4398).PMLR.
+               https://proceedings.mlr.press/v119/hsieh20a/hsieh20a.pdf
+        Examples
+        --------
+        >>> from fedartml import SplitAsFederatedData
+        >>> from keras.datasets import mnist
+        >>> (train_X, train_y), (test_X, test_y) = mnist.load_data()
+        >>> my_federater = SplitAsFederatedData(random_state=0)
+        >>>
+        >>> # Using percent_noniid method
+        >>> clients_glob, list_ids_sampled, miss_class_per_node, distances =
+        >>>     my_federater.create_clients(image_list=train_X, label_list=train_y, num_clients=4,
+        >>>     prefix_cli='Local_node',method="percent_noniid", percent_noniid=0)
+        >>>
+        >>> # Using dirichlet method
+        >>> clients_glob, list_ids_sampled, miss_class_per_node, distances =
+        >>>     my_federater.create_clients(image_list=train_X, label_list=train_y, num_clients=4,
+        >>>     prefix_cli='Local_node',method="dirichlet", alpha=1000)
         """
         # create a list of client names
         client_names = ['{}_{}'.format(prefix_cli, i + 1) for i in range(num_clients)]
 
         # Zip the data as list
         data = list(zip(image_list, label_list))
```

### Comparing `FedArtML-0.1.6/fedartml/function_base.py` & `FedArtML-0.1.7/fedartml/function_base.py`

 * *Files identical despite different names*

### Comparing `FedArtML-0.1.6/setup.py` & `FedArtML-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="FedArtML",
-    version="0.1.6",
+    version="0.1.7",
     description="Federated learning for Artificial Intelligence and Machine Learning library ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Daniel Mauricio Jimenez Gutierrez, Aris Anagnostopoulos, Ioannis Chatzigiannakis, Andrea Vitaletti",
     author_email="jimenezgutierrez@diag.uniroma1.it",
     license="MIT",
```

