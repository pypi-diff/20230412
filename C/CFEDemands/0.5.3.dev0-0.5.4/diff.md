# Comparing `tmp/CFEDemands-0.5.3.dev0-py2.py3-none-any.whl.zip` & `tmp/CFEDemands-0.5.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 47322 bytes, number of entries: 15
--rw-rw----  2.0 unx        9 b- defN 23-Feb-14 01:43 cfe/VERSION
--rw-rw----  2.0 unx      342 b- defN 23-Feb-14 01:40 cfe/__init__.py
--rw-rw----  2.0 unx    18602 b- defN 23-Feb-14 05:32 cfe/df_utils.py
--rw-rw----  2.0 unx     5576 b- defN 23-Feb-14 05:32 cfe/dgp.py
--rw-rw----  2.0 unx    41290 b- defN 23-Feb-14 05:32 cfe/estimation.py
--rw-rw----  2.0 unx     3409 b- defN 23-Feb-14 05:32 cfe/input_files.py
--rw-rw----  2.0 unx    60351 b- defN 23-Feb-14 05:32 cfe/regression.py
+Zip file size: 47307 bytes, number of entries: 15
+-rw-rw----  2.0 unx        6 b- defN 23-Apr-12 21:38 cfe/VERSION
+-rw-rw----  2.0 unx      342 b- defN 23-Feb-14 05:42 cfe/__init__.py
+-rw-rw----  2.0 unx    18602 b- defN 23-Apr-12 21:38 cfe/df_utils.py
+-rw-rw----  2.0 unx     5576 b- defN 23-Apr-12 21:38 cfe/dgp.py
+-rw-rw----  2.0 unx    41290 b- defN 23-Apr-12 21:38 cfe/estimation.py
+-rw-rw----  2.0 unx     3409 b- defN 23-Apr-12 21:38 cfe/input_files.py
+-rw-rw----  2.0 unx    60892 b- defN 23-Apr-12 21:38 cfe/regression.py
 -rw-rw----  2.0 unx      292 b- defN 23-Feb-14 01:42 cfe/requirements.txt
--rw-rw----  2.0 unx    32526 b- defN 23-Feb-14 05:32 cfe/result.py
--rw-rw----  2.0 unx      282 b- defN 23-Feb-14 05:34 CFEDemands-0.5.3.dev0.dist-info/LICENSE.txt
--rw-rw----  2.0 unx     1769 b- defN 23-Feb-14 05:34 CFEDemands-0.5.3.dev0.dist-info/METADATA
--rw-rw----  2.0 unx      110 b- defN 23-Feb-14 05:34 CFEDemands-0.5.3.dev0.dist-info/WHEEL
--rw-rw----  2.0 unx        4 b- defN 23-Feb-14 05:34 CFEDemands-0.5.3.dev0.dist-info/top_level.txt
--rw-rw----  2.0 unx        1 b- defN 22-Oct-11 04:24 CFEDemands-0.5.3.dev0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1171 b- defN 23-Feb-14 05:34 CFEDemands-0.5.3.dev0.dist-info/RECORD
-15 files, 165734 bytes uncompressed, 45402 bytes compressed:  72.6%
+-rw-rw----  2.0 unx    32526 b- defN 23-Apr-12 21:38 cfe/result.py
+-rw-rw----  2.0 unx      282 b- defN 23-Apr-12 21:39 CFEDemands-0.5.4.dist-info/LICENSE.txt
+-rw-rw----  2.0 unx     1764 b- defN 23-Apr-12 21:39 CFEDemands-0.5.4.dist-info/METADATA
+-rw-rw----  2.0 unx      110 b- defN 23-Apr-12 21:39 CFEDemands-0.5.4.dist-info/WHEEL
+-rw-rw----  2.0 unx        4 b- defN 23-Apr-12 21:39 CFEDemands-0.5.4.dist-info/top_level.txt
+-rw-rw----  2.0 unx        1 b- defN 22-Oct-11 04:24 CFEDemands-0.5.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1141 b- defN 23-Apr-12 21:39 CFEDemands-0.5.4.dist-info/RECORD
+15 files, 166237 bytes uncompressed, 45447 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: cfe/requirements.txt
 Comment: 
 
 Filename: cfe/result.py
 Comment: 
 
-Filename: CFEDemands-0.5.3.dev0.dist-info/LICENSE.txt
+Filename: CFEDemands-0.5.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: CFEDemands-0.5.3.dev0.dist-info/METADATA
+Filename: CFEDemands-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: CFEDemands-0.5.3.dev0.dist-info/WHEEL
+Filename: CFEDemands-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: CFEDemands-0.5.3.dev0.dist-info/top_level.txt
+Filename: CFEDemands-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: CFEDemands-0.5.3.dev0.dist-info/zip-safe
+Filename: CFEDemands-0.5.4.dist-info/zip-safe
 Comment: 
 
