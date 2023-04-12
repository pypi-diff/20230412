# Comparing `tmp/AutoCarver-3.1.0.tar.gz` & `tmp/AutoCarver-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-3.1.0.tar", last modified: Wed Feb  8 09:47:40 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.0.0.tar", last modified: Wed Apr 12 09:41:05 2023, max compression
```

## Comparing `AutoCarver-3.1.0.tar` & `AutoCarver-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/
-drwxrwxrwx   0        0        0        0 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/AutoCarver/
--rw-rw-rw-   0        0        0    20532 2023-01-30 08:32:41.000000 AutoCarver-3.1.0/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0    36939 2023-02-08 09:45:44.000000 AutoCarver-3.1.0/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    14207 2023-01-28 13:57:43.000000 AutoCarver-3.1.0/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-09 19:45:37.000000 AutoCarver-3.1.0/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7523 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7523 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6003 2023-01-24 08:07:41.000000 AutoCarver-3.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-02-08 09:47:40.000000 AutoCarver-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-02-08 09:46:36.000000 AutoCarver-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver/
+-rw-rw-rw-   0        0        0    22755 2023-04-12 09:39:04.000000 AutoCarver-4.0.0/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0    50557 2023-04-11 15:29:18.000000 AutoCarver-4.0.0/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    14207 2023-01-28 13:57:43.000000 AutoCarver-4.0.0/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-09 19:45:37.000000 AutoCarver-4.0.0/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     7905 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7905 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6003 2023-01-24 08:07:41.000000 AutoCarver-4.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-12 09:39:21.000000 AutoCarver-4.0.0/setup.py
```

### Comparing `AutoCarver-3.1.0/AutoCarver/AutoCarver.py` & `AutoCarver-4.0.0/AutoCarver/AutoCarver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from .Discretizers import GroupedList, GroupedListDiscretizer, is_equal
 from IPython.display import display_html
 from matplotlib.pyplot import subplots, show
 from matplotlib.ticker import PercentFormatter
 from numpy import sort, nan, inf, float32, where, isin, argsort, array, append, quantile, linspace, argmin, sqrt, random
 from pandas import DataFrame, Series, isna, qcut, notna, unique, concat, crosstab
+from pandas.api.types import is_string_dtype
 from scipy.stats import chi2_contingency
 from seaborn import color_palette, despine
 from tqdm.notebook import tqdm
+from typing import Any, Dict, List
 
 
 class AutoCarver(GroupedListDiscretizer):
     """ Automatic carving of continuous, categorical and categorical ordinal features 
     that maximizes association with a binary target.
 
     Modalities/values of features are carved/regrouped according to a computed specific
@@ -88,263 +90,318 @@
     pipe += [('AutoCarver', auto_carver)]
     pipe = Pipeline(pipe)
 
     # applying pipe to a validation set or in production
     X_val = pipe.transform(X_val)
 
     """
-    
-    def __init__(self, values_orders: dict={}, *, sort_by: str='tschuprowt',
-                 copy: bool=False, max_n_mod: int=5, keep_nans: bool=False,
-                 verbose: bool=True):
+   
+    def __init__(self, values_orders: Dict[str, Any]={}, *, sort_by: str='tschuprowt',
+                 copy: bool=False, max_n_mod: int=5, dropna: bool=True,
+                 verbose: bool=True) -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.target = None  # le nom de la target est récupéré lors du fit
-        self.non_viable_features = []  # liste des features pas stable entre TRAIN et TEST
-        self.max_n_mod = max_n_mod  # nombre maximal de modalités
-        self.keep_nans = keep_nans  # whether or not to group NaNs with other modalities
-        self.sort_by = sort_by  # association measure used find the best groups
+        self.non_viable_features: List[str] = []  # list of features non viable features
+        self.max_n_mod = max_n_mod  # maximum number of modality per feature
+        self.dropna = dropna  # whether or not to group NaNs with other modalities
+        
+        # association measure used to find the best groups
+        implemented = ['tschuprowt', 'cramerv']
+        assert sort_by in implemented, f"Measure {sort_by} is not yet implemented. Choose from: {', '.join(implemented)}."
+        self.sort_by = sort_by
+
         self.copy = copy
         self.verbose = verbose
-
-    def fit(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None):
- 
-        # copying dataframes
+    
+    def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> tuple:
+        """ Checks validity of provided data"""
+        
+        # preparing train sample
+        # checking for binary target
+        y_values = unique(y)
+        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        
+        # checking for quantitative columns
+        is_object = X[self.features].dtypes.apply(is_string_dtype)
+        assert all(is_object), f"Non-string features in X: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
+        
+        # Copying DataFrame if requested
         Xc = X
-        Xtestc = X_test if X_test is not None else DataFrame(columns=X.columns)
         if self.copy:
             Xc = X.copy()
-            Xtestc = X_test.copy() if X_test is not None else DataFrame(columns=X.columns)
-
-        # récupération du nom de la target
-        self.target = y.name
+        
+        # preparing test sample
+        # checking for binary target
+        if y_test is not None:
+            assert X_test is not None, "y_test was provided but X_test is missing"
+            y_values = unique(y_test)
+            assert (0 in y_values) & (1 in y_values), "y_test must be a binary Series (int or float, not object)"
+            assert len(y_values) == 2, "y_test must be a binary Series (int or float, not object)"
+        
+        # Copying DataFrame if requested
+        Xtestc = X_test
+        if X_test is not None:
+            assert y_test is not None, "X_test was provided but y_test is missing"
+            if self.copy:
+                Xtestc = X_test.copy()
+        
+            # checking for quantitative columns
+            is_object = X_test[self.features].dtypes.apply(is_string_dtype)
+            assert all(is_object), f"Non-string features in X_test: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
+            
+        return Xc, y, Xtestc, y_test
+    
+    def fit(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> None:
 
-        # découpage automatique de chacune des variables
+        # preparing datasets and checking for wrong values
+        Xc, y, Xtestc, y_test = self.prepare_data(X, y, X_test, y_test)
+        
+        # automatic carving of each feature
         for n, feature in tqdm(enumerate(self.features), total=len(self.features), disable=self.verbose):
 
             # printing the group statistics and determining default ordering
-            if self.verbose: print(f"\n---\n[AutoCarver] Fitting {feature} ({n+1}/{len(self.features)})")
+            if self.verbose:
+                print(f"\n---\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})")
 
             # getting best combination
-            best_groups = self.get_best_combination(feature, X, y, X_test, y_test)
+            best_groups = self.get_best_combination(feature, Xc, y, Xtestc, y_test)
 
             # feature can not be carved robustly
             if not bool(best_groups):
-                self.non_viable_features += [feature]
-                print(f"Feature {feature} is not viable")
+                self.non_viable_features += [feature]  # adding it to list of non viable features
 
         # discretizing features based on each feature's values_order
         super().__init__(self.values_orders, copy=self.copy, output=float)
         super().fit(X, y)
 
         return self
 
-    def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame, y_test: Series):
+    def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Dict[str, Any]:
 
         # getting all possible combinations for the feature without NaNS
         combinations = get_all_combinations(self.values_orders.get(feature), X[feature].nunique(dropna=True), self.max_n_mod)
         combinations = [GroupedList({group[0]: group for group in combination}) for combination in combinations]
 
         # computing crosstabs
+        # crosstab on TRAIN
         xtab = nan_crosstab(X[feature], y)
-        xtab_test = nan_crosstab(X_test[feature], y_test)
+        # crosstab on TEST
+        xtab_test = None
+        if X_test is not None:
+            xtab_test = nan_crosstab(X_test[feature], y_test)
 
         # printing the group statistics
         if self.verbose:
-            print(f'\n - Initial distribution of {feature}')
-            self.display_target_rate(feature, xtab, xtab_test)
+            self.display_xtabs(feature, 'Raw', xtab, xtab_test)
+            
+        # filtering out nans
+        notna_xtab = xtab[notna(xtab.index)]
+        notna_xtab_test = None
+        if xtab_test is not None:
+            notna_xtab_test = xtab_test[notna(xtab_test.index)]
 
         # measuring association with target for each combination and testing for stability on TEST
