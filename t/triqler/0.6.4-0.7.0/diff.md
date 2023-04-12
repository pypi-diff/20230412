# Comparing `tmp/triqler-0.6.4-py3-none-any.whl.zip` & `tmp/triqler-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 59885 bytes, number of entries: 28
+Zip file size: 62571 bytes, number of entries: 28
 -rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 triqler/__init__.py
 -rw-r--r--  2.0 unx      140 b- defN 80-Jan-01 00:00 triqler/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 triqler/convert/__init__.py
--rw-r--r--  2.0 unx      143 b- defN 80-Jan-01 00:00 triqler/convert/__main__.py
+-rw-r--r--  2.0 unx     2041 b- defN 80-Jan-01 00:00 triqler/convert/diann.py
 -rw-r--r--  2.0 unx     6505 b- defN 80-Jan-01 00:00 triqler/convert/dinosaur.py
 -rw-r--r--  2.0 unx     6022 b- defN 80-Jan-01 00:00 triqler/convert/helpers.py
 -rw-r--r--  2.0 unx     6372 b- defN 80-Jan-01 00:00 triqler/convert/maxquant.py
 -rw-r--r--  2.0 unx     5245 b- defN 80-Jan-01 00:00 triqler/convert/normalize_intensities.py
 -rwxr-xr-x  2.0 unx     2902 b- defN 80-Jan-01 00:00 triqler/convert/percolator.py
 -rw-r--r--  2.0 unx     6447 b- defN 80-Jan-01 00:00 triqler/convert/quandenser.py
 -rw-r--r--  2.0 unx     1127 b- defN 80-Jan-01 00:00 triqler/convolution_dp.py
 -rwxr-xr-x  2.0 unx     9823 b- defN 80-Jan-01 00:00 triqler/diff_exp.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 triqler/distribution/__init__.py
--rw-r--r--  2.0 unx      145 b- defN 80-Jan-01 00:00 triqler/distribution/__main__.py
 -rw-r--r--  2.0 unx     2689 b- defN 80-Jan-01 00:00 triqler/distribution/plot_hyperparameter_fits.py
 -rw-r--r--  2.0 unx    29078 b- defN 80-Jan-01 00:00 triqler/distribution/plot_posteriors.py
--rw-r--r--  2.0 unx    11148 b- defN 80-Jan-01 00:00 triqler/hyperparameters.py
+-rw-r--r--  2.0 unx    17329 b- defN 80-Jan-01 00:00 triqler/hyperparameters.py
 -rw-r--r--  2.0 unx     1735 b- defN 80-Jan-01 00:00 triqler/multiprocessing_pool.py
 -rw-r--r--  2.0 unx    11469 b- defN 80-Jan-01 00:00 triqler/parsers.py
 -rwxr-xr-x  2.0 unx     9551 b- defN 80-Jan-01 00:00 triqler/pgm.py
 -rw-r--r--  2.0 unx    16130 b- defN 80-Jan-01 00:00 triqler/qvality.py
--rw-r--r--  2.0 unx    23385 b- defN 80-Jan-01 00:00 triqler/triqler.py
+-rw-r--r--  2.0 unx    23827 b- defN 80-Jan-01 00:00 triqler/triqler.py
 -rw-r--r--  2.0 unx     1018 b- defN 80-Jan-01 00:00 triqler/version.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 triqler-0.6.4.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 triqler-0.6.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx    10067 b- defN 16-Jan-01 00:00 triqler-0.6.4.dist-info/METADATA
-?rw-r--r--  2.0 unx     2273 b- defN 16-Jan-01 00:00 triqler-0.6.4.dist-info/RECORD
-28 files, 186211 bytes uncompressed, 56261 bytes compressed:  69.8%
+?rw-r--r--  2.0 unx      368 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 triqler-0.7.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    10942 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     2279 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/RECORD
+28 files, 195836 bytes uncompressed, 58937 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -6,15 +6,15 @@
 
 Filename: triqler/__main__.py
 Comment: 
 
 Filename: triqler/convert/__init__.py
 Comment: 
 
-Filename: triqler/convert/__main__.py
+Filename: triqler/convert/diann.py
 Comment: 
 
 Filename: triqler/convert/dinosaur.py
 Comment: 
 
 Filename: triqler/convert/helpers.py
 Comment: 