-Filename: CFEDemands-0.5.3.dev0.dist-info/RECORD
+Filename: CFEDemands-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cfe/VERSION

```diff
@@ -1 +1 @@
-0.5.3dev
+0.5.4
```

## cfe/df_utils.py

```diff
@@ -1,9 +1,9 @@
 # [[file:../Empirics/cfe_estimation.org::df_utils][df_utils]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: df_utils
 
 import numpy as np
 from scipy import sparse
 import pandas as pd
 from warnings import warn
 
@@ -332,15 +332,15 @@
     return tuple(Y)
 
 def use_indices(df,idxnames):
     return df.reset_index()[idxnames].set_index(df.index)
 # df_utils ends here
 
 # [[file:../Empirics/cfe_estimation.org::*Some econometric routines][Some econometric routines:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 import warnings
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore",category=UserWarning)
     import xarray as xr
 
 from scipy.linalg import block_diag
 
@@ -442,15 +442,15 @@
         if return_e:
             out.append(u)
 
     return tuple(out)
 # Some econometric routines:1 ends here
 
 # [[file:../Empirics/cfe_estimation.org::broadcast_binary_op][broadcast_binary_op]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: broadcast_binary_op
 
 def merge_multi(df1, df2, on):
     """Merge on subset of multiindex.
    
     Idea due to http://stackoverflow.com/questions/23937433/efficiently-joining-two-dataframes-based-on-multiple-levels-of-a-multiindex
     """
@@ -479,15 +479,15 @@
 
     newdf = op(x[cols],z[cols])
 
     return newdf
 # broadcast_binary_op ends here
 
 # [[file:../Empirics/cfe_estimation.org::*Utility functions related to transformations between xarray and pandas objects][Utility functions related to transformations between xarray and pandas objects:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: broadcast_binary_op
 
 import warnings
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore",category=UserWarning)
     import xarray as xr
```

## cfe/dgp.py

```diff
@@ -1,9 +1,9 @@
 # [[file:../Empirics/cfe_estimation.org::lambdas_dgp][lambdas_dgp]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: lambdas_dgp
 
 from scipy.stats.distributions import lognorm
 import numpy as np
 
 import warnings
 with warnings.catch_warnings():  
@@ -29,24 +29,24 @@
     L = xr.concat((L0,innov),dim='t').transpose('j','t','m')
   
     # Add aggregate shocks Lbar:
     return L*lambdabar(T,M,Fbar=Fbar)
 # lambdas_dgp ends here
 
 # [[file:../Empirics/cfe_estimation.org::characteristics_dgp][characteristics_dgp]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: characteristics_dgp
 
 def characteristics(N,T,M=1): 
     z = lambdas(N,T,M,Fbar=geometric_brownian(.05),F=geometric_brownian(0.1))
     return z
 # characteristics_dgp ends here
 
 # [[file:../Empirics/cfe_estimation.org::prices_dgp][prices_dgp]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: prices_dgp
 
 def prices(T,M,n,G0=lognorm(.5),Fbar=geometric_brownian(.05),F=geometric_brownian(.2)):
 
     P0 = xr.DataArray(G0.rvs(size=(n,1,M)),dims=('i','t','m'),
                       coords={'i':range(n),'t':range(1),'m':range(M)})  # Initial lambdas
     innov = xr.DataArray(F.rvs(size=(n,T-1,M)),dims=('i','t','m'),
@@ -55,15 +55,15 @@
     P = xr.concat((P0,innov),dim='t').transpose('t','m','i')
     
     # Add aggregate shocks L0:
     return P*lambdabar(T,M,Fbar=Fbar)
 # prices_dgp ends here
 
 # [[file:../Empirics/cfe_estimation.org::expenditures_dgp][expenditures_dgp]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: expenditures_dgp
 
 #name: measurement_error_dgp
 
 import pandas as pd
 from scipy.stats import distributions
 import numpy as np
```

## cfe/estimation.py