-        best_groups = best_combination(combinations, self.sort_by, xtab[notna(xtab.index)], 
-                                       xtab_test[notna(xtab_test.index)])
+        best_groups = best_combination(combinations, self.sort_by, notna_xtab, notna_xtab_test)
 
         # update of the values_orders grouped modalities in values_orders
         if best_groups:
-
-            self.update_values_orders(feature, best_groups['combination'])
-            # update of the crosstabs
-            xtab = xtab.groupby(list(map(best_groups['combination'].get_group, xtab.index)), dropna=False).sum()
-            xtab_test = xtab_test.groupby(list(map(best_groups['combination'].get_group, xtab_test.index)), dropna=False).sum()
+            xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
 
         # testing adding NaNs to built groups
         order = self.values_orders.get(feature)
-        if any(isna(X[feature])) & (not self.keep_nans) & (len(order) <= self.max_n_mod):
+        if any(isna(X[feature])) & self.dropna & (len(order) <= self.max_n_mod) & (len(order)>1):
 
             # getting all possible combinations for the feature with NaNS
             combinations = get_all_nan_combinations(order)
             combinations = [GroupedList({group[0]: group for group in combination}) for combination in combinations]
-
+            
             # adding nans at the end of the order
             order.append(nan)
 
             # measuring association with target for each combination and testing for stability on TEST
             best_groups = best_combination(combinations, self.sort_by, xtab, xtab_test)
 
             # update of the values_orders grouped modalities in values_orders
             if best_groups:
-
-                self.update_values_orders(feature, best_groups['combination'])
-                # update of the crosstabs
-                xtab = xtab.groupby(list(map(best_groups['combination'].get_group, xtab.index)), dropna=False).sum()
-                xtab_test = xtab_test.groupby(list(map(best_groups['combination'].get_group, xtab_test.index)), dropna=False).sum()
+                xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
 
         # printing the new group statistics
         if self.verbose and best_groups:
-
-            print(f'\n - Fitted distribution of {feature}')
-            self.display_target_rate(feature, xtab, xtab_test, plot=True)
+            self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
 
         return best_groups
 
-    def update_values_orders(self, feature: str, best_groups: GroupedList):
-        """ Updates the values_orders according to the best_groups"""
+    def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> tuple[DataFrame, DataFrame]:
+        """ Updates the values_orders and xtabs according to the best_groups"""
 
         # accessing current order for specified feature
         order = self.values_orders.get(feature)
 
         # grouping for each group of the combination
         for kept, discarded in best_groups.contained.items():
             order.group_list(discarded, kept)
 
-    def display_target_rate(self, feature: str, xtab: DataFrame, xtab_test: DataFrame, plot: bool=False):
+        # update of the TRAIN crosstab
+        best_combi = list(map(best_groups.get_group, xtab.index))
+        xtab = xtab.groupby(best_combi, dropna=False).sum()
+
+        # update of the TEST crosstab
+        if xtab_test is not None:
+            best_combi = list(map(best_groups.get_group, xtab_test.index))
+            xtab_test = xtab_test.groupby(best_combi, dropna=False).sum()
+        
+        return xtab, xtab_test
+    
+    def display_xtabs(self, feature: str, caption: str, xtab: DataFrame, xtab_test: DataFrame=None) -> None:
         """ Pretty display of frequency and target rate per modality on the same line. """
-
+        
+        # known_order per feature
         known_order = self.values_orders.get(feature)
-        stat_cols = ['target_rate', 'frequency']
-
+        
         # target rate and frequency on TRAIN
-        train_stats = DataFrame({
-            'target_rate': xtab[1].divide(xtab[0].add(xtab[1])),  # target rate of each modality
-            'frequency': xtab[1].add(xtab[0]) / xtab.sum().sum()  # frequency of each modality
-        })
+        train_stats = stats_xtab(xtab, known_order)
     
         # target rate and frequency on TEST
-        test_stats = DataFrame({
-            'target_rate': xtab_test[1].divide(xtab_test[0].add(xtab_test[1])),  # target rate of each modality
-            'frequency': xtab_test[1].add(xtab_test[0]) / xtab_test.sum().sum()  # frequency of each modality
-        })
-
-        # default ordering based on observed target rate (on TRAIN)
-        train_order = list(train_stats.sort_values('target_rate').index)
-        test_order = list(test_stats.sort_values('target_rate').index)
-
-        # keeping numpy.nan at the end of the order (default ordering)
-        if any(isna(xtab.index)):
-            train_order = [c for c in train_order if notna(c)]
-            train_order += [nan]
-            test_order = [c for c in test_order if notna(c)]
-            test_order += [nan]
-
-        # ordering by target rate
-        train_stats = train_stats.reindex(train_order)
-        test_stats = test_stats.reindex(test_order)
-
-        # ordering statistics if an order already exists
-        if known_order is not None:
-
-            # known modalities
-            new_train_order = known_order[:]
-
-            # adding unexpected modalities (only present in train_order)
-            new_train_order += [elt for elt in train_order if not any(is_equal(elt, t) for t in new_train_order)]
-
-            # ordering TRAIN
-            train_stats = train_stats.reindex(new_train_order)
-
-            # adding start and end modalities
-            renamed_train_order = [f'{known_order.get(c)[-1]} to {known_order.get(c)[0]}' if c in known_order and len(known_order.get(c)) > 1 else c for c in new_train_order]
-            train_stats.index = renamed_train_order
-
-            # ordering the TEST statistics based on known order
-            new_test_order = new_train_order[:]
+        if xtab_test is not None:
+            test_stats = stats_xtab(xtab_test, train_stats.index, train_stats.labels)
+            test_stats = test_stats.set_index('labels')  # setting labels as indices
+        
+        # setting TRAIN labels as indices
+        train_stats = train_stats.set_index('labels')
 
-            # adding unexpected modalities (only present in test_order)
-            new_test_order += [elt for elt in test_order if not any(is_equal(elt, t) for t in new_test_order)]
+        # Displaying TRAIN modality level stats
+        train_style = train_stats.style.background_gradient(cmap='coolwarm')  # color scaling
+        train_style = train_style.set_table_attributes("style='display:inline'")  # printing in notebook
+        train_style = train_style.set_caption(f'{caption} distribution on X:')  # title
+        html = train_style._repr_html_()
+        
+        # adding TEST modality level stats
+        if xtab_test is not None:
+            test_style = test_stats.style.background_gradient(cmap='coolwarm')  # color scaling
+            test_style = test_style.set_table_attributes("style='display:inline'")  # printing in notebook
+            test_style = test_style.set_caption(f'{caption} distribution on X_test:')  # title
+            html += ' ' + test_style._repr_html_()
+
+        # displaying html of colored DataFrame
+        display_html(html, raw=True)
+
+def stats_xtab(xtab: DataFrame, known_order: List[Any]=None, known_labels: List[Any]=None) -> DataFrame:
+    """ Computes column (target) rate per row (modality) and row frequency"""
+    
+    # target rate and frequency statistics per modality
+    stats = DataFrame({
+        # target rate per modality
+        'target_rate': xtab[1].divide(xtab[0].add(xtab[1])),
+        # frequency per modality
+        'frequency': xtab[1].add(xtab[0]) / xtab.sum().sum()
+    })
+    
+    # sorting statistics
+    # case 0: default ordering based on observed target rate
+    if known_order is None:
+        order = list(stats.sort_values('target_rate', ascending=True).index)
+    
+    # case 1: a known_order was provided
+    else:
+        order = known_order[:]
+      
+    # modalities' labels
+    # case 0: default labels
+    if known_labels is None:
+        
+        # accessing string representation of the GroupedList
+        if isinstance(known_order, GroupedList):
+            labels = known_order.get_repr()
 