@@ -36,17 +36,14 @@
 
 Filename: triqler/diff_exp.py
 Comment: 
 
 Filename: triqler/distribution/__init__.py
 Comment: 
 
-Filename: triqler/distribution/__main__.py
-Comment: 
-
 Filename: triqler/distribution/plot_hyperparameter_fits.py
 Comment: 
 
 Filename: triqler/distribution/plot_posteriors.py
 Comment: 
 
 Filename: triqler/hyperparameters.py
@@ -66,20 +63,23 @@
 
 Filename: triqler/triqler.py
 Comment: 
 
 Filename: triqler/version.py
 Comment: 
 
-Filename: triqler-0.6.4.dist-info/LICENSE
+Filename: triqler-0.7.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: triqler-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: triqler-0.6.4.dist-info/WHEEL
+Filename: triqler-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: triqler-0.6.4.dist-info/METADATA
+Filename: triqler-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: triqler-0.6.4.dist-info/RECORD
+Filename: triqler-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## triqler/hyperparameters.py

```diff
@@ -3,63 +3,93 @@
 from __future__ import print_function
 
 import csv
 import sys
 import os
 import itertools
 
+import pandas as pd
 import numpy as np
 from scipy.stats import hypsecant, gamma, norm, binom, t, cauchy
 from scipy.optimize import curve_fit
 
 from . import parsers
 
 def fitPriors(peptQuantRows, params, printImputedVals = False, plot = False):
   params['proteinQuantCandidates'] = np.arange(-5.0, 5.0 + 1e-10, 0.01) # log10 of protein ratio  
   qc = params['proteinQuantCandidates']
   params['proteinDiffCandidates'] = np.linspace(2*qc[0], 2*qc[-1], len(qc)*2-1)
   
+    
   protQuantRows = parsers.filterAndGroupPeptides(peptQuantRows, lambda x : not x.protein[0].startswith(params['decoyPattern']))
   
   imputedVals, imputedDiffs, observedXICValues, protQuants, protDiffs, protStdevsInGroup, protGroupDiffs = list(), list(), list(), list(), list(), list(), list()
   quantRowsCollection = list()
+  if params["missingValuePrior"] == "DIA":
+      imputed_peptide_group_means = [] # Added for DIA prior
   for prot, quantRows in protQuantRows:
     quantRows, quantMatrix = parsers.getQuantMatrix(quantRows)
     
     quantMatrixNormalized = [parsers.geoNormalize(row) for row in quantMatrix]
     quantRowsCollection.append((quantRows, quantMatrix))
     geoAvgQuantRow = getProteinQuant(quantMatrixNormalized, quantRows)
     
     protQuants.extend([np.log10(x) for x in geoAvgQuantRow if not np.isnan(x)])
 
     args = parsers.getQuantGroups(geoAvgQuantRow, params["groups"], np.log10)
-    #means = list()
     for group in args:
       if np.count_nonzero(~np.isnan(group)) > 1:
         protDiffs.extend(group - np.mean(group))
         protStdevsInGroup.append(np.std(group))
-      #if np.count_nonzero(~np.isnan(group)) > 0:
-      #  means.append(np.mean(group))
-    
-    #if np.count_nonzero(~np.isnan(means)) > 1:
-    #  for mean in means:  
-    #    #protGroupDiffs.append(mean - np.mean(means))
-    #    protGroupDiffs.append(mean)
-    
+
+
     quantMatrixFiltered = np.log10(np.array([x for x, y in zip(quantMatrix, quantRows) if y.combinedPEP < 1.0]))  
+
+    # Fit prior based on means of missing value
+    if params["missingValuePrior"] == "DIA": 
+        for peptide in quantMatrixFiltered:
+            for group in params["groups"]:
+
+                n_imputed_values = len(group) - (~np.isnan(peptide[group])).sum() # number of imputed values.  
+                if n_imputed_values == 0: # If the condition has no NaN, dont add it to imputed group mean
+                    continue
+                else:
+                    
+                    for n_imputed in range(n_imputed_values): # For every imputed value add it to imputed_peptide_group_mean
+                        group_means = peptide[group][~np.isnan(peptide[group])].mean()
+                        if group_means != np.nan: # If not all samples in condition in mean, append it into imputed_peptide_group_means
+                            imputed_peptide_group_means.append(group_means)
+
+    # DIA PRIOR COMMENT 
+    # We can impute in many different ways. The current version adds one condition imputed mean for every missing replicate 
+    # e.g. if we have [3 NaN NaN] and impute the NaN to 3, we add two 3 to our imputed_peptide_group_means list.
+    #
+    # We can also modify the code so that
+    # 1) We only add one mean per condition to imputed_peptide_group_means, e.g. [3 NaN NaN] adds only 3 one time to imputed_peptide_group_means 
+    # 2) We can add a filter so that if more than 50% (or x% or x samples) are missing in our condition we do not add it to our imputed_peptide_group_means
+    
     observedXICValues.extend(quantMatrixFiltered[~np.isnan(quantMatrixFiltered)])
     
     # counts number of NaNs per run, if there is only 1 non NaN in the column, we cannot use it for estimating the imputedDiffs distribution
     numNonNaNs = np.count_nonzero(~np.isnan(quantMatrixFiltered), axis = 0)[np.newaxis,:]
     xImps = imputeValues(quantMatrixFiltered, geoAvgQuantRow, np.log10(geoAvgQuantRow))
     imputedDiffs.extend((xImps - quantMatrixFiltered)[(~np.isnan(quantMatrixFiltered)) & (np.array(numNonNaNs) > 1)])
     #imputedVals.extend(xImps[(np.isnan(quantMatrixFiltered)) & (np.array(numNonNaNs) > 1)])
   
-  fitLogitNormal(observedXICValues, params, plot)
-  
+
+  # Add parameter to params for selecting fitLogitNormal
+  if params["missingValuePrior"] == "DIA":
+      
+      imputed_peptide_group_means = np.array(imputed_peptide_group_means)
+      imputed_peptide_group_means = imputed_peptide_group_means[~np.isnan(imputed_peptide_group_means)]
+      imputedValues = imputed_peptide_group_means
+      fitLogitNormalDIA(observedXICValues, imputedValues, params, plot) # DIA fitLogitNormal - missing value prior
+  else:
+      fitLogitNormal(observedXICValues, params, plot) # old fitLogitNormal - missing value prior
+
   fitDist(protQuants, funcHypsec, "log10(protein ratio)", ["muProtein", "sigmaProtein"], params, plot)
     
   fitDist(imputedDiffs, funcHypsec, "log10(imputed xic / observed xic)", ["muFeatureDiff", "sigmaFeatureDiff"], params, plot)
   
   fitDist(protStdevsInGroup, funcGamma, "stdev log10(protein diff in group)", ["shapeInGroupStdevs", "scaleInGroupStdevs"], params, plot, x = np.arange(-0.1, 1.0, 0.005))
   
   sigmaCandidates = np.arange(0.001, 3.0, 0.001)
@@ -70,23 +100,22 @@
   params['proteinPrior'] = funcLogHypsec(params['proteinQuantCandidates'], params["muProtein"], params["sigmaProtein"])
   if "shapeInGroupStdevs" in params:
     params['inGroupDiffPrior'] = funcHypsec(params['proteinDiffCandidates'], 0, params['sigmaCandidates'][:, np.newaxis])
   else: # if we have technical replicates, we could use a delta function for the group scaling parameter to speed things up
     fitDist(protDiffs, funcHypsec, "log10(protein diff in group)", ["muInGroupDiffs", "sigmaInGroupDiffs"], params, plot)
     params['inGroupDiffPrior'] = funcHypsec(params['proteinDiffCandidates'], params['muInGroupDiffs'], params['sigmaInGroupDiffs'])
   
-  #fitDist(protGroupDiffs, funcHypsec, "log10(protein diff between groups)", ["muProteinGroupDiffs", "sigmaProteinGroupDiffs"], params, plot)
   
 def fitLogitNormal(observedValues, params, plot):
   m = np.mean(observedValues)
   s = np.std(observedValues)
   minBin, maxBin = m - 4*s, m + 4*s
-  #minBin, maxBin = -2, 6
   vals, bins = np.histogram(observedValues, bins = np.arange(minBin, maxBin, 0.1), normed = True)
   bins = bins[:-1]
+
   popt, _ = curve_fit(funcLogitNormal, bins, vals, p0 = (m, s, m - s, s))
   
   resetXICHyperparameters = False
   if popt[0] < popt[2] - 5*popt[3] or popt[0] > popt[2] + 5*popt[3]:
     print("  Warning: muDetect outside of expected region [", popt[2] - 5*popt[3] , ",", popt[2] + 5*popt[3], "]:", popt[0], ".")
     resetXICHyperparameters = True
   
@@ -94,20 +123,17 @@
     print("  Warning: sigmaDetect outside of expected region [0.1,2.0]:" , popt[1], ".")
     resetXICHyperparameters = True
   
   if resetXICHyperparameters:
     print("    Resetting mu/sigmaDetect hyperparameters to default values of muDetect = muXIC - 1.0 and sigmaDetect = 0.3")
     popt[1] = 0.3
     popt[0] = popt[2] - 1.0
-  
-  #print("  params[\"muDetectInit\"], params[\"sigmaDetectInit\"] = %f, %f" % (popt[0], popt[1]))
+    
   print("  params[\"muDetect\"], params[\"sigmaDetect\"] = %f, %f" % (popt[0], popt[1]))
   print("  params[\"muXIC\"], params[\"sigmaXIC\"] = %f, %f" % (popt[2], popt[3]))
-  #params["muDetectInit"], params["sigmaDetectInit"] = popt[0], popt[1]
-  #popt[0], popt[1] = popt[2] - popt[3]*3, popt[3]*1.5
   params["muDetect"], params["sigmaDetect"] = popt[0], popt[1]
   params["muXIC"], params["sigmaXIC"] = popt[2], popt[3]
   if plot:
     poptNormal, _ = curve_fit(funcNorm, bins, vals)
     
     import matplotlib.pyplot as plt
     plt.figure()
@@ -118,14 +144,89 @@
     plt.plot(bins, funcNorm(bins, popt[2], popt[3]), 'c', label = "normal-part fit", linewidth = 2.0)
     plt.plot(bins, funcNorm(bins, *poptNormal), 'r', label='normal fit (for comparison)', linewidth = 2.0, alpha = 0.5)
     plt.ylabel("relative frequency", fontsize = 14)
     plt.xlabel("log10(intensity)", fontsize = 14)
     plt.legend()
     plt.tight_layout()
     
+# Added for DIAPrior
+def fitLogitNormalDIA(observedValues, imputedValues, params, plot):
+  m = np.mean(observedValues)
+  s = np.std(observedValues)
+  minBin, maxBin = -1, 4 # DIA prior binning interval... reasoning is that missing values will be close to zero. Higher intensity missing values should not be regarded. We could also go with -2, 6 for example.
+  vals, bins = np.histogram(observedValues, bins = np.arange(minBin, maxBin, 0.1), normed = True)
+  bins = bins[:-1]
+  
+  DIA_bins = np.arange(minBin, maxBin, 0.1)
+  """
+  Need to do the binomial weighting to the curve fit
+    # We fit the fraction data we have to pmissings
+    # binaomial distribution wiki
+    #sigma.plot()
+    
+    # We fit the fraction data we have to pmissings
+    popt, pcov = curve_fit(pmissing, xdata, ydata, sigma=sigma)
+  """
+  
+
+  df_binned_imputed_mean_nans = pd.cut(imputedValues, DIA_bins, include_lowest=True)
+  df_binned_vals = pd.cut(observedValues, DIA_bins, include_lowest=True)
+  df_binned_missing_value_fraction = (df_binned_imputed_mean_nans.value_counts() / (df_binned_vals.value_counts()+df_binned_imputed_mean_nans.value_counts()))
+  df_binned_missing_value_fraction = pd.DataFrame(df_binned_missing_value_fraction.values, index = df_binned_missing_value_fraction.index, columns = ["fraction"])
+  df_binned_missing_value_fraction["n_count"] = (df_binned_vals.value_counts()+df_binned_imputed_mean_nans.value_counts())  
+  df_binned_missing_value_fraction.reset_index(inplace =True)
+  df_binned_missing_value_fraction.index = bins#[:-1]
+  df_binned_missing_value_fraction = df_binned_missing_value_fraction[df_binned_missing_value_fraction.n_count > 10] # I actually forgot what was the reasoning for the n_count > 10 heuristic...
+
+  xdata = df_binned_missing_value_fraction.index
+  ydata = df_binned_missing_value_fraction.fraction
+  sigma = np.sqrt(ydata * (1-ydata) / df_binned_missing_value_fraction.n_count) # Used for the binomial weighing of the curve_fit function. An uncertainty estimator, can we write this down again somewhere. I will 100  % forget the reasoning for this in the future
+  # I feel like we need to document and explain this somewhere because I have already forgot the reasoning for this. 
+
+  # This is to fit the normal logitNormal
+  popt, _ = curve_fit(funcLogitNormal, bins, vals, p0 = (m, s, m - s, s)) # replace  with code below.
+  
+  popt_DIA, pcov_DIA = curve_fit(funcOneMinusLogit, xdata, ydata, sigma=sigma) # popt_DIA, funcOneMinusLogit is the function called pmissing in dia_sum/script/clean/plot_fraction_missing_values.py. The sigma is for the binomial weighing to the curve_fit
+    
+  resetXICHyperparameters = False
+
+  if popt_DIA[1] < 0.005 or popt_DIA[1] > 10.0: #Heureistically set
+    print("  Warning: sigmaDetect outside of expected region [0.005,10.0]:" , popt_DIA[1], ".")
+    resetXICHyperparameters = True
+  
+  if popt_DIA[0] < -100 or popt_DIA[0] > 100.0: #Heureistically set
+    print("  Warning: muDetect outside of expected region [-100.0,100.0]:" , popt_DIA[0], ".")
+    resetXICHyperparameters = True
+    
+  if resetXICHyperparameters:
+    print("    Resetting mu/sigmaDetect hyperparameters to default DIA values of muDetect = muXIC - 1.0 and sigmaDetect = 0.3")
+    popt_DIA[1] = 0.3
+    popt_DIA[0] = popt[2] - 1.0
+  
+  print("  params[\"muDetect\"], params[\"sigmaDetect\"] = %f, %f" % (popt_DIA[0], popt_DIA[1]))
+  print("  params[\"muXIC\"], params[\"sigmaXIC\"] = %f, %f" % (popt[2], popt[3]))
+
+  params["muDetect"], params["sigmaDetect"] = popt_DIA[0], popt_DIA[1] #popt[0], popt[1] # estimated here
+  params["muXIC"], params["sigmaXIC"] = popt[2], popt[3] # not estimated here. We need to
+  if plot:
+    poptNormal, _ = curve_fit(funcNorm, bins, vals)
+    
+    import matplotlib.pyplot as plt
+    plt.figure()
+    plt.title('Curve fits for muDetect, sigmaDetect, muXIC and sigmaXIC', fontsize = 14)
+    plt.bar(bins, vals, width = bins[1] - bins[0], alpha = 0.5, label = 'observed distribution')
+    plt.plot(bins, funcLogitNormal(bins, *popt), 'g', label='logit-normal fit', linewidth = 2.0)
+    plt.plot(bins, 0.5 + 0.5 * np.tanh((np.array(bins) - popt[0]) / popt[1]), 'm', label = "logit-part fit", linewidth = 2.0)
+    plt.plot(bins, funcNorm(bins, popt[2], popt[3]), 'c', label = "normal-part fit", linewidth = 2.0)
+    plt.plot(bins, funcNorm(bins, *poptNormal), 'r', label='normal fit (for comparison)', linewidth = 2.0, alpha = 0.5)
+    plt.ylabel("relative frequency", fontsize = 14)
+    plt.xlabel("log10(intensity)", fontsize = 14)
+    plt.legend()
+    plt.tight_layout()    
+    
 def fitDist(ys, func, xlabel, varNames, params, plot, x = np.arange(-2,2,0.01)):
   vals, bins = np.histogram(ys, bins = x, normed = True)
   bins = bins[:-1]
   popt, _ = curve_fit(func, bins, vals)
   outputString = ", ".join(["params[\"%s\"]"]*len(popt)) + " = " + ", ".join(["%f"] * len(popt))
   for varName, val in zip(varNames, popt):
     params[varName] = val
@@ -221,7 +322,11 @@
   
 def funcGamma(x, shape, sigma):
   return gamma.pdf(x, shape, 0.0, sigma)
   
 def logit(x, muLogit, sigmaLogit):
   return 0.5 + 0.5 * np.tanh((np.array(x) - muLogit) / sigmaLogit)
 
+# Added for DIA prior from pgm.py
+def funcOneMinusLogit(x, muLogit, sigmaLogit):
+  return 1.0 - logit(x, muLogit, sigmaLogit) + np.nextafter(0, 1)
+
```

