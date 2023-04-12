# Comparing `tmp/explai-0.5.tar.gz` & `tmp/explai-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explai-0.5.tar", last modified: Mon Apr 10 07:29:19 2023, max compression
+gzip compressed data, was "explai-0.6.tar", last modified: Wed Apr 12 07:05:17 2023, max compression
```

## Comparing `explai-0.5.tar` & `explai-0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 07:29:19.188089 explai-0.5/
--rw-rw-rw-   0        0        0      790 2023-04-10 07:29:19.188089 explai-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 07:29:19.188089 explai-0.5/explai/
--rw-rw-rw-   0        0        0       60 2023-04-10 06:48:30.939730 explai-0.5/explai/__init__.py
--rw-rw-rw-   0        0        0     9229 2023-04-10 07:25:45.539083 explai-0.5/explai/reports.py
--rw-rw-rw-   0        0        0       63 2023-04-09 06:19:21.827327 explai-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1713 2023-04-10 07:27:01.805807 explai-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:05:17.076580 explai-0.6/
+-rw-rw-rw-   0        0        0      790 2023-04-12 07:05:17.076580 explai-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 07:05:17.075553 explai-0.6/explai/
+-rw-rw-rw-   0        0        0       60 2023-04-10 06:48:30.939730 explai-0.6/explai/__init__.py
+-rw-rw-rw-   0        0        0     9396 2023-04-12 07:01:15.497053 explai-0.6/explai/reports.py
+-rw-rw-rw-   0        0        0       63 2023-04-09 06:19:21.827327 explai-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1713 2023-04-12 06:54:06.018355 explai-0.6/setup.py
```

### Comparing `explai-0.5/PKG-INFO` & `explai-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: explai
-Version: 0.5
+Version: 0.6
 Summary: A reporting tool for explainable AI
 Home-page: https://github.com/ritwikbd/explai
 Author: Ritwik Bandyopadhyay
 Author-email: ritwikbanrg@gmail.com
 License: MIT