-            # ordering TEST
-            test_stats = test_stats.reindex(new_test_order)
+        # labels are the default order
+        else:
+            labels = order[:]
+            
+    # case 1: known_labels were provided
+    else:
+        labels = known_labels[:]
+            
+            
+    # keeping values missing from the order at the end
+    unknown_modality = [mod for mod in xtab.index if mod not in order]
+    for mod in unknown_modality:
+        order = [c for c in order if not is_equal(c, mod)] + [mod]
+        labels = [c for c in labels if not is_equal(c, mod)] + [mod]
+    
+    # sorting statistics
+    stats = stats.reindex(order, fill_value=0)
+    stats['labels'] = labels
+    
+    return stats
 
-            # adding start and end modalities
-            renamed_test_order = [f'{known_order.get(c)[-1]} to {known_order.get(c)[0]}' if c in known_order and len(known_order.get(c)) > 1 else c for c in new_test_order]
-            test_stats.index = renamed_test_order
+def apply_combination(xtab: DataFrame, combination: GroupedList) -> Dict[str, Any]:
+    """ applies a modality combination to a crosstab """
 
-        # plotting the train stats
-        if plot:
-            fig, ax = plot_stats(train_stats)
-            show()
+    # initiating association dict
+    association = {'combination': combination}
 
-        # displaying the train and test stats
-        else:
+    # grouping modalities in the initial crosstab
+    groups = list(map(combination.get_group, xtab.index))
+    combi_xtab = xtab.groupby(groups, dropna=False).sum()
+    association.update({'combi_xtab': combi_xtab})
 
-            # Displaying feature level stats
-            styler = concat([train_stats, test_stats], ignore_index=True).style.background_gradient(cmap='coolwarm')  # unifying colors for both stats
-            train_style = train_stats.style.use(styler.export()).set_table_attributes("style='display:inline'").set_caption('Train:')
-            test_style = test_stats.style.use(styler.export()).set_table_attributes("style='display:inline'").set_caption('Test:')
-            display_html(train_style._repr_html_() + ' ' + test_style._repr_html_(), raw=True)
+    # measuring association with the target
+    association.update(association_xtab(combi_xtab))
 
+    return association
 
-def best_combination(combinations: list, sort_by: str, xtab: DataFrame, xtab_test: DataFrame):
+def best_combination(combinations: List[GroupedList], sort_by: str, xtab: DataFrame, xtab_test: DataFrame=None):
     """ Finds the best combination of groups of feature's values:
      - Most associated combination on train sample 
      - Stable target rate of combination on test sample.
     """
 
-    # initiating list of associations between cut feature and target 
-    associations = []
-
-    # iterating over each combination
-    for combination in combinations:
-        
-        # converting combination to a grouped list
-        association = {'combination': combination}
-
-        # grouping modalities in the initial crosstab
-        groups = list(map(combination.get_group, xtab.index))
-        combi_xtab = xtab.groupby(groups, dropna=False).sum()
-        association.update({'combi_xtab': combi_xtab})
-
-        # measuring association with the target
-        association.update(association_xtab(combi_xtab))
-        
-        # storing results
-        associations += [association]
+    # computing association measure per combination 
+    associations = [apply_combination(xtab, combi) for combi in combinations]
 
     # sort according to association measure
-    if any(combinations):
+    if len(combinations) > 0:
         associations = DataFrame(associations)
         associations.sort_values(sort_by, inplace=True, ascending=False)
         associations = associations.to_dict(orient='records')
 
     # testing associations
-    for association in associations:
-        
-        # needed parameters
-        combination, combi_xtab = association['combination'], association['combi_xtab']
+    # case 0: no test set was provided
+    if xtab_test is None and len(associations) > 0:
+        return associations[0]
+    
+    # case 1: testing viability on provided TEST sample
+    else:
+        for association in associations:
+            
+            # needed parameters
+            combination, combi_xtab = association['combination'], association['combi_xtab']
 
-        # grouping modalities in the initial crosstab
-        combi_xtab_test = xtab_test.groupby(list(map(combination.get_group, xtab_test.index)), dropna=False).sum()
+            # grouping modalities in the initial crosstab
+            combi_xtab_test = xtab_test.groupby(list(map(combination.get_group, xtab_test.index)), dropna=False).sum()
 
-        # checking that all non-nan groups are in TRAIN and TEST
-        unq_x =  [v for v in unique(combi_xtab.index) if v != notna(v)]
-        unq_xtest = [v for v in unique(combi_xtab_test.index) if v != notna(v)]
-        viability = all([e in unq_x for e in unq_xtest])
-        viability = viability and all([e in unq_xtest for e in unq_x])
+            # checking that all non-nan groups are in TRAIN and TEST
+            unq_x =  [v for v in unique(combi_xtab.index) if v != notna(v)]
+            unq_xtest = [v for v in unique(combi_xtab_test.index) if v != notna(v)]
+            viability = all([e in unq_x for e in unq_xtest])
+            viability = viability and all([e in unq_xtest for e in unq_x])
 
-        # same target rate order in TRAIN and TEST
-        train_target_rate = combi_xtab[1].divide(combi_xtab[0]).sort_values()
-        test_target_rate = combi_xtab_test[1].divide(combi_xtab_test[0]).sort_values()
-        viability = viability and all(train_target_rate.index == test_target_rate.index)
+            # same target rate order in TRAIN and TEST
+            train_target_rate = combi_xtab[1].divide(combi_xtab[0]).sort_values()
+            test_target_rate = combi_xtab_test[1].divide(combi_xtab_test[0]).sort_values()
+            viability = viability and all(train_target_rate.index == test_target_rate.index)
 
-        # checking that some combinations were provided
-        if viability:
+            # checking that some combinations were provided
+            if viability:
 
-        	association.update({'combi_xtab_test': combi_xtab_test})
+                association.update({'combi_xtab_test': combi_xtab_test})
 
-        	return association
+                return association
 
 
 def get_all_combinations(values: list, q: int, max_n_mod: int=None):
 
     # max number of classes
     if max_n_mod is None:
     	max_n_mod = q
@@ -354,22 +411,27 @@
     for n_class in range(2, max_n_mod + 1):
         combinations += get_combinations(n_class, q)
 
     combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]  # getting real feature values
 
     return combinations
 
-def get_all_nan_combinations(order: list):
+def get_all_nan_combinations(order: List[Any]):
     """ all possible combinations of modalities with numpy.nan"""
 
     # computing all non-NaN combinations
+    # case 0: several modalities -> several combinations
     if len(order) > 1:
         combinations = get_all_combinations(order, len(order))
-    else:
+    # case 1: unique modality -> two combinations
+    elif len(order) == 1:
         combinations = [[order]]
+    # case 2: no modality (only nan) -> no combination
+    else:
+        combinations = [[]]
 
     # iterating over each combinations of non-NaNs
     new_combinations = []
     for combi in combinations:
 
          # NaNs not attributed to a group (own modality)
         new_combinations += [combi + [[nan]]] 
@@ -485,11 +547,11 @@
         ax.text(sum(x[k: k+2]) / 2, y2[k], s[i], rotation=90, ha='center', va='bottom')
 
     ax.xaxis.set_major_formatter(PercentFormatter(xmax=1))    
     ax.yaxis.set_major_formatter(PercentFormatter(xmax=1))    
     ax.set_xlabel('Volume')
     ax.set_ylabel('Target rate')
     ax.set_xlim(0, 1)
-    ax.set_ylim(0, 1)
+    ax.set_ylim(0)
     despine()
     
     return fig, ax
```

### Comparing `AutoCarver-3.1.0/AutoCarver/Discretizers.py` & `AutoCarver-4.0.0/AutoCarver/Discretizers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from IPython.display import display_html
 from numpy import sort, nan, inf, float16, where, isin, argsort, array, select, append, quantile, linspace, argmin
 from pandas import DataFrame, Series, isna, qcut, notna, unique