## triqler/triqler.py

```diff
@@ -15,18 +15,20 @@
 from . import qvality
 from . import hyperparameters
 from . import pgm
 from . import diff_exp
 from . import version
 
 __version__ = version.get_version_from_pyproject()
-__copyright__ = '''Copyright (c) 2018-2020 Matthew The. All rights reserved.
-Written by Matthew The (matthew.the@scilifelab.se) in the
-School of Engineering Sciences in Chemistry, Biotechnology and Health at the 
-Royal Institute of Technology in Stockholm.'''
+__copyright__ = '''Copyright (c) 2018-2023 Matthew The, Patrick Truong. All rights reserved.
+Written by:
+- Matthew The (matthew.the@scilifelab.se)
+- Patrick Truong (patrick.truong@scilifelab.se)
+in the School of Engineering Sciences in Chemistry, Biotechnology and Health
+at the Royal Institute of Technology in Stockholm.'''
 
 
 def main():
   print('Triqler version %s\n%s' % (__version__, __copyright__))
   print('Issued command:', os.path.basename(__file__) + " " + " ".join(map(str, sys.argv[1:])))
   
   args, params = parseArgs()
@@ -54,14 +56,17 @@
                           ''')
   
   apars.add_argument('--fold_change_eval', type=float, default=1.0, metavar='F',
                      help='log2 fold change evaluation threshold.')
   
   apars.add_argument('--decoy_pattern', default = "decoy_", metavar='P', 
                      help='Prefix for decoy proteins.')
+
+  apars.add_argument('--missing_value_prior', default = "default", metavar='D',
+                     help='Distribution to fit for missing value prior. Use "DIA" for using means of NaNs to fit the censored normal distribution. The "default" option fits the censored normal distribution with all observed XIC values.')
   
   apars.add_argument('--min_samples', type=int, default=2, metavar='N', 
                      help='Minimum number of samples a peptide needed to be quantified in.')
   # Peptides quantified in less than the minimum number will be discarded
   
   apars.add_argument('--num_threads', type=int, default=multiprocessing.cpu_count(), metavar='N', 
                      help='Number of threads, by default this is equal to the number of CPU cores available on the device.')
@@ -90,14 +95,15 @@
   
   params = dict()
   params['warningFilter'] = "default"
   params['foldChangeEval'] = args.fold_change_eval
   params['t-test'] = args.ttest
   params['minSamples'] = args.min_samples
   params['decoyPattern'] = args.decoy_pattern
+  params['missingValuePrior'] = args.missing_value_prior
   params['numThreads'] = args.num_threads
   params['writeSpectrumQuants'] = args.write_spectrum_quants
   params['proteinPosteriorsOutput'] = args.write_protein_posteriors
   params['groupPosteriorsOutput'] = args.write_group_posteriors
   params['foldChangePosteriorsOutput'] = args.write_fold_change_posteriors
   params['returnPosteriors'] = len(params['proteinPosteriorsOutput']) > 0 or len(params['groupPosteriorsOutput']) > 0 or len(params['foldChangePosteriorsOutput']) > 0
```