```diff
@@ -1,9 +1,9 @@
 # [[file:../Empirics/cfe_estimation.org::agg_shares_and_mean_shares][agg_shares_and_mean_shares]]
-# Tangled on Mon Feb 13 21:32:52 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: agg_shares_and_mean_shares
 
 import pylab as pl
 import pandas as pd
 import numpy as np
 from cfe.df_utils import broadcast_binary_op, is_none
 from itertools import cycle
@@ -161,30 +161,30 @@
     if figname:
         pl.savefig(figname)
 
     return tab,ax
 # agg_shares_and_mean_shares ends here
 
 # [[file:../Empirics/cfe_estimation.org::group_expenditures][group_expenditures]]
-# Tangled on Mon Feb 13 21:32:52 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: group_expenditures
 def group_expenditures(df,groups):
     myX=pd.DataFrame(index=df.index)
     for k,v in groups.items():
         if len(k):
             myv = [int(i) for i in v if len(str(i))>0]
             try:
                 myX[k]=df[['$x_{%d}$' % int(i) for i in myv]].sum(axis=1)
             except KeyError: pass
             
     return myX
 # group_expenditures ends here
 
 # [[file:../Empirics/cfe_estimation.org::svd_rank1_approximation_with_missing_data][svd_rank1_approximation_with_missing_data]]
-# Tangled on Mon Feb 13 21:32:52 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: svd_rank1_approximation_with_missing_data
 import pandas as pd
 #name: svd_missing
 
 import numpy as np
 import warnings
 
@@ -407,15 +407,15 @@
         else:
             out = (out,u,s,v)
 
     return out
 # svd_rank1_approximation_with_missing_data ends here
 
 # [[file:../Empirics/cfe_estimation.org::estimate_reduced_form][estimate_reduced_form]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: estimate_reduced_form
 import pandas as pd
 import warnings
 import sys
 from collections import OrderedDict
 from cfe.df_utils import drop_missing, ols, arellano_robust_cov, broadcast_binary_op, use_indices, df_norm
 
@@ -556,15 +556,15 @@
   if return_v:
       V = xr.Dataset(V).to_array(dim='i')
       out += [V]
   return out
 # estimate_reduced_form ends here
 
 # [[file:../Empirics/cfe_estimation.org::get_loglambdas][get_loglambdas]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: get_loglambdas
 
 import pandas as pd
 
 try: 
     from joblib import Parallel, delayed
     #import timeit
@@ -714,15 +714,15 @@
     if len(out)==1:
         return out[0]
     else:
         return out
 # get_loglambdas ends here
 
 # [[file:../Empirics/cfe_estimation.org::direct_price_elasticities][direct_price_elasticities]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: direct_price_elasticities
 
 def direct_price_elasticities(y,p,z,VERBOSE=True,return_se=False,return_v=False):
     """Estimate reduced-form Frisch expenditure/demand system.
 
        Inputs:
          - y : pd.DataFrame of log expenditures or log quantities, indexed by (j,t,m), 
@@ -782,15 +782,15 @@
         out += [sed]
     if return_v:
         out += [V]
     return out
 # direct_price_elasticities ends here
 
 # [[file:../Empirics/cfe_estimation.org::*Indirect estimation of price elasticities][Indirect estimation of price elasticities:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 def indirect_price_elasticities(a,p,zbar):
     """Estimate reduced-form Frisch expenditure/demand system.
 
        Inputs:
          - a : pd.DataFrame of good-time-market effects estimated by =estimate_reduced_form=,
                indexed by (t,m), where t indexes the period, and m the market.  
                Columns are different expenditure items.
@@ -828,15 +828,15 @@
 
     B = pd.Series(B)
     SE = pd.Series(SE)
     return B,SE
 # Indirect estimation of price elasticities:1 ends here
 
 # [[file:../Empirics/cfe_estimation.org::*Iterated Regression][Iterated Regression:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 def iterated_regression(y,z,return_se=False,return_v=False,VERBOSE=False,tol=1e-3,max_its=30,cores=None):
     """Estimate (delta,beta,loglambda).
     """
 
     # Create location-time dummies
     dm = use_indices(y,['t','m'])
     DateLocD = pd.get_dummies(zip(dm['t'],dm['m']))
@@ -932,15 +932,15 @@
         SE.index.name = 'i'
         out = out + [SE,V]
 
     return tuple(out)
 # Iterated Regression:1 ends here
 
 # [[file:../Empirics/cfe_estimation.org::analysis_omnibus][analysis_omnibus]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: analysis_omnibus
 
 # -*- coding: utf-8 -*-
 
 import tempfile
 import numpy as np
 import pandas as pd
@@ -1079,15 +1079,15 @@
     results['logexpenditures'] = y
     results['logexpenditures_hat'] = yhat
 
     return results
 # analysis_omnibus ends here
 
 # [[file:../Empirics/cfe_estimation.org::elasticities_equal][elasticities_equal]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: elasticities_equal
 
 import numpy as np
 from scipy.optimize import minimize_scalar
 from scipy.stats.distributions import f as F
 
 def elasticities_equal(b1,b2,v1,v2,N,N2,pvalue=False,criterion=False):
@@ -1135,15 +1135,15 @@
     if criterion:
         outputs.append(Fcriterion)
     
     return tuple(outputs)
 # elasticities_equal ends here
 
 # [[file:../Empirics/cfe_estimation.org::predicted_expenditures][predicted_expenditures]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: predicted_expenditures
 
 import numpy as np
 
 def predicted_expenditures(yhat,e):
     """
     Return levels of predicted expenditures.
@@ -1158,15 +1158,15 @@
 
     x = np.exp(yhat + ebar + evar/2)
 
     return x
 # predicted_expenditures ends here
 
 # [[file:../Empirics/cfe_estimation.org::optimal_index][optimal_index]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 #name: optimal_index
 
 import warnings
 with warnings.catch_warnings():  
     warnings.filterwarnings("ignore",category=UserWarning)
     import xarray as xr
```