+from pandas.api.types import is_numeric_dtype, is_string_dtype
 from sklearn.base import BaseEstimator, TransformerMixin
+from typing import Any, Dict, List
 from warnings import warn
 
+def nan_unique(x: Series):
+    """ Unique non-NaN values. """
+    
+    # unique values
+    uniques = unique(x)
+    
+    # filtering out nans
+    uniques = [u for u in uniques if notna(u)]
+    
+    return uniques
 
 class GroupedList(list):
     
-    def __init__(self, iterable=()):
+    def __init__(self, iterable=()) -> None:
         """ An ordered list that historizes its elements' merges."""
         
         # case 0: iterable est le dictionnaire contained
         if isinstance(iterable, dict):
             
             # récupération des valeurs de la liste (déjà ordonné)
             values = [key for key, _ in iterable.items()]
@@ -36,21 +48,21 @@
 
             # initialsiation de la liste
             super().__init__(iterable)
 
             # création des groupes
             self.contained = {v: [v] for v in iterable}
 
-    def group_list(self, to_discard: list, to_keep: str):
+    def group_list(self, to_discard: List[Any], to_keep: Any) -> None:
         """ Groups elements to_discard into values to_keep"""
 
         for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
             self.group(discarded, kept)
 
-    def group(self, discarded, kept):
+    def group(self, discarded: Any, kept: Any) -> None:
         """ Groups the discarded value with the kept value"""
 
         if not is_equal(discarded, kept):
 
             assert discarded in self, f"{discarded} not in list"
             assert kept in self, f"{kept} not in list"
 
@@ -62,25 +74,25 @@
                 discarded: []
             })
 
             self.remove(discarded)
         
         return self
         
-    def append(self, new_value):
+    def append(self, new_value: Any) -> None:
         """ Appends a new_value to the GroupedList"""
         
         self += [new_value]
         
         self.contained.update({new_value: [new_value]})
         
         return self
 
-    def sort(self):
-        """ Sorts the values of the list and dict, if any, NaNs are the last. """
+    def sort(self) -> None:
+        """ Sorts the values of the list and dict (if any, NaNs are last). """
 
         # str values
         keys_str = [key for key in self if isinstance(key, str)]
 
         # non-str values
         keys_float = [key for key in self if not isinstance(key, str)]
 
@@ -88,255 +100,537 @@
         keys = list(sort(keys_str)) + list(sort(keys_float)) 
 
         # recreating an ordered GroupedList
         self = GroupedList({key: self.get(key) for key in keys})
 
         return self
 
-    def sort_by(self, ordering):
+    def sort_by(self, ordering: List[Any]) -> None:
         """ Sorts the values of the list and dict, if any, NaNs are the last. """
 
         # recreating an ordered GroupedList
         self = GroupedList({k: self.get(k) for k in ordering})
 
         return self
 
     
-    def remove(self, value):
+    def remove(self, value: Any) -> None:
         
         super().remove(value)
         self.contained.pop(value)
     
-    def pop(self, idx):
+    def pop(self, idx: int) -> None:
         
         value = self[idx]
         self.remove(value)
     
-    def get(self, key):
+    def get(self, key: Any) -> List[Any]:
         """ returns list of values contained in key"""
 
         # default to fing an element
         found = self.contained.get(key)
 
         # copying with dictionnaries (not working with numpy.nan)
         if isna(key):
             found = [value for dict_key, value in self.contained.items() if is_equal(dict_key, key)][0]
 
         return found
 
-    def get_group(self, value):
+    def get_group(self, value: Any) -> Any:
         """ returns the group containing the specified value """
         
         found = [key for key, values in self.contained.items() if any(is_equal(value, elt) for elt in values)]
 
         if any(found):
             return found[0]
 
-    def values(self):
+    def values(self) -> List[Any]:
         """ returns all values contained in each group """
 
         known = [value for values in self.contained.values() for value in values]
 
         return known
 
-    def contains(self, value):
+    def contains(self, value: Any) -> bool:
         """ checks if a value if contained in any group """
 
         known_values = self.values()
 
         return any(is_equal(value, known) for known in known_values)
 
+    def get_repr(self, char_limit: int=10) -> List[str]:
+        """" Returns a representative list of strings of values of groups. """
 
-class Discretizer(BaseEstimator, TransformerMixin):
-    """ Automatic discretizing of continuous, categorical and categorical ordinal features.
+        # initiating list of group representation
+        repr: List[str] = []
+
+        # iterating over each group
+        for group in self:
+
+            # accessing group's values
+            values = self.get(group)
+            
+            if len(values) == 0:  # case 0: there are no value in this group
+                pass
+            
+            elif len(values) == 1:  # case 1: there is only one value in this group
+                repr += [values[0]]
+            
+            elif len(values) == 2:  # case 2: two values in this group
+                repr += [f'{values[1]}'[:char_limit]+' and '+f'{values[0]}'[:char_limit]]
+            
+            elif len(values) > 2:  # case 3: more than two values in this group
+                repr += [f'{values[-1]}'[:char_limit]+' to '+f'{values[0]}'[:char_limit]]
+                
+        return repr
+
+
+class StringConverter(BaseEstimator, TransformerMixin):
+    """ Converts specified columns a DataFrame into str
+    
+     - Keeps NaN inplace
+     - Converts floats of int to int
+
+    Parameters
+    ----------
+    features: list, default []
+        List of columns to be converted to string.
+    """
+    
+    def __init__(self, features: List[str]=[], copy: bool=False) -> None:
+    
+        self.features = features[:]
+        self.copy = copy
+        
+    def fit(self, X: DataFrame, y: Series=None):
+        
+        return self
+        
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # copying DataFrame if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # storing nans
+        nans = isna(Xc[self.features])
+
+        # storing ints
+        ints = Xc[self.features].applymap(lambda u: isinstance(u, float) and float.is_integer(u))
+        
+        # converting to string
+        Xc[self.features] = Xc[self.features].astype(str)
+        
+        # converting to int-strings
+        converted_ints = Xc[ints][self.features].applymap(lambda u: str(int(float(u))) if isinstance(u, str) else u)
+        Xc[self.features] = select([ints], [converted_ints], default=Xc[self.features])
+        
+        # converting back to nan
+        Xc[nans] = nan
+        
+        return Xc
+
+class QualitativeDiscretizer(BaseEstimator, TransformerMixin):
+    """ Automatic discretizing of categorical and categorical ordinal features.
 
     Modalities/values of features are grouped according to there respective orders:
      - [Qualitative features] order based on modality target rate.
      - [Qualitative ordinal features] user-specified order.
-     - [Quantitative features] real order of the values.
 
     Parameters
     ----------
-    quanti_features: list, default []
-        Contains quantitative (continuous) features to be discretized.
-
-    quali_features: list, default []
+    features: list
         Contains qualitative (categorical and categorical ordinal) features to be discretized.
 
     min_freq: int, default None
         [Qualitative features] Minimal frequency of a modality.
          - NaNs are considered a specific modality but will not be grouped.
          - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (specified
         in the `values_orders` dictionnary).
         Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
 
-    q: int, default None
-        [Quantitative features] Number of quantiles to initialy cut the feature.
-         - NaNs are considered a specific value but will not be grouped.
-         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
-        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
-        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
-        cut in q=5 quantiles.
-        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
-
     values_orders: dict, default {}
         [Qualitative ordinal features] dict of features values and list of orders of their values.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
     
-    def __init__(self, quanti_features: list=[], quali_features: list=[], q: int=None, min_freq: float=None, values_orders: dict={}, copy: bool=False, verbose: bool=False):
+    def __init__(self, features: List[str], min_freq: float=None, 
+                 values_orders: Dict[str, Any]={}, copy: bool=False, 
+                 verbose: bool=False, dropna: bool=False) -> None:
     
-        
-        self.features = quanti_features[:] + quali_features[:]
-        self.quanti_features = quanti_features[:]
-        self.quali_features = quali_features[:]
+        self.features = features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.ordinal_features = [f for f in values_orders if f in features]
+        self.non_ordinal_features = [f for f in features if f not in self.ordinal_features]
         self.min_freq = min_freq