## Comparing `triqler-0.6.4.dist-info/LICENSE` & `triqler-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triqler-0.6.4.dist-info/METADATA` & `triqler-0.7.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: triqler
-Version: 0.6.4
+Version: 0.7.0
 Summary: Triqler: TRansparent Identification-Quantification-Linked Error Rates
 Home-page: https://github.com/statisticalbiotechnology/triqler
 License: Apache-2.0
 Keywords: mass spectrometry,missing values,proteomics,quantification
 Author: Matthew The
 Author-email: matthew.the@tum.de
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: threadpoolctl (>=3.1.0,<4.0.0)
 Project-URL: Repository, https://github.com/statisticalbiotechnology/triqler
 Description-Content-Type: text/x-rst
 
 Triqler: TRansparent Identification-Quantification-Linked Error Rates
 =====================================================================
@@ -37,16 +38,17 @@
 the converters to the Triqler input format are available in our 
 `wiki <https://github.com/statisticalbiotechnology/triqler/wiki>`_.
 
 
 Method description / Citation
 -----------------------------
 
-The, M. & Käll, L. (2019). Integrated identification and quantification error probabilities for shotgun proteomics. *Molecular & Cellular Proteomics, 18* (3), 561-570.
+The, M. & Käll, L. (2019). Integrated identification and quantification error probabilities for shotgun proteomics. *Molecular & Cellular Proteomics, 18* (3), 561-570. https://doi.org/10.1074/mcp.RA118.001018
 