## cfe/input_files.py

```diff
@@ -1,9 +1,9 @@
 # [[file:../Files/input_files.org::*Code for constructing inputs to CFEDemands from *.dta files][Code for constructing inputs to CFEDemands from *.dta files:1]]
-# Tangled on Mon Feb 13 21:32:54 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import numpy as np
 import pandas as pd
 from collections import defaultdict
 
 try:  # If we can't load dvc, take a pass and fail only if we call.
     import dvc.api
 except ModuleNotFoundError:
```

## cfe/regression.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # [[file:../Empirics/regression.org::*Outer product of two series][Outer product of two series:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import numpy as np
 import pandas as pd
 
 def outer(a,b):
     """
     Outer product of two series.
     """
@@ -25,15 +25,15 @@
     except AttributeError:
         x = pd.DataFrame(x)
 
     return x
 # Outer product of two series:1 ends here
 
 # [[file:../Empirics/regression.org::*Inner product][Inner product:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def to_series(df):
     """
     Stack a dataframe to make a series.
     """
     try:
         df.columns.names = [n if n is not None else "_%d" % i for i,n in enumerate(df.columns.names)]
     except AttributeError: # Already a series?
@@ -95,15 +95,15 @@
     if len(colsout):
         p = p.sort_index(axis=1)
 
     return p
 # Inner product:1 ends here
 
 # [[file:../Empirics/regression.org::*SVD with missing data][SVD with missing data:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import pandas as pd
 import numpy as np
 
 def svd_missing(X,gls=False):
     """
     Compute rank one approximation to X.
     """
@@ -138,15 +138,15 @@
     scale = np.sqrt(v.T@v)
     u = pd.Series(u[:,-1],index=b.index)
 
     return u,np.sqrt(s2[-1])*scale,v/scale
 # SVD with missing data:1 ends here
 
 # [[file:../Empirics/regression.org::*Angle between vectors (or series)][Angle between vectors (or series):1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 """
 Compute angle between two vectors, thx to https://stackoverflow.com/questions/2827393/angles-between-two-n-dimensional-vectors-in-python/13849249#13849249
 """
 import numpy as np
 
 def unit_vector(vector):
     """ Returns the unit vector of the vector.  """
@@ -164,15 +164,15 @@
     """
     v1_u = unit_vector(v1)
     v2_u = unit_vector(v2)
     return np.arccos(np.clip(np.dot(v1_u, v2_u), -1.0, 1.0))
 # Angle between vectors (or series):1 ends here
 
 # [[file:../Empirics/regression.org::*OLS][OLS:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def ols(y,x):
     try:
         xcols = x.columns
     except AttributeError:
         xcols = x
         x = y[xcols]
         y = y[y.columns.difference(xcols)]