-Download-URL: https://github.com/ritwikbd/explai/archive/refs/tags/v05.tar.gz
+Download-URL: https://github.com/ritwikbd/explai/archive/refs/tags/v06.tar.gz
 Description: UNKNOWN
 Keywords: Explainable AI,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `explai-0.5/explai/reports.py` & `explai-0.6/explai/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,19 @@
 def getDistro(df_y):
     t9=sns.histplot(df_y)
     t9.set_xlabel("Label Values",fontsize=15)
     t9.set_ylabel("Counts",fontsize=15)
     img9=t9.get_figure()
     img9.savefig("histPlot.png",bbox_inches='tight')
     t9.remove()
+    matplotlib.pyplot.close()
     
 
     
-def classifierReport(df_x,df_y,model,filename="Tesst.pdf"):
+def classifierReport(df_x,df_y,model,filename="explaiReport.pdf"):
     
     import os
     preds=model.predict(df_x)
     predsio=model.predict_proba(df_x)
     
     ct=canvas.Canvas(filename)
     ct.drawString(150,200,"Testfile Content v3")
@@ -151,23 +152,23 @@
     ct.drawString(110,558,'Label Distribution',)
     ct.drawImage("histPlot.png",x=20,y=325,width=266,height=225)
     os.remove("histPlot.png")
 
     
     feats_df=standardFeatImps(pca,df_x)
     getFeatImps(model,df_x,feats_df)
-    ct.drawString(106,248,'Standardised Feature Importance',)
+    ct.drawString(55,248,'Standardised Feature Importance',)
     ct.drawImage("featsBar.png",x=20,y=14,width=250,height=225)
     os.remove("featsBar.png")
     
     
     getPermFeatImp(df_x, df_y, model)
     ct.drawString(346,248,"Permutation Feature Importance")
-    ct.drawImage("barPlot.png",x=295,y=14,height=225,width=270)
-    os.remove("barPlot.png")
+    ct.drawImage("boxPlot.png",x=295,y=14,height=225,width=270)
+    os.remove("boxPlot.png")
     
     ct.save()
     
 
 def getEvals_reg(df_y,preds):
     from sklearn import metrics
     evals=['','','','']
@@ -175,36 +176,39 @@
     evals[1] = str(round(metrics.mean_absolute_error(df_y,preds),2))
     evals[2] = str(round(metrics.mean_absolute_percentage_error(df_y,preds),2))
     evals[3] = str(round(metrics.mean_squared_log_error(df_y,preds),2))
     return evals
 
 def getPermFeatImp(df_x,df_y,model):
     from sklearn.inspection import permutation_importance
+    matplotlib.pyplot.ticklabel_format(style='plain', axis='y')
     result_test = permutation_importance(model, df_x, df_y, n_repeats=20, random_state=42, n_jobs=2)
     sorted_importances_idx_test = result_test.importances_mean.argsort()
     importances_test = pd.DataFrame(result_test.importances[sorted_importances_idx_test].T,columns=df_x.columns[sorted_importances_idx_test],)
-    t9=sns.barplot(data=importances_test, orient='h')
+    t9=sns.boxplot(data=importances_test, orient='h')
     t9.set_xlabel("Importance",fontsize=15)
     t9.set_ylabel("Feature",fontsize=15)
     img9=t9.get_figure()
-    img9.savefig("barPlot.png",bbox_inches='tight')
+    img9.savefig("boxPlot.png",bbox_inches='tight')
     t9.remove()
+    matplotlib.pyplot.close()
 
 
 def getResidual(df_y,preds):
     residuals=df_y-preds
     t8=sns.scatterplot(y=residuals,x=df_y)
     t8.set_xlabel("Actual",fontsize=15)
     t8.set_ylabel("Residual",fontsize=15)
     img8=t8.get_figure()
     img8.savefig("scatterPlot.png",bbox_inches='tight')
     t8.remove()
+    matplotlib.pyplot.close()
 
 
-def regressorReport(df_x,df_y,model,filename="TesstRef.pdf"):
+def regressorReport(df_x,df_y,model,filename="explaiReport.pdf"):
     
     import os
     preds=model.predict(df_x)
     
     ct=canvas.Canvas(filename)
     
     ct.setFont(psfontname='Times-Roman',size=15)
@@ -232,15 +236,15 @@
     ct.drawString(435,282,evals[2])
     
     feats_df=standardFeatImps(pca,df_x)
     
     
     getFeatImps(model,df_x,feats_df)
     ct.setFont(psfontname='Times-Roman',size=15)
-    ct.drawString(106,248,'Standardised Feature Importance',)
+    ct.drawString(55,248,'Standardised Feature Importance',)
     ct.drawImage("featsBar.png",x=20,y=14,width=255,height=225)
     os.remove("featsBar.png")
     
     getDistro(df_y)
     ct.setFont(psfontname='Times-Roman',size=15)
     ct.drawString(110,558,'Label Distribution',)
     ct.drawImage("histPlot.png",x=20,y=325,width=266,height=225)
@@ -251,15 +255,15 @@
     ct.drawString(390,558,"Residual Plot")
     ct.drawImage("scatterPlot.png",x=295,y=325,height=225,width=270)
     os.remove("scatterPlot.png")
     
     getPermFeatImp(df_x, df_y, model)
     ct.setFont(psfontname='Times-Roman',size=15)
     ct.drawString(346,248,"Permutation Feature Importance")
-    ct.drawImage("barPlot.png",x=295,y=14,height=225,width=270)
-    os.remove("barPlot.png")
+    ct.drawImage("boxPlot.png",x=295,y=14,height=225,width=270)
+    os.remove("boxPlot.png")
     
     
     
     ct.save()
```

### Comparing `explai-0.5/setup.py` & `explai-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'explai',         # How you named your package folder (MyLib)
   packages = ['explai'],   # Chose the same as "name"
-  version = '0.5',      # Start with a small number and increase it with every change you make
+  version = '0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A reporting tool for explainable AI',   # Give a short description about your library
   author = 'Ritwik Bandyopadhyay',                   # Type in your name
   author_email = 'ritwikbanrg@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ritwikbd/explai',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ritwikbd/explai/archive/refs/tags/v05.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ritwikbd/explai/archive/refs/tags/v06.tar.gz',    # I explain this later on
   keywords = ['Explainable AI', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'reportlab','scikit-learn','matplotlib','seaborn','pandas'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