+Truong, P., The, M., & Käll, L. (2023). Triqler for Protein Summarization of Data from Data-Independent Acquisition Mass Spectrometry. *Journal of Proteome Research, 22* (4), 1359-1366. https://doi.org/10.1021/acs.jproteome.2c00607
 
 Requirements
 ------------
 
 Python 2 or 3 installation
 
 Packages needed:
@@ -75,40 +77,47 @@
   pip install .
 
 Usage
 -----
 
 ::
 
-  usage: python -m triqler [-h] [--out_file OUT] [--fold_change_eval F]
-                   [--decoy_pattern P] [--min_samples N] [--num_threads N]
-                   [--ttest] [--write_spectrum_quants]
-                   [--write_protein_posteriors P_OUT]
-                   [--write_group_posteriors G_OUT]
-                   [--write_fold_change_posteriors F_OUT]
-                   IN_FILE
+  usage: triqler [-h] [--out_file OUT] [--fold_change_eval F]
+               [--decoy_pattern P] [--missing_value_prior D] [--min_samples N]
+               [--num_threads N] [--ttest] [--write_spectrum_quants]
+               [--write_protein_posteriors P_OUT]
+               [--write_group_posteriors G_OUT]
+               [--write_fold_change_posteriors F_OUT]
+               [--csv-field-size-limit CSV_FIELD_SIZE_LIMIT]
+               IN_FILE
 
   positional arguments:
     IN_FILE               List of PSMs with abundances (not log transformed!)
                           and search engine score. See README for a detailed
                           description of the columns.
 
   optional arguments:
     -h, --help            show this help message and exit
     --out_file OUT        Path to output file (writing in TSV format). N.B. if
                           more than 2 treatment groups are present, suffixes
                           will be added before the file extension. (default:
                           proteins.tsv)
     --fold_change_eval F  log2 fold change evaluation threshold. (default: 1.0)
     --decoy_pattern P     Prefix for decoy proteins. (default: decoy_)