@@ -181,26 +181,26 @@
 
     b = np.linalg.lstsq(x,y,rcond=None)[0]
 
     return pd.Series(b.squeeze(),index=x.columns)
 # OLS:1 ends here
 
 # [[file:../Empirics/regression.org::*Inter-quartile range][Inter-quartile range:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def iqr(x,std=False):
     y = np.diff(x.quantile([0.25,0.75]))[0]
 
     # Ratio between std deviation and iqr for normal distribution
     if std: y = y*1.3489795
 
     return y
 # Inter-quartile range:1 ends here
 
 # [[file:../Empirics/regression.org::code:Mp][code:Mp]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import pandas as pd
 import numpy as np
 from warnings import warn
 
 def Mp(X):
     """
     Construct X-E(X|p) = (I-S(S'S)^{-1}S')X.
@@ -217,15 +217,15 @@
     if len(use):
         return X - X.groupby(use).transform(np.mean)
     else:
         return X - X.mean()
 # code:Mp ends here
 
 # [[file:../Empirics/regression.org::code:Mpi][code:Mpi]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 
 def Mpi(X):
     """
     Construct X-E(X|pi).
 
     Drop any categorical variables where taking means isn't sensible.
     """
@@ -234,15 +234,15 @@
     else:
         if X.dtype == 'category': warn('Taking mean of categorical variable.')
 
     return X - X.groupby(['t','m']).transform(np.mean)
 # code:Mpi ends here
 
 # [[file:../Empirics/regression.org::code:kmeans][code:kmeans]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from sklearn.model_selection import GroupKFold
 from .df_utils import use_indices, drop_missing
 from scipy.optimize import minimize_scalar
 from sklearn.cluster import KMeans
 
 def kmean_controls(n_clusters,Mpy,Mpd,shuffles=0,classifiers=None,verbose=False):
     n_clusters = int(n_clusters)
@@ -343,15 +343,15 @@
             MdX = pd.Series(y.squeeze() - (x@b).squeeze(),index=y.index)
     else: raise ValueError("No method %s." % method)
 
     return MdX
 # code:kmeans ends here
 
 # [[file:../Empirics/regression.org::*Compute $\MdMpy$][Compute $\MdMpy$:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def estimate_MdMpy(y,d,K=None):
 
     if K is not None:
         d,MdMpy = kmean_controls(K,Mp(y),Mp(d),classifiers=d.loc[:,d.dtypes == 'category'])
         MdMp = lambda x: Md_generator(x,d,Mp=True)
         Md = lambda x: Md_generator(x,d,Mp=False)
         method = 'categorical'
@@ -373,15 +373,15 @@
     if not np.all(np.abs(MdMpy.groupby(['j','t','m']).mean()) < 1e-6):
         warn('MdMpy means greater than 1e-6')
 
     return MdMpy,Md,MdMp,d
 # Compute $\MdMpy$:1 ends here
 
 # [[file:../Empirics/regression.org::code:beta_from_MdMpy][code:beta_from_MdMpy]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from .estimation import svd_missing
 import numpy as np
 
 def estimate_beta(MdMpy,
                   heteroskedastic=False,
                   cov = lambda X : pd.DataFrame.cov(X,ddof=0),
                   return_se=False,bootstrap_tol=None,Mdp=None,verbose=False):
@@ -437,15 +437,15 @@
     if return_se:
         return b,seb,V
     else:
         return b,None,None
 # code:beta_from_MdMpy ends here
 
 # [[file:../Empirics/regression.org::*Estimation of $\M{p}w$][Estimation of $\M{p}w$:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from scipy import sparse
 import warnings
 
 def estimate_Mpw(y,b,MdMpy,return_se=False,bootstrap_tol=None,
                  verbose=False):
 
     # Construct regression to compute Mpw
@@ -541,15 +541,15 @@
 
             return Mpw, scale, mults, seb, mults_se, e1
 
     return Mpw,scale,mults
 # Estimation of $\M{p}w$:1 ends here
 
 # [[file:../Empirics/regression.org::*Estimate Lagrange Multipliers][Estimate Lagrange Multipliers:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def estimate_stderrs(y,scale):
 
     cols = y.groupby(['i','t','m']).mean().index
 
     TM = [(np.nan,t,m) for t in y.index.levels[y.index.names.index('t')] for m in y.index.levels[y.index.names.index('m')]]
 
     with warnings.catch_warnings():
@@ -584,15 +584,15 @@
                             name='mults_se')
 
 
     return seb, mults_se, e1
 # Estimate Lagrange Multipliers:1 ends here
 
 # [[file:../Empirics/regression.org::*Estimation of \beta and $\M{p}w$][Estimation of \beta and $\M{p}w$:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from scipy import sparse
 import warnings
 
 def estimate_beta_and_Mpw(y,Mdp,return_se=False,bootstrap_tol=None,
                           verbose=False):
 
     MdMpy = Mdp(y)
@@ -701,15 +701,15 @@
         mults_se = None
         e1 = None
 
     return b,Mpw,seb,mults,mults_se,e1
 # Estimation of \beta and $\M{p}w$:1 ends here
 
 # [[file:../Empirics/regression.org::code:gamma][code:gamma]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def estimate_gamma(y,beta,w,tau,method='categorical',verbose=False):
     """
     Estimate $gamma(tau) = E[Mp(Y -hat{beta}hat{w}) | tau]$.
     """
     if beta is not None:
         e = y.unstack('j') - pd.DataFrame({0:w})@pd.DataFrame({0:beta}).T
     else:
@@ -748,15 +748,15 @@
     #e2 = e - gamma_d.loc[e.index]
     e2 = e - gamma_d.reindex_like(e)
 
     return gamma, gamma_d, e2
 # code:gamma ends here
 
 # [[file:../Empirics/regression.org::code:Ar_w][code:Ar_w]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from scipy import sparse
 from timeit import default_timer as timer
 
 def estimate_w(y,beta,return_se=False,verbose=False):
     """
     Estimate regression $Mpi(Y - widehat{gamma(d)})  =  A(r) + hat{beta}w + e$.
     """
@@ -826,15 +826,15 @@
 
     what = pd.Series(b[len(A.columns):(len(A.columns)+len(B.columns))],index=B.columns)
 
     return what,Ar,Ar_se,e3
 # code:Ar_w ends here
 
 # [[file:../Empirics/regression.org::code:pi][code:pi]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def estimate_pi(y,b,w,Ar,gamma_d,verbose=False):
 
     try:
         y0 = y.stack()
     except AttributeError:
         y0 = y.copy()
 
@@ -856,25 +856,25 @@
     e4 = e - pi
     e4 = e4.reorder_levels(['i','t','m','j']).sort_index()
 
     return pi, pi_se, e4
 # code:pi ends here
 
 # [[file:../Empirics/regression.org::code:predict][code:predict]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def predict_y(pi,Ar,gamma_d,beta,wr):
     bwr = outer(wr,beta).stack()
 
     yhat = pi + Ar + gamma_d + bwr
 
     return yhat.reorder_levels(['i','t','m','j']).sort_index()
 # code:predict ends here
 
 # [[file:../Empirics/regression.org::code:data_preparation][code:data_preparation]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from .df_utils import broadcast_binary_op
 from .estimation import drop_columns_wo_covariance
 import matplotlib.pyplot as plt
 from types import SimpleNamespace
 
 def prepare_data(y,d,min_obs=None,min_prop_items=0.1,alltm=False):
     assert y.index.names == ['i','t','m','j']
@@ -924,15 +924,15 @@
                                                           classifiers=d.loc[:,d.dtypes == 'category'],
                                                           verbose=verbose)[0],
                                     bracket=[1,20]).x)
     return nstar
 # code:data_preparation ends here
 
 # [[file:../Empirics/regression.org::*Construct Missing "correction"][Construct Missing "correction":1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 def missing_correction(y,d,K=None):
     M = 1-np.isnan(y.unstack('j'))  # Non-missing
     M = M.stack()
 
     M,d = prepare_data(M,d)
 
     R =  estimation(M,d,K=K,return_se=False)
@@ -945,15 +945,15 @@
     e = M - Mhat
     R['R2'] = 1-e.var()/M.var()
 
     return e,R
 # Construct Missing "correction":1 ends here
 
 # [[file:../Empirics/regression.org::*Estimate][Estimate:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import time
 
 def estimation(y,d,K=None,beta=None,bootstrap_tol=None,return_se=False,rectify=False,verbose=False):
 
     if K is None: method = 'linear'
     else: method = 'categorical'
 
@@ -1117,15 +1117,15 @@
                 Ar = Ar.unstack(['t','m']),
                 Ar_se = Ar_se,
                 B=B,
                 X=X)
 # Estimate:1 ends here
 
 # [[file:../Empirics/regression.org::*Validate][Validate:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 
 def validate(y,pi,Ar,d,w,beta,gamma,GramSchmidt=False):
     def ols(x):
         y = x['y']
         x = x.drop('y',axis=1)
 
         y,x = drop_missing([y,x])
@@ -1177,15 +1177,15 @@
 
     B = X.groupby('j').apply(lambda x: ols(x))
 
     return B,X
 # Validate:1 ends here
 
 # [[file:../Empirics/regression.org::regression_class][regression_class]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import numpy as np
 import pandas as pd
 import warnings
 from sqlalchemy import create_engine
 from pathlib import Path
 from collections import namedtuple, OrderedDict
 from cfe.df_utils import is_none
@@ -1279,15 +1279,15 @@
         if 'y' in kwargs.keys() and 'd' in kwargs.keys():
             self.y,self.d = prepare_data(self.y,self.d,min_obs=min_obs,
                                          min_prop_items=min_prop_items,
                                          alltm=alltm)
 # regression_class ends here
 
 # [[file:../Empirics/regression.org::*Estimate][Estimate:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
     def estimate(self,beta=None):
 
         if beta is not None:
             beta = pd.DataFrame(beta)
 
         R = estimation(self.y,self.d,
                        K=self.attrs['K'],
@@ -1302,15 +1302,15 @@
                 if getattr(self,k) is not None: continue
                 setattr(self,k,v)
             except AttributeError:
                 setattr(self,k,v)
 # Estimate:1 ends here
 
 # [[file:../Empirics/regression.org::*Persistence][Persistence:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
     def to_sql(self,fn=None,overwrite=False):
         """
         Save to sql database fn.
         """
         if overwrite: if_exists = 'replace'
         else: if_exists = 'fail'
 
@@ -1349,15 +1349,15 @@
 
             d['attrs'] = self.attrs
 
         pd.to_pickle(d,fn)
 # Persistence:1 ends here
 
 # [[file:../Empirics/regression.org::*Accessors][Accessors:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
     def get_MdMpy(self):
         MdMpy,Md,MdMp,d = estimate_MdMpy(self.y,self.d,self.attrs['K'])
 
         self.d = d
 
         self.MdMp = MdMp
         self.Md = Md
@@ -1392,14 +1392,22 @@
         self.beta = b
 
         if return_se:
             return self.beta_se
         else:
             return self.beta
 
+    def get_gamma(self,verbose=None):
+
+        if self.gamma is not None:
+            return self.gamma
+        else:
+            gd = get_gamma_d(self,verbose=verbose)
+            return self.gamma
+
     def get_gamma_d(self,verbose=None):
 
         if self.gamma_d is not None:
             return self.gamma_d
 
         if self.MdMp is None:
             MdMpy = self.get_MdMpy()
@@ -1543,15 +1551,15 @@
             except KeyError:  # d doesn't vary with j?
                 self.gamma_se = np.sqrt((outer(sigma2,1/((d.var()+d.mean()**2)*d.count()))))
 
         return self.gamma_se
 # Accessors:1 ends here
 
 # [[file:../Empirics/regression.org::*Other methods][Other methods:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
     def validate(self,rectify=False,GramSchmidt=False,verbose=False):
         B,X = validate(self.y,
                        self.pi,
                        self.Ar,
                        self.d,
                        self.w,
                        self.beta,
@@ -1656,15 +1664,15 @@
             xhat = np.exp(self.yhat + evar/2)
             xhat = xhat.reorder_levels(self.yhat.index.names).sort_index()
 
         return xhat
 # Other methods:1 ends here
 
 # [[file:../Empirics/regression.org::*Presentation methods][Presentation methods:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
     def graph_beta(self,fn=None,xlabel='Frisch Elasticities'):
         import matplotlib.pyplot as plt
 
         if self.beta is None or self.beta_se is None:
             self.get_beta(return_se=True)
 
         beta = self.beta.sort_values()
@@ -1685,29 +1693,33 @@
         if fn is not None:
             fig.savefig(fn,bbox_inches='tight')
 
         return fig
 # Presentation methods:1 ends here
 
 # [[file:../Empirics/regression.org::regression_demand_interface][regression_demand_interface]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import consumerdemands
 import pandas as pd
 
 def _demand_parameters(self,p=None,d=None):
     """Return tuple of p and dictionary of (alpha,beta,phi) from regression instance.
 
     Suitable for passing to =cfe.demand= functions.
     """
 
     beta = self.beta
     n = len(beta)
 
     if d is None:
-        alpha = np.exp(self.gamma_d.groupby('j').mean())
+        gd = self.get_gamma_d().groupby('j').mean()
+    else:
+        gd = d@self.gamma.T
+
+    alpha = np.exp(gd)
 
     if p is None or len(p)==0:
         prices = np.exp(self.Ar.groupby('j').mean())
     else:
         prices = p
 
     assert len(prices), f"What happened to prices? p={prices}."
@@ -1746,28 +1758,35 @@
           'Hicksian':consumerdemands.hicksian.demands,
           'Frischian':consumerdemands.frischian.demands}
 
     q = pd.Series(Qs[type](x,p,pparms),index=pparms['alpha'].index,name='quantities')
 
     return q
 
-def _utility(self,x,p=None,z=None):
-    """Indirect utility
+def _expenditures(self,x,p=None,z=None,type='Marshallian'):
+    """Expenditures for different goods at prices p for household with observable
+    characteristics z, having a utility function with parameters given
+    by (possibly estimated) attributes from a Regression (i.e., the
+    vectors of parameters alpha, beta, delta).
+
+    Default type is "Marshallian", in which case argument x is budget.
 
-    Varies with prices p, budget x and observable characteristics z,
-    having a utility function with parameters given by (possibly
-    estimated) attributes from a Regression (i.e., the vectors of
-    parameters alpha, beta, delta).
+    Alternative types:
+       - "Frischian" :: argument x is Marginal utility of expenditures
+       - "Hicksian" :: argument x is level of utility
 
-    Ethan Ligon                                    April 2019
+    Ethan Ligon                                    April 2023
     """
 
     p,pparms = _demand_parameters(self,p,z)
 