-        self.q = q
-        self.pipe = []
+        self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
-
-    def fit(self, X, y):
+        self.dropna = dropna
+        
+    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """ Checking data for bucketization"""
         
-        # copie des features
+        # checking for quantitative columns
+        is_object = X[self.features].dtypes.apply(is_string_dtype)
+        assert all(is_object), f"Non-string features: {', '.join(is_object[~is_object].index)}, consider using StringConverter."
+        
+        # checking for binary target
+        y_values = unique(y)
+        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        
+        # checking that all unique values in X are in values_orders
+        uniques = X[self.features].apply(nan_unique)
+        for feature in self.ordinal_features:
+            missing = [val for val in uniques[feature] if val not in self.values_orders[feature]]
+            assert len(missing)==0, f"The ordering for {', '.join(missing)} of feature '{feature}' must be specified in values_orders (str-only)."
+        
+        # copying dataframe
         Xc = X.copy()
+        
+        return Xc
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Learning TRAIN distribution"""
+        
+        # checking data before bucketization
+        Xc = self.prepare_data(X, y)
 
         # [Qualitative ordinal features] Grouping rare values into closest common one
-        if any(self.values_orders.keys()):
-            if self.verbose: print("\n---\n[Discretizer] Fitting Qualitative Ordinal Features")
+        if len(self.ordinal_features) > 0:
 
-            discretizer = ClosestDiscretizer(self.values_orders, min_freq=self.min_freq, verbose=self.verbose)
+            # discretizing
+            ordinal_orders = {f: self.values_orders[f] for f in self.ordinal_features}
+            discretizer = ClosestDiscretizer(ordinal_orders, min_freq=self.min_freq, 
+                                             verbose=self.verbose)
             discretizer.fit(Xc, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += [('QualiClosestDiscretizer', discretizer)]  # adding discretizer to pipe
+            self.pipe += [('QualitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
 
         # [Qualitative non-ordinal features] Grouping rare values into default_value '__OTHER__'
-        non_ordinal = [f for f in self.quali_features if f not in self.values_orders.keys()]
-        if any(non_ordinal):
-            if self.verbose: print("\n---\n[Discretizer] Fitting Qualitative Non-Ordinal Features")
+        if len(self.non_ordinal_features) > 0:
 
-            discretizer = DefaultDiscretizer(non_ordinal, min_freq=self.min_freq, verbose=self.verbose)
+            # Grouping rare modalities
+            discretizer = DefaultDiscretizer(self.non_ordinal_features, min_freq=self.min_freq, 
+                                             verbose=self.verbose, dropna=self.dropna)
             discretizer.fit(Xc, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += [('DefaultDiscretizer', discretizer)]  # adding discretizer to pipe
 
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        """ Applying learned bucketization on TRAIN and/or TEST"""
+
+        # copying dataframe if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # iterating over each transformer
+        for _, step in self.pipe:
+            Xc = step.transform(Xc)
+
+        return Xc
+
+class QuantitativeDiscretizer(BaseEstimator, TransformerMixin):
+    """ Automatic discretizing of continuous features.
+
+    Modalities/values of features are grouped according to there respective orders:
+     - [Quantitative features] real order of the values.
+
+    Parameters
+    ----------
+    features: list
+        Contains quantitative (continuous) features to be discretized.
+
+    q: int, default None
+        [Quantitative features] Number of quantiles to initialy cut the feature.
+         - NaNs are considered a specific value but will not be grouped.
+         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
+        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
+        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
+        cut in q=5 quantiles.
+        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
+
+    """
+    
+    def __init__(self, features: List[str], q: int=None, copy: bool=False, 
+                 verbose: bool=False, dropna: bool=False) -> None:
+        
+        self.features = features[:]
+        self.values_orders: Dict[str, GroupedList] = {}
+        self.q = q
+        self.pipe: List[BaseEstimator] = []
+        self.copy = copy
+        self.verbose = verbose
+    
+    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """ Checking data for bucketization"""
+        
+        # checking for quantitative columns
+        is_numeric = X[self.features].dtypes.apply(is_numeric_dtype)
+        assert all(is_numeric), f"Non-numeric features: {', '.join(is_numeric[~is_numeric].index)}"
+        
+        # checking for binary target
+        y_values = unique(y)
+        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        
+        # copying dataframe
+        Xc = X.copy()
+        
+        return Xc
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Learning TRAIN distribution"""
+        
+        # checking data before bucketization
+        Xc = self.prepare_data(X, y)
+        
         # [Quantitative features] Grouping values into quantiles
-        if any(self.quanti_features):
-            if self.verbose: print("\n---\n[Discretizer] Fitting Quantitative Features")
+        discretizer = QuantileDiscretizer(self.features, q=self.q, verbose=self.verbose)
+        Xc = discretizer.fit_transform(Xc, y)
 