+    --missing_value_prior D
+                          Distribution to fit for missing value prior. Use "DIA"
+                          for using means of NaNs to fit the censored normal
+                          distribution. The "default" option fits the censored
+                          normal distribution with all observed XIC values.
+                          (default: default)
     --min_samples N       Minimum number of samples a peptide needed to be
                           quantified in. (default: 2)
     --num_threads N       Number of threads, by default this is equal to the
                           number of CPU cores available on the device. (default:
-                          8)
+                          6)
     --ttest               Use t-test for evaluating differential expression
                           instead of posterior probabilities. (default: False)
     --write_spectrum_quants
                           Write quantifications for consensus spectra. Only
                           works if consensus spectrum index are given in input.
                           (default: False)
     --write_protein_posteriors P_OUT
@@ -116,14 +125,16 @@
                           file in TSV format. (default: )
     --write_group_posteriors G_OUT
                           Write raw data of treatment group posteriors to the
                           specified file in TSV format. (default: )
     --write_fold_change_posteriors F_OUT
                           Write raw data of fold change posteriors to the
                           specified file in TSV format. (default: )
+    --csv-field-size-limit CSV_FIELD_SIZE_LIMIT
+                          Set a new maximum CSV field size (default: None)
 
 
 Example
 -------
 
 A sample file ``iPRG2016.tsv`` is provided in the ``example`` folder. You can
 run Triqler on this file by running the following command:
