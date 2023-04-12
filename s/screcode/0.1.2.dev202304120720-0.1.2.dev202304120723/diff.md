# Comparing `tmp/screcode-0.1.2.dev202304120720-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304120723-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 119267 bytes, number of entries: 6
+Zip file size: 119252 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    60761 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120720.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120720.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304120720.dist-info/RECORD
-6 files, 211547 bytes uncompressed, 118363 bytes compressed:  44.0%
+-rw-r--r--  2.0 unx    60737 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120723.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304120723.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304120723.dist-info/RECORD
+6 files, 211523 bytes uncompressed, 118348 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304120720.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304120723.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304120720.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304120723.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304120720.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304120723.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -494,17 +494,17 @@
 		fig = plt.figure(figsize=figsize)
 		plt.rcParams['xtick.direction'] = 'in'
 		plt.rcParams['ytick.direction'] = 'in'
 		spec = matplotlib.gridspec.GridSpec(ncols=2, nrows=1,width_ratios=[4, 1],wspace=0.)
 		ax0 = fig.add_subplot(spec[0])
 		if self.seq_target == 'Multiome':
 			ax0.scatter(x[idx_sig & (self.idx_atac==False)],y[idx_sig & (self.idx_atac==False)],color='b',s=ps,label='significant genes' ,zorder=2,marker='o',facecolor='None')
-			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None',s=5)
+			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None')
 			ax0.scatter(x[idx_nonsig & (self.idx_atac==False)],y[idx_nonsig & (self.idx_atac==False)],color='r',s=ps,label='non-significant genes',zorder=3,marker='x')
-			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x',s=5)
+			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x')
 		else:
 			ax0.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %s' % self.unit,zorder=2)
 			ax0.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %s' % self.unit,zorder=3)
 		ax0.axhline(1,color='gray',ls='--',lw=2,zorder=1)
 		ax0.set_xscale('log')
 		ax0.set_yscale('log')
 		ax0.set_title(title,fontsize=14)
@@ -707,17 +707,17 @@
 		ps = 2
 		gs = GridSpecFromSubplotSpec(nrows=1,ncols=2,width_ratios=[4, 1],subplot_spec=gs_master[37:85,8:100],wspace=0.)
 		ax0 = fig.add_subplot(gs[0,0])
 		x,y = np.mean(X_scaled,axis=0),norm_var
 		idx_nonsig, idx_sig = y <= 1, y > 1
 		if self.seq_target == 'Multiome':
 			ax0.scatter(x[idx_sig & (self.idx_atac==False)],y[idx_sig & (self.idx_atac==False)],color='b',s=ps,label='significant genes' ,zorder=2,marker='o',facecolor='None')
-			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None',s=5)
+			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None')
 			ax0.scatter(x[idx_nonsig & (self.idx_atac==False)],y[idx_nonsig & (self.idx_atac==False)],color='r',s=ps,label='non-significant genes',zorder=3,marker='x')
-			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x',s=5)
+			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x')
 		else:
 			ax0.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %s' % self.unit,zorder=2)
 			ax0.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %s' % self.unit,zorder=3)
 		# ax0.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %ss' % self.unit,zorder=2)
 		# ax0.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %ss' % self.unit,zorder=3)
 		ax0.axhline(1,color='gray',ls='--',lw=2,zorder=1)
 		ax0.set_xscale('log')
@@ -791,17 +791,17 @@
 		gs = GridSpecFromSubplotSpec(nrows=1,ncols=2,subplot_spec=gs_master[163:200,5:100])
 		ax0 = fig.add_subplot(gs[0,0])
 		plt.rcParams['xtick.direction'] = 'in'
 		plt.rcParams['ytick.direction'] = 'in'
 		x,y = np.mean(X_ss_log,axis=0),np.var(X_ss_log,axis=0,ddof=1)
 		if self.seq_target == 'Multiome':
 			ax0.scatter(x[idx_sig & (self.idx_atac==False)],y[idx_sig & (self.idx_atac==False)],color='b',s=ps,label='significant genes' ,zorder=2,marker='o',facecolor='None')
-			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None',s=5)
+			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='lightblue',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None')
 			ax0.scatter(x[idx_nonsig & (self.idx_atac==False)],y[idx_nonsig & (self.idx_atac==False)],color='r',s=ps,label='non-significant genes',zorder=3,marker='x')
-			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x',s=5)
+			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='orange',s=ps,label='non-significant peaks',zorder=3,marker='x')
 		else:
 			ax0.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %s' % self.unit,zorder=2)
 			ax0.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %s' % self.unit,zorder=3)
 		# ax0.scatter(x,y,color='b',s=ps,label='significant %ss' % self.unit,zorder=2)
 		ax0.axhline(0,color='gray',ls='--',lw=2,zorder=1)
 		ax0.set_xlabel('Mean',fontsize=fs_label)
 		ax0.set_ylabel('Variance',fontsize=fs_label)
```

## Comparing `screcode-0.1.2.dev202304120720.dist-info/METADATA` & `screcode-0.1.2.dev202304120723.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304120720
+Version: 0.1.2.dev202304120723
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