-            discretizer = QuantileDiscretizer(self.quanti_features, q=self.q, verbose=self.verbose)
-            Xc = discretizer.fit_transform(Xc)
+        # storing results
+        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+        self.pipe += [('QuantileDiscretizer', discretizer)]  # adding discretizer to pipe
+
+        # [Quantitative features] Grouping rare quantiles into closest common one
+        #  -> can exist because of overrepresented values (values more frequent than 1/q)
+        # searching for features with rare quantiles: computing min frequency per feature
+        frequencies = Xc[self.features].apply(lambda u: min_value_counts(u, self.values_orders[u.name]), axis=0)
+        
+        # minimal frequency of a quantile
+        q_min_freq = 1 / self.q / 2
+        
+        # identifying features that have rare modalities
+        has_rare = list(frequencies[frequencies <= q_min_freq].index)
+        
+        # Grouping rare modalities
+        if len(has_rare) > 0:
+            
+            # Grouping only features with rare modalities 
+            rare_values_orders = {feature: order for feature, order in self.values_orders.items() if feature in has_rare}
+            discretizer = ClosestDiscretizer(rare_values_orders, min_freq=q_min_freq, verbose=self.verbose)
+            discretizer.fit(Xc, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += [('QuantileDiscretizer', discretizer)]  # adding discretizer to pipe
+            self.pipe += [('QuantitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        """ Applying learned bucketization on TRAIN and/or TEST"""
+
+        # copying dataframe if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # iterating over each transformer
+        for _, step in self.pipe:
+            Xc = step.transform(Xc)
+
+        return Xc
+
+class Discretizer(BaseEstimator, TransformerMixin):
+    """ Automatic discretizing of continuous, categorical and categorical ordinal features.
+
+    Modalities/values of features are grouped according to there respective orders:
+     - [Qualitative features] order based on modality target rate.
+     - [Qualitative ordinal features] user-specified order.
+     - [Quantitative features] real order of the values.
+
+    Parameters
+    ----------
+    quanti_features: list
+        Contains quantitative (continuous) features to be discretized.
 
-            # [Quantitative features] Grouping rare quantiles into closest common one 
-            #  -> can exist because of overrepresented values (values more frequent than 1/q)
-            frequencies = Xc[self.quanti_features].apply(lambda u: u.value_counts(dropna=False, normalize=True).drop(nan, errors='ignore').reindex(self.values_orders.get(u.name)).fillna(0).values.min(), axis=0)  # computing min frequency per quantitative feature
-            q_min_freq = 1 / self.q / 2
-            has_rare = list(frequencies[frequencies <= q_min_freq].index)
-            if any(has_rare):
-                if self.verbose: print("\n---\n[Discretizer] Fitting Quantitative Features (that have rare values)")
+    quali_features: list
+        Contains qualitative (categorical and categorical ordinal) features to be discretized.
+
+    min_freq: int, default None
+        [Qualitative features] Minimal frequency of a modality.
+         - NaNs are considered a specific modality but will not be grouped.
+         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
+         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
+        (smallest frequency or closest target rate), between the superior and inferior values (specified
+        in the `values_orders` dictionnary).
+        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
 
-                rare_values_orders = {feature: order for feature, order in self.values_orders.items() if feature in has_rare}
-                discretizer = ClosestDiscretizer(rare_values_orders, min_freq=q_min_freq, verbose=self.verbose)
-                discretizer.fit(Xc, y)
+    q: int, default None
+        [Quantitative features] Number of quantiles to initialy cut the feature.
+         - NaNs are considered a specific value but will not be grouped.
+         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
+        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
+        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
+        cut in q=5 quantiles.
+        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
 
-                # storing results
-                self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-                self.pipe += [('QuantiClosestDiscretizer', discretizer)]  # adding discretizer to pipe
+    values_orders: dict, default {}
+        [Qualitative ordinal features] dict of features values and list of orders of their values.
+         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
+        (smallest frequency or closest target rate), between the superior and inferior values (described
+        by the `values_orders`).
+        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+    """
+
+    def __init__(self, quanti_features: List[str], quali_features: List[str], q: int=None, min_freq: float=None, 
+                 values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False, dropna: bool=False) -> None:
+
+        self.features = quanti_features[:] + quali_features[:]
+        self.quanti_features = quanti_features[:]
+        self.quali_features = quali_features[:]
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.min_freq = min_freq
+        self.q = q
+        self.pipe: List[BaseEstimator] = []
+        self.copy = copy
+        self.verbose = verbose
+        self.dropna = dropna
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+
+        # [Qualitative features] Grouping qualitative features
+        # verbose if requested
+        if self.verbose:
+            print("\n---\n[Discretizer] Fit Qualitative Features")
+
+        # grouping qualitative features
+        discretizer = QualitativeDiscretizer(
+            self.quali_features, min_freq=self.min_freq,
+            values_orders=self.values_orders, copy=self.copy,
+            verbose=self.verbose, dropna=self.dropna
+        )
+        discretizer.fit(X, y)
+
+        # storing results
+        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+        self.pipe += discretizer.pipe  # adding discretizer to pipe
+
+        # [Quantitative features] Grouping quantitative features
+        # verbose if requested
+        if self.verbose:
+            print("\n---\n[Discretizer] Fit Quantitative Features")
+
+        # grouping quantitative features
+        discretizer = QuantitativeDiscretizer(
+            self.quanti_features, q=self.q, copy=self.copy,
+            verbose=self.verbose, dropna=self.dropna
+        )
+        discretizer.fit(X, y)
+
+        # storing results
+        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+        self.pipe += discretizer.pipe  # adding discretizer to pipe
 
         return self
 
-    def transform(self, X, y=None):
-        if self.verbose: print("\n---\n[Discretizer] Discretizing Features")
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+
+        # verbose if requested
+        if self.verbose:
+            print("\n---\n[Discretizer] Transform Features")
         
-        # copie des features
+        # copying dataframe if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
 
         # iterating over each transformer
         for _, step in self.pipe:
             Xc = step.transform(Xc)
 
         return Xc
 
 
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     
-    def __init__(self, values_orders: dict, *, copy: bool=False, output: type= float, verbose: bool=False):
+    def __init__(self, values_orders: Dict[str, Any], *, copy: bool=False, output: type= float, verbose: bool=False) -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {feature: GroupedList(order) for feature, order in values_orders.items()}
         self.copy = copy
         self.output = output
         self.verbose = verbose
         
-    def fit(self, X, y=None):
+    def fit(self, X, y=None) -> None:
+        """ Does nothing, info is found in values_orders"""
 
         return self
     
-    def transform(self, X, y=None):
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # copying dataframes
         Xc = X
         if self.copy:
             Xc = X.copy()
 
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [GroupedListDiscretizer] Discretizing {feature} ({n+1}/{len(self.features)})")
             
+            # verbose if requested
+            if self.verbose: 
+                print(f" - [GroupedListDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+            
+            # bucketizing feature
             order = self.values_orders.get(feature)  # récupération des groupes
             to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
-            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identification des observations à regrouper
+            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identifying main bucket value
             to_keep = [n if self.output == float else group for n, group in enumerate(order)]  # récupération du groupe dans lequel regrouper
-            Xc[feature] = select(to_input, to_keep, default=Xc[feature])  # grouping modalities
+
+            # case when there are no values
+            if len(to_input)==0 & len(to_keep)==0:
+                pass
+
+            # grouping modalities
+            else:
+                Xc[feature] = select(to_input, to_keep, default=Xc[feature])
 
         # converting to float
         if self.output == float:
             Xc[self.features] = Xc[self.features].astype(float16)
 
         return Xc
 
 class ChainedDiscretizer(GroupedListDiscretizer):
     
-    def __init__(self, features: list, min_freq: float, chained_orders: list, *, copy: bool=False, verbose: bool=False):       
+    def __init__(self, features: List[str], min_freq: float, chained_orders: List[List[Any]], *, copy: bool=False, verbose: bool=False) -> None:       
         
         self.min_freq = min_freq
         self.features = features[:]
         self.chained_orders = [GroupedList(order) for order in chained_orders]
-        self.pipe = []
         self.copy = copy
         self.verbose = verbose
         
         # initiating features' values orders to all possible values
         self.known_values = list(set([value for group in self.chained_orders for value in group.values()]))
         self.values_orders = {f: GroupedList(self.known_values[:]) for f in self.features}
 
-    def fit(self, X, y=None):
+    def fit(self, X: DataFrame, y: Series=None) -> None:
         
         # copying dataframe
         Xc = X[self.features].copy()
         
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [ChainedDiscretizer] Fitting {feature} ({n+1}/{len(self.features)})")
+            if self.verbose: print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
 
             # computing frequencies of each modality
             frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
             values, frequencies = frequencies.index, frequencies.values
 
             # checking for unknown values (values to present in an order of self.chained_orders)
             missing = [value for value in values if notna(value) and (value not in self.known_values)]
@@ -364,37 +658,40 @@
         super().__init__(self.values_orders, copy=self.copy, output=str)
         super().fit(X, y)
             
         return self
 
 class QuantileDiscretizer(BaseEstimator, TransformerMixin):
     
-    def __init__(self, features: list, q: int, copy: bool=False, verbose: bool=False):
+    def __init__(self, features: List[str], q: int, copy: bool=False, verbose: bool=False) -> None:
         """ Discretizes quantitative features into groups of q quantiles"""
         
         self.features = features[:]
         self.q = q
-        self.values_orders = dict()
-        self.quantiles = None
+        self.values_orders: Dict[str, any] = {}
+        self.quantiles: Dict[str, Any] = {}
         self.copy = copy
         self.verbose = verbose
 
-    def fit(self, X, y=None):
+    def fit(self, X: DataFrame, y: Series=None) -> None:
         
         # computing quantiles for the feature
         self.quantiles = X[self.features].apply(find_quantiles, q=self.q, axis=0)
 
         # case when only one feature is discretized
         if len(self.features) == 1:
         	self.quantiles = {self.features[0]: list(self.quantiles.get(self.features[0]).values)}
 
         # building string of values to be displayed
-        values = []
+        values: List[str] = []
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [QuantileDiscretizer] Fitting {feature} ({n+1}/{len(self.features)})")
+
+            # verbose
+            if self.verbose:
+                print(f" - [QuantileDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
 
             # quantiles as strings
             feature_quantiles = self.quantiles.get(feature)
             str_values = ['<= ' + q for q in format_list(feature_quantiles)]
 
             # case when there is only one value
             if len(feature_quantiles) == 0:
@@ -409,24 +706,24 @@
         self.quantiles = {f: q + [inf] for f, q in self.quantiles.items()}
 
         # creating the values orders based on quantiles
         self.values_orders.update({feature: GroupedList(str_values) for feature, str_values in zip(self.features, values)})
 
         return self
     
-    def transform(self, X, y=None):
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
         
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
         
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [QuantileDiscretizer] Discretizing {feature} ({n+1}/{len(self.features)})")
+            if self.verbose: print(f" - [QuantileDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             nans = isna(Xc[feature])  # keeping track of nans
 
             # grouping values inside quantiles
             to_input = [Xc[feature] <= q for q in self.quantiles.get(feature)]  # values that will be imputed
             values = [[v] * len(X) for v in self.values_orders.get(feature)]  # new values to imput
             Xc[feature] = select(to_input, values, default=Xc[feature])  # grouping modalities
@@ -435,26 +732,30 @@
             if any(nans):
                 Xc.loc[nans, feature] = nan
         
         return Xc
 
 class ClosestDiscretizer(BaseEstimator, TransformerMixin):
     
-    def __init__(self, values_orders: dict, min_freq: float, *, default: str='worst', copy: bool=False, verbose: bool=False):
+    def __init__(self, values_orders: Dict[str, Any], min_freq: float, *, default: str='worst', copy: bool=False, verbose: bool=False):
         """ Discretizes ordered qualitative features into groups more frequent than min_freq"""
         
         self.features = list(values_orders.keys())
         self.min_freq = min_freq
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.default = default[:]
-        self.default_values = {}
+        self.default_values: Dict[str, Any] = {}
         self.copy = copy
         self.verbose = verbose
 
-    def fit(self, X, y):
+    def fit(self, X: DataFrame, y: Series) -> None:
+        
+        # verbose
+        if self.verbose:
+            print(f" - [ClosestDiscretizer] Fit {', '.join(self.features)}")
         
         # grouping rare modalities for each feature
         common_modalities = X[self.features].apply(
             lambda u: find_common_modalities(u, y, self.min_freq, self.values_orders.get(u.name)), 
             axis=0, result_type='expand'
         ).T.to_dict()
 
@@ -462,24 +763,24 @@
         self.values_orders = {f: common_modalities.get('order').get(f) for f in self.features}
 
         # defining the default value based on the strategy
         self.default_values = {f: common_modalities.get(self.default).get(f) for f in self.features}
 
         return self
     
-    def transform(self, X, y=None):
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
         
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
 
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [ClosestDiscretizer] Discretizing {feature} ({n+1}/{len(self.features)})")
+            if self.verbose: print(f" - [ClosestDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             # accessing feature's modalities' order
             order = self.values_orders.get(feature)
 
             # imputation des valeurs inconnues le cas échéant
             unknowns = [value for value in Xc[feature].unique() if not any(is_equal(value, known) for known in order.values())]
             unknowns = [value for value in unknowns if notna(value)]  # suppression des NaNs
@@ -491,94 +792,146 @@
             # grouping values inside groups of modalities
             to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
             to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identification des valeurs à regrouper
             Xc[feature] = select(to_input, order, default=Xc[feature])  # regroupement des valeurs
 
         return Xc
 
+def min_value_counts(x: Series, order: List[Any]) -> float:
+    """ Minimum of modalities' frequencies. """
+
+    # modality frequency
+    values = x.value_counts(dropna=False, normalize=True)
+    
+    # ignoring NaNs
+    values = values.drop(nan, errors='ignore')
+    
+    # adding missing modalities
+    values = values.reindex(order).fillna(0)
+    
+    # minimal frequency 
+    min_values = values.values.min()
+
+    return min_values
+
+def value_counts(x: Series, dropna: bool=False, normalize: bool=True) -> dict:
+    """ Counts the values of each modality of a series into a dictionnary"""
+    
+    values = x.value_counts(dropna=dropna, normalize=normalize)
+    
+    return values.to_dict()
+
+def target_rate(x: Series, y: Series, dropna: bool=True, ascending=True) -> dict:
+    """ Target y rate per modality of x into a dictionnary"""
+    
+    rates = y.groupby(x, dropna=dropna).mean().sort_values(ascending=ascending)
+    
+    return rates.to_dict()
+
+def nunique(x: Series, dropna=False) -> int:
+    """ Computes number of unique modalities"""
+    
+    uniques = unique(x)
+    n = len(uniques)
+    
+    # removing nans
+    if dropna:
+        if any(isna(uniques)):
+            n -= 1
+    
+    return n
 
 class DefaultDiscretizer(BaseEstimator, TransformerMixin):
     
-    def __init__(self, features: list, min_freq: float, *, default_value: str='__OTHER__', copy: bool=False, verbose: bool=False):
+    def __init__(
+        self, features: List[str], min_freq: float, *, 
+        default_value: str='__OTHER__', dropna: bool=False, 
+        copy: bool=False, verbose: bool=False) -> None:
         """ Groups a qualitative features' values less frequent than min_freq into a default_value"""
         
         self.features = features[:]
         self.min_freq = min_freq
-        self.values_orders = {}
+        self.values_orders: Dict[str, Any] = {}
         self.default_value = default_value[:]
         self.copy = copy
         self.verbose = verbose
+        self.dropna = dropna
 
-    def fit(self, X, y):
+    def fit(self, X: DataFrame, y: Series) -> None:
 
         # computing frequencies of each modality
-        frequencies = X[self.features].apply(
-            lambda u: u.value_counts(dropna=False, normalize=True).to_dict(), 
-        axis=0)
-        frequencies.index = self.features
-        frequencies = frequencies.to_dict()
-
-        # computing target rate per modality for ordering
-        target_rates = X[self.features].apply(
-            lambda u: y.groupby(u, dropna=True).mean().sort_values().to_dict(), 
-            axis=0
-        )
-        target_rates.index = self.features
-        target_rates = target_rates.to_dict()
+        frequencies = X[self.features].apply(value_counts, dropna=False, normalize=True, axis=0)
 
-        # attributing orders to each feature
-        self.values_orders = {feature: GroupedList([value for value, _ in target_rates.get(feature).items()]) for feature in self.features}
+        # computing ordered target rate per modality for ordering
+        target_rates = X[self.features].apply(target_rate, y=y, dropna=True, ascending=True, axis=0)
 
+        # attributing orders to each feature
+        self.values_orders = {feature: GroupedList(list(target_rates[feature])) for feature in self.features}
+        
+        #number of unique modality perf feature
+        nuniques = X[self.features].apply(nunique, dropna=self.dropna, axis=0)
+            
         # identifying modalities which are the most common
-        self.to_keep = {feature: [value for value, frequency in frequencies.get(feature).items() if (frequency >= self.min_freq) & notna(value)] + [nan] for feature in self.features}
-
+        kept_nan = [nan] * (~self.dropna)  # whether or not to keep nans whatever there frequency
+        self.to_keep = {
+            feature: kept_nan[:] + [
+                value for value, frequency in frequencies[feature].items()
+                    if ((frequency >= self.min_freq) & notna(value)) | (nuniques[feature] <= 2)
+            ] for feature in self.features
+        }
+        
         # grouping rare modalities 
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [DefaultDiscretizer] Fitting {feature} ({n+1}/{len(self.features)})")
+            if self.verbose:
+                print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
             
-            # identifying values to discard (rare modalities)
-            to_discard = [value for value in self.values_orders.get(feature) if value not in self.to_keep.get(feature)]
-            
-            # discarding rare modalities
-            if any(to_discard):
-                
-                # adding default_value to possible values
-                order = self.values_orders.get(feature)
-                order.append(self.default_value)
-                
-                # grouping rare modalities into default_value
-                order.group_list(to_discard, self.default_value)
                 
-                # computing target rate for default value and reordering values according to feature's target rate
-                default_target_rate = y.loc[X[feature].isin(order.get(self.default_value))].mean()  # computing target rate for default value
-                order_target_rate = [target_rates.get(feature).get(value) for value in order if value != self.default_value]
-                default_position = next(n for n, trate in enumerate(order_target_rate + [inf]) if trate > default_target_rate)
-                new_order = order[:-1][:default_position] + [self.default_value] + order[:-1][default_position:]  # getting rid of default value already in order
-                order = order.sort_by(new_order)
-                self.values_orders.update({feature: order})
+                # identifying values to discard (rare modalities)
+                to_discard = [value for value in self.values_orders[feature] if value not in self.to_keep[feature]]
+
+                # discarding rare modalities
+                if len(to_discard) > 0:
+
+                    # adding default_value to possible values
+                    order = self.values_orders[feature]
+                    order.append(self.default_value)
+
+                    # grouping rare modalities into default_value
+                    order.group_list(to_discard, self.default_value)
+
+                    # computing target rate for default value and reordering values according to feature's target rate
+                    default_target_rate = y.loc[X[feature].isin(order.get(self.default_value))].mean()  # computing target rate for default value
+                    order_target_rate = [target_rates.get(feature).get(value) for value in order if value != self.default_value]
+                    default_position = next(n for n, trate in enumerate(order_target_rate + [inf]) if trate > default_target_rate)
+
+                    # updating the modalities' order                
+                    new_order = order[:-1][:default_position] + [self.default_value] + order[:-1][default_position:]  # getting rid of default value already in order
+                    order = order.sort_by(new_order)
+                    self.values_orders.update({feature: order})
 
         return self
 
-    def transform(self, X, y=None):
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
 
         # grouping values inside groups of modalities
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [DefaultDiscretizer] Discretizing {feature} ({n+1}/{len(self.features)})")
+            if self.verbose: print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             # grouping modalities
-            Xc[feature] = select([~Xc[feature].isin(self.to_keep.get(feature))], [self.default_value], default=Xc[feature])
+            Xc[feature] = select([~Xc[feature].isin(self.to_keep[feature])], [self.default_value], default=Xc[feature])
 
         return Xc
 
-def find_quantiles(df_feature: Series, q: int, len_df: int=None, quantiles: list=None):
+
+def find_quantiles(df_feature: Series, q: int, len_df: int=None, quantiles: List[float]=None) -> List[float]:
     """ Découpage en quantile de la feature.
     
     Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
     Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
     Une fois il n'y a plus de valeurs qui soient sur-représentées,
     on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
     
@@ -636,27 +989,27 @@
 
             # case when there are no enough observations to compute quantiles
             else:
                 quantiles += [max(df_feature.values)]
 
             return quantiles
 
-def is_equal(a, b):
+def is_equal(a: Any, b: Any) -> bool:
     """ checks if a and b are equal (NaN insensitive)"""
     
     # default equality
     equal = a == b
     
     # Case where a and b are NaNs
     if isna(a) and isna(b):
         equal = True
     
     return equal
 
-def find_common_modalities(df_feature: Series, y: Series, min_freq: float, order: GroupedList, len_df: int=None):
+def find_common_modalities(df_feature: Series, y: Series, min_freq: float, order: GroupedList, len_df: int=None) -> Dict[str, Any]:
     """ Découpage en modalités de fréquence minimal (Cas des variables ordonnées).
     
     Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
     Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
     Une fois il n'y a plus de valeurs qui soient sur-représentées,
     on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
     
@@ -708,26 +1061,26 @@
             underrepresented = [value for value, frequency in zip(values, frequencies) if frequency < min_freq]  # valeur peu fréquentes
 
         worst, best = target_rate.idxmin(), target_rate.idxmax()
 
         # cas 2 : il n'existe pas de valeur sous-représentée
         return {'order': order, 'worst': worst, 'best': best}
 
-def find_closest_modality(value, idx, freq_target, min_freq):
-    """HELPER Finds the closesd modality in terms of frequency and target rate"""
+def find_closest_modality(value, idx: int, freq_target: Series, min_freq: float) -> int:
+    """HELPER Finds the closest modality in terms of frequency and target rate"""
 
-    # cas 1: il s'agit de la modalité la plus petite
+    # case 1: lowest modality
     if idx == 0:
         closest_modality = 1
         
-    # cas 2: il s'agit de la modalité la plus grande
+    # case 2: biggest modality
     elif idx == len(freq_target) - 1:
         closest_modality = len(freq_target) - 2
     
-    # cas 3: il s'agit d'un cas intermédiaire
+    # case 3: not the lowwest nor the biggest modality
     else:
         # previous modality's volume and target rate
         previous_value, previous_volume, previous_target = freq_target[idx - 1]
         
         # current modality's volume and target rate
         _, volume, target = freq_target[idx]
         
@@ -778,25 +1131,25 @@
     
     # récupération de la valeur associée
     closest_value = freq_target[closest_modality][0]
     
     return closest_value
 
 
-def format_list(a_list: list):
+def format_list(a_list: List[float]) -> List[str]:
     """ Formats a list of floats to a list of unique rounded strings of floats"""
 
-    # finding the closest power of thsousands for each element
-    closest_powers = [next((k for k in range(-3, 4) if abs(elt) // 1000**(k) < 10)) for elt in a_list]
+    # finding the closest power of thousands for each element
+    closest_powers = [next((k for k in range(-3, 4) if abs(elt) / 100 // 1000**(k) < 10)) for elt in a_list]
 
     # rounding elements to the closest power of thousands
     rounded_to_powers = [elt / 1000**(k) for elt, k in zip(a_list, closest_powers)]
 
     # computing optimal decimal per unique power of thousands
-    optimal_decimals = {}
+    optimal_decimals: Dict[str, int] = {}
     for power in unique(closest_powers):  # iterating over each power of thousands found
 
         # filtering on the specific power of thousands
         sub_array = array([elt for elt, p in zip(rounded_to_powers, closest_powers) if power == p])
 
         # number of distinct values
         n_uniques = sub_array.shape[0]
@@ -807,15 +1160,15 @@
 
         # storing in the dict    
         optimal_decimals.update({
             power: optimal_decimal
         })
 
     # rounding according to each optimal_decimal
-    rounded_list = []
+    rounded_list: List[float] = []
     for elt, power in zip(rounded_to_powers, closest_powers):
 
         # rounding each element
         rounded = elt  # by default None (no rounding)
         optimal_decimal = optimal_decimals.get(power)
         if optimal_decimal:  # checking that the optimal decimal exists
             rounded = round(elt, optimal_decimal)
@@ -825,10 +1178,13 @@
 
     # dict of suffixes per power of thousands
     suffixes = {
         -3: 'n', -2: 'mi', -1: 'm', 0: '', 1: 'K', 2: 'M', 3: 'B'
     }
 
     # adding the suffixes
-    formatted_list = [str(elt) + suffixes.get(power) for elt, power in zip(rounded_list, closest_powers)]
-
-    return formatted_list
+    formatted_list = [f'{elt: 3.3f}{suffixes[power]}' for elt, power in zip(rounded_list, closest_powers)]
+    
+    # keeping zeros
+    formatted_list = [rounded if raw != 0 else f'{raw: 3.3f}' for rounded, raw in zip(formatted_list, a_list)]
+    
+    return formatted_list
```

### Comparing `AutoCarver-3.1.0/AutoCarver/FeatureSelector.py` & `AutoCarver-4.0.0/AutoCarver/FeatureSelector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-3.1.0/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.0.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 3.1.0
-Summary: Automatic Carving of Features with Optimal Association
+Version: 4.0.0
+Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Description: # AutoCarver
         
@@ -145,8 +145,16 @@
         pipe = load(open('my_pipe.pkl', 'rb'))
         
         # applying pipe to a validation set or in production
         X_val = pipe.transform(X_val)
         ```
         
 Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `AutoCarver-3.1.0/PKG-INFO` & `AutoCarver-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 3.1.0
-Summary: Automatic Carving of Features with Optimal Association
+Version: 4.0.0
+Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Description: # AutoCarver
         
@@ -145,8 +145,16 @@
         pipe = load(open('my_pipe.pkl', 'rb'))
         
         # applying pipe to a validation set or in production
         X_val = pipe.transform(X_val)
         ```
         
 Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `AutoCarver-3.1.0/README.md` & `AutoCarver-4.0.0/README.md`

 * *Files identical despite different names*