```

## Comparing `triqler-0.6.4.dist-info/RECORD` & `triqler-0.7.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 triqler/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 triqler/__main__.py,sha256=4KsrTa5I-Sx5SYo9dkAxVahQ3tXNMxun_xhbfEdfOGE,140
 triqler/convert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-triqler/convert/__main__.py,sha256=pcHtHApFNPAwhN3XODtduoRKbMqGbORgLvBKOeoxEGw,143
+triqler/convert/diann.py,sha256=rpG7yaB7eEBRUvs4oXiQO8BIuyLLiXXDs9pngYoWU-c,2041
 triqler/convert/dinosaur.py,sha256=SlLUbw02sTjWi6DfRBG8d_5IFJKmu0xneyF4aA_eeis,6505
 triqler/convert/helpers.py,sha256=EpQhQ7QcICU1itp44yrAFzUu9allkItAFNQka5axkf4,6022
 triqler/convert/maxquant.py,sha256=ErLgH6Ccg2rtZW0suImfxSHbJUYYp2SL9ldHzrj12C0,6372
 triqler/convert/normalize_intensities.py,sha256=EWpuYIWhVEuAtej-_398IAk4PqMPNo2oUGZoWsEA7mI,5245
 triqler/convert/percolator.py,sha256=S_topa6Upt1Z4JX8vlR-zQhyHnqFSbXj7LLLrEtJGJY,2902
 triqler/convert/quandenser.py,sha256=c_eivM7K_hUldOgjs6A3dV1Hmr6_vGSBvcNB0wI3jGc,6447
 triqler/convolution_dp.py,sha256=kkrkXzFoo_qyiaYhFe-eL-cWsIqXexC8O2VSvbn2390,1127
 triqler/diff_exp.py,sha256=-RkW139-FAz2jQdv4Srdwu4wwly_iUrEjhOMggTTtUk,9823
 triqler/distribution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-triqler/distribution/__main__.py,sha256=ki0Mg-pXGclysyCmEcVF7mX5G-GsuIYw3D0cnkTiZDQ,145
 triqler/distribution/plot_hyperparameter_fits.py,sha256=TSZG5PKcQguz9HX9iQCQimOWnTSU6PTJlbTtbh7ZGdo,2689
 triqler/distribution/plot_posteriors.py,sha256=Pneg3S71aaDrjjgt7o753ijA5jeYkcDTOI2Q-VdfkZk,29078
