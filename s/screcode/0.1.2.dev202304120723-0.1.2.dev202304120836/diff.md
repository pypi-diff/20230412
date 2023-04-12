# Comparing `tmp/screcode-0.1.2.dev202304120723-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304120836-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 119252 bytes, number of entries: 6
+Zip file size: 119303 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    60737 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120723.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120723.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304120723.dist-info/RECORD
-6 files, 211523 bytes uncompressed, 118348 bytes compressed:  44.0%
+-rw-r--r--  2.0 unx    61615 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120836.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120836.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304120836.dist-info/RECORD
+6 files, 212401 bytes uncompressed, 118399 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304120723.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304120836.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304120723.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304120836.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304120723.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304120836.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -808,15 +808,23 @@
 		ax0.set_title(titles[0],fontsize=fs_title)
 		ylim = [-0.05*np.percentile(y,99.9),1.05*np.percentile(y,99.9)]
 		ax0.set_ylim(ylim)	
 		plt.gca().spines['right'].set_visible(False)
 		plt.gca().spines['top'].set_visible(False)
 		ax1 = fig.add_subplot(gs[0,1])
 		x,y = np.mean(X_RECODE_ss_log,axis=0),np.var(X_RECODE_ss_log,axis=0,ddof=1)
-		ax1.scatter(x,y,color='b',s=ps,label='significant %ss' % self.unit,zorder=2)
+		# ax1.scatter(x,y,color='b',s=ps,label='significant %ss' % self.unit,zorder=2)
+		if self.seq_target == 'Multiome':
+			ax1.scatter(x[idx_sig & (self.idx_atac==False)],y[idx_sig & (self.idx_atac==False)],color='b',s=ps,label='significant genes' ,zorder=2,marker='o',facecolor='None')
+			ax1.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None')
+			ax1.scatter(x[idx_nonsig & (self.idx_atac==False)],y[idx_nonsig & (self.idx_atac==False)],color='r',s=ps,label='non-significant genes',zorder=3,marker='x')
+			ax1.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x')
+		else:
+			ax1.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %s' % self.unit,zorder=2)
+			ax1.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %s' % self.unit,zorder=3)
 		ax1.set_ylim(ylim)
 		ax1.axhline(0,color='gray',ls='--',lw=2,zorder=1)
 		ax1.set_xlabel('Mean',fontsize=fs_label)
 		ax1.set_ylabel('Variance',fontsize=fs_label)
 		ax1.set_title(titles[1],fontsize=fs_title)
 		plt.gca().spines['right'].set_visible(False)
 		plt.gca().spines['top'].set_visible(False)
```

## Comparing `screcode-0.1.2.dev202304120723.dist-info/METADATA` & `screcode-0.1.2.dev202304120836.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304120723
+Version: 0.1.2.dev202304120836
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