-    return consumerdemands.marshallian.indirect_utility(x,p,pparms)
+    q = _demands(self,x,p=p,z=z,type=type)
+
+    return p*q
+
 
 def _utility(self,x,p=None,z=None,type="Marshallian"):
     """(Indirect) utility
 
     Level of utility at prices p for household with observable
     characteristics z, having a utility function with parameters given
     by (possibly estimated) attributes from a Regression (i.e., the
@@ -1825,23 +1844,24 @@
 
     p,pparms = _demand_parameters(self,p,z)
 
     return consumerdemands.demands.relative_risk_aversion(p,pparms)
 
 Regression.consumerdemands = consumerdemands
 Regression.demands = _demands
+Regression.expenditures = _expenditures
 Regression.demand_parameters = _demand_parameters
 Regression.lambdavalue = _lambdavalue
 Regression.indirect_utility = _utility
 Regression.expenditure = _expenditurefunction
 Regression.relative_risk_aversion = _relative_risk_aversion
 # regression_demand_interface ends here
 
 # [[file:../Empirics/regression.org::*=read_sql=][=read_sql=:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 from sqlalchemy import inspect, create_engine
 from ast import literal_eval as make_tuple
 
 def read_sql(fn):
     """
     Read Regression object from file fn.
     """
@@ -1876,15 +1896,15 @@
         if not len(R):
             raise OSError(f'Trying to read empty file?  Check {loc}.')
 
     return Regression(**R)
 # =read_sql=:1 ends here
 
 # [[file:../Empirics/regression.org::*=read_pickle=][=read_pickle=:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:14 2023
 import pickle
 
 def read_pickle(fn,cache_dir=None):
     """
     Read pickled dictionary and assign keys as attributes to Regression object.
     """
     import fsspec
```

## cfe/result.py

```diff
@@ -1,9 +1,9 @@
 # [[file:../Empirics/result.org::result_class][result_class]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 import numpy as np
 import pandas as pd
 from . import estimation 
 import warnings
 
 # Funky warning re: cfgrib from xarray we can't do anything about
 with warnings.catch_warnings():  
@@ -688,15 +688,15 @@
 
         R['y'] = R.yhat + R.e
 
         return R
 # result_class ends here
 
 # [[file:../Empirics/result.org::result_to_file][result_to_file]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
     def to_dataset(self,fn=None,**kwargs):
         """Convert Result instance to xarray.Dataset."""
         D = xr.Dataset(self)
 
         if fn is not None:
             D.to_netcdf(fn,**kwargs)
 
@@ -740,15 +740,15 @@
 
     R = Result(data=D)
 
     return R
 # result_to_file ends here
 
 # [[file:../Empirics/result.org::*Drop useless expenditures][Drop useless expenditures:1]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 def _drop_useless_expenditures(y0, attrs, VERBOSE=False):
     """Drop expenditure items with too few observations.
 
     "Too few" depends on the attributes min_proportion_items and min_xproducts.  
     Once called this method sets the attribute 'useless_expenditures' to False.
     """
 
@@ -792,15 +792,15 @@
     _y = y.to_xarray().to_array('i')
     attrs['useless_expenditures'] = False
 
     return _y,attrs
 # Drop useless expenditures:1 ends here
 
 # [[file:../Empirics/result.org::result_demand_interface][result_demand_interface]]
-# Tangled on Mon Feb 13 21:32:53 2023
+# Tangled on Wed Apr 12 14:38:13 2023
 import consumerdemands as demands
 import pandas as pd
 
 def _demand_parameters(self,p=None,z=None):
     """Return tuple of (p,alpha,beta,phi) from result.
 
     Note that the alpha returned is exp(alpha + delta.T z).
```

## Comparing `CFEDemands-0.5.3.dev0.dist-info/METADATA` & `CFEDemands-0.5.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFEDemands
-Version: 0.5.3.dev0
+Version: 0.5.4
 Summary: Tools for estimating and computing Constant Frisch Elasticity (CFE) demands.
 Home-page: https://bitbucket.org/ligonresearch/cfedemands
 Author-email: ligon@berkeley.edu
 License: Creative Commons Attribution-Noncommercial-ShareAlike 4.0 International license
 Description-Content-Type: text/plain
 License-File: LICENSE.txt
 Requires-Dist: ConsumerDemands (>=0.3.dev0)
```