-triqler/hyperparameters.py,sha256=e40DjQr9CjZBT0n3CRJ1zHWLG8-9eaABmSOGvCAdxqY,11148
+triqler/hyperparameters.py,sha256=cynq1MiULviVRelkus1CUYjEDdMKQvCORPzWBsiD2UY,17329
 triqler/multiprocessing_pool.py,sha256=7-WLPbe4oGxDCBsXXt6liHvWqLTHqpbnBo8csL7GMms,1735
 triqler/parsers.py,sha256=1P5u_XGIzFXmDzVUPguCJNWNP5HC7IixaZ-NS56Is8M,11469
 triqler/pgm.py,sha256=K8ahgtkXJBvfRGR8Dlw6DOV3uWRgQ3Pkfar_0sj5YjY,9551
 triqler/qvality.py,sha256=OKUBqN33ueQZXcwNfCFvsTCkSsvb2CsokBCfOraqXVo,16130
-triqler/triqler.py,sha256=iPgK95ai8H9qBfmaIn6TAC5UBtF4Z222MOslzVK8-_A,23385
+triqler/triqler.py,sha256=ViKI3oR06mGsSLOQL9E8574GXmDdnWztjpXBqElOm_I,23827
 triqler/version.py,sha256=zzbjDF36eHFnDr1FmWabpC8EPDbZ16N5ExMFhM1smPQ,1018
-triqler-0.6.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-triqler-0.6.4.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-triqler-0.6.4.dist-info/METADATA,sha256=LFyz7nV4vplgOSL-Z7MguanmYCx-mvnhzMqYYuzgGZQ,10067
-triqler-0.6.4.dist-info/RECORD,,
+triqler-0.7.0.dist-info/entry_points.txt,sha256=BjsG9Dsy4s82N-4fVE_AymOkM3HhvbjU5rovQmj4oQE,368
+triqler-0.7.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+triqler-0.7.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+triqler-0.7.0.dist-info/METADATA,sha256=PZI4uxGV2fCyVD2_IM3-tmeNTD1ViqGSIhnr8EugCXc,10942
+triqler-0.7.0.dist-info/RECORD,,
```

