# Comparing `tmp/cellmap-1.0.1.dev202304110129-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304120506-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8546 bytes, number of entries: 5
+Zip file size: 8861 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    40660 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304110129.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304110129.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304110129.dist-info/RECORD
-5 files, 42791 bytes uncompressed, 7792 bytes compressed:  81.8%
+-rw-r--r--  2.0 unx    42978 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120506.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120506.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304120506.dist-info/RECORD
+5 files, 45109 bytes uncompressed, 8107 bytes compressed:  82.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304110129.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304120506.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304110129.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304120506.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304110129.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304120506.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -189,15 +189,15 @@
     basis = 'umap',
     potential_key = 'Hodge_potential',
     potential_vkey = 'potential_velocity',
     rotation_key = 'Hodge_rotation',
     rotation_vkey = 'rotation_velocity',
     graph_key = 'CM_graph',
     graph_method = 'Delauney',
-    alpha = 0.2,
+    HD_rate = 0.2,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
     logscale_vel = True,
     ):
@@ -247,28 +247,28 @@
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(exp_HD.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
-    if alpha > 0:
+    if HD_rate > 0:
         idx_vel_HD = np.isnan(vel_HD[0])==False
         X1,X2 = exp_HD[:,idx_vel_HD][source],exp_HD[:,idx_vel_HD][target]
         V1,V2 = vel_HD[:,idx_vel_HD][source],vel_HD[:,idx_vel_HD][target]
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
         edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel_HD)
         # edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         edge_vel_HD_norm = np.linalg.norm(edge_vel_HD)
         if edge_vel_HD_norm > 0: edge_vel_HD = edge_vel_HD/edge_vel_HD_norm
     else:
         edge_vel_HD = 0
     
-    if alpha < 1:
+    if HD_rate < 1:
         idx_vel_LD = np.isnan(vel_LD[0])==False
         X1,X2 = exp_LD[:,idx_vel_LD][source],exp_LD[:,idx_vel_LD][target]
         V1,V2 = vel_LD[:,idx_vel_LD][source],vel_LD[:,idx_vel_LD][target]
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
         V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
         V1_p[V1_p<0] = 0
@@ -280,15 +280,15 @@
     ## Solve potential
     n_edge_ = len(source)
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
     lap = -np.dot(div_mat,grad_mat)
-    edge_vel = (1-alpha)*edge_vel_LD+alpha*edge_vel_HD
+    edge_vel = (1-HD_rate)*edge_vel_LD+HD_rate*edge_vel_HD
     source_term = np.dot(div_mat,edge_vel)
     lap_inv = np.linalg.pinv(lap)
     potential = np.dot(lap_inv,source_term)
     pot_flow = -np.dot(grad_mat,potential)
     adata.obs[potential_key] = potential - np.min(potential)
 
     rot_flow = edge_vel - pot_flow
@@ -555,31 +555,79 @@
     adata,
     basis = 'umap',
     vkey = 'velocity',
     potential_key = 'Hodge_potential',
     potential_vkey = 'potential_velocity',
     rotation_key = 'Hodge_rotation',
     rotation_vkey = 'rotation_velocity',
+    cluster_key = 'clusters',
     density = 4,
-    alpha=0.5,
+    alpha=0.3,
     **kwargs
     ):
     
-    kwargs_arg = check_arguments(adata,basis = basis)
+    kwargs_arg = check_arguments(adata,
+                             basis = basis,
+                             potential_key = potential_key,
+                            )
     basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
+    pot_vkey_ = '%s_%s' % (potential_vkey,basis)
+    rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
     
     fig,ax = plt.subplots(1,3,figsize=(24,8),tight_layout=True)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],
-                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],
-                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],
-                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2)
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],color=cluster_key,
+                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],color=cluster_key,
+                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
+                                     show=False,density=density,alpha=alpha,fontsize=18,legend_fontsize=16, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
 
 
+def view_quiver(
+    adata,
+    basis = 'umap',
+    vkey = 'velocity',
+    potential_vkey = 'potential_velocity',
+    rotation_vkey = 'rotation_velocity',
+    cluster_key='clusters',
+    alpha=0.3,
+    fontsize = 18,
+    **kwargs
+    ):
+    
+    kwargs_arg = check_arguments(adata,basis = basis)
+    basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
+    vkey_ = '%s_%s' % (vkey,basis)
+    pot_vkey_ = '%s_%s' % (potential_vkey,basis)
+    rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
+    cluster_set = np.unique(adata.obs[cluster_key].values)
+    cmap = plt.get_cmap("tab20")
+    color = np.zeros(adata.shape[0],dtype=int)
+    for j in range(len(cluster_set)):
+        idx = adata.obs[cluster_key] == cluster_set[j]
+        color[idx] = j
+    fig,ax = plt.subplots(1,3,figsize=(24,8),tight_layout=True)
+    for i in range(3):
+        for j in range(len(cluster_set)):
+            idx = adata.obs[cluster_key] == cluster_set[j]
+            ax[i].scatter(adata.obsm[basis_key][idx,0],adata.obsm[basis_key][idx,1],s=200,alpha=alpha,label=cluster_set[j],color=cmap(j),zorder=0)
+            ax[i].text(np.mean(adata.obsm[basis_key][idx,0]),np.mean(adata.obsm[basis_key][idx,1]),cluster_set[j],fontsize=fontsize,
+                       ha='center',va='center',weight='bold')
+    ax[0].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[vkey_][:,0],adata.obsm[vkey_][:,1],scale=1,zorder=1)
+    ax[0].set_title('RNA velocity',fontsize=fontsize)
+    ax[0].axis('off')
+    ax[1].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[pot_vkey_][:,0],adata.obsm[pot_vkey_][:,1],scale=1,zorder=1,**kwargs)
+    ax[1].set_title('Potential flow',fontsize=fontsize)
+    ax[1].axis('off')
+    ax[2].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[rot_vkey_][:,0],adata.obsm[rot_vkey_][:,1],scale=1,zorder=1,**kwargs)
+    ax[2].set_title('Rotational flow',fontsize=fontsize)
+    ax[2].axis('off')
+
 def view_surface_genes(
     adata,
     genes,
     exp_key = None,
     basis = 'umap',
     vel_key  = 'velocity',
     potential_key = 'Hodge_potential',
```

## Comparing `cellmap-1.0.1.dev202304110129.dist-info/METADATA` & `cellmap-1.0.1.dev202304120506.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304110129
+Version: 1.0.1.dev202304120506
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

