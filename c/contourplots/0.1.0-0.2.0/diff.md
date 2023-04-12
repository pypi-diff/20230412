# Comparing `tmp/contourplots-0.1.0.tar.gz` & `tmp/contourplots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contourplots-0.1.0.tar", last modified: Fri Feb 17 19:08:03 2023, max compression
+gzip compressed data, was "contourplots-0.2.0.tar", last modified: Wed Apr 12 02:12:36 2023, max compression
```

## Comparing `contourplots-0.1.0.tar` & `contourplots-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 19:08:03.614416 contourplots-0.1.0/
--rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      608 2023-02-17 19:08:03.613420 contourplots-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 19:08:03.600460 contourplots-0.1.0/contourplots/
--rw-rw-rw-   0        0        0      732 2023-02-17 19:07:02.000000 contourplots-0.1.0/contourplots/__init__.py
--rw-rw-rw-   0        0        0    22570 2023-02-10 05:39:20.000000 contourplots-0.1.0/contourplots/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-17 19:08:03.611425 contourplots-0.1.0/contourplots.egg-info/
--rw-rw-rw-   0        0        0      608 2023-02-17 19:08:03.000000 contourplots-0.1.0/contourplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-02-17 19:08:03.000000 contourplots-0.1.0/contourplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 19:08:03.000000 contourplots-0.1.0/contourplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-02-17 19:08:03.000000 contourplots-0.1.0/contourplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-17 19:08:03.000000 contourplots-0.1.0/contourplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-17 19:08:03.614416 contourplots-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-02-17 19:07:15.000000 contourplots-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:12:36.050519 contourplots-0.2.0/
+-rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      608 2023-04-12 02:12:36.049558 contourplots-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 02:12:36.038489 contourplots-0.2.0/contourplots/
+-rw-rw-rw-   0        0        0      732 2023-04-12 02:10:36.000000 contourplots-0.2.0/contourplots/__init__.py
+-rw-rw-rw-   0        0        0    25220 2023-03-20 13:57:23.000000 contourplots-0.2.0/contourplots/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:12:36.047527 contourplots-0.2.0/contourplots.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:12:36.050519 contourplots-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-12 02:10:29.000000 contourplots-0.2.0/setup.py
```

### Comparing `contourplots-0.1.0/LICENSE.txt` & `contourplots-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contourplots-0.1.0/PKG-INFO` & `contourplots-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.1.0
+Version: 0.2.0
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.1.0/contourplots/__init__.py` & `contourplots-0.2.0/contourplots/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ContourPlots: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 # Copyright (C) 2022-2023, Sarang Bhagwat <sarang.bhagwat.git@gmail.com>
 # 
 # This module is under the MIT open-source license. See 
 # https://github.com/sarangbhagwat/contourplots/blob/main/LICENSE
 # for license details.
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 __author__ = 'Sarang S. Bhagwat'
 
 # %% Initialize ContourPlots 
 
 from . import utils
 
 animated_contourplot = utils.animated_contourplot
```

### Comparing `contourplots-0.1.0/contourplots/utils.py` & `contourplots-0.2.0/contourplots/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,25 +47,30 @@
                                   w_tick_width=0.5, # width for labeled, lined contours
                                   fmt_clabel = lambda cvalue: "{:.2f}".format(cvalue), # format of contour labels
                                   gridspec_kw={'height_ratios': [1, 20]},
                                   fontname={'fontname':'Arial'},
                                   figwidth=3.9,
                                   dpi=600,
                                   cmap='viridis',
+                                  extend_cmap='neither',
+                                  cmap_over_color=None,
                                   cbar_ticks=None,
                                   z_marker_color='b',
                                   z_marker_type='v',
                                   axis_title_fonts={'size': {'x': 12, 'y':12, 'z':12, 'w':12},},
                                   gap_between_figures=20., 
                                   clabel_fontsize = 12,
                                   fps=3, # animation frames (z values traversed) per second
                                   n_loops='inf', # the number of times the animated contourplot should loop animation over z; infinite by default
                                   animated_contourplot_filename='animated_contourplot',
                                   keep_frames=False, # leaves frame PNG files undeleted after running; False by default
                                   n_minor_ticks = 1,
+                                  cbar_n_minor_ticks = 4,
+                                  comparison_range=[],
+                                  comparison_range_hatch_pattern='///',
                                     ):
     results = np.array(w_data_vs_x_y_at_multiple_z)
     plt.rcParams['font.sans-serif'] = "Arial"
     plt.rcParams['font.size'] = "14"
     def create_frame(z_index):
         fig, axs = plt.subplots(2, 1, constrained_layout=True, 
                                 gridspec_kw=gridspec_kw)
@@ -89,50 +94,70 @@
         ax.plot(a,y,
                 color=z_marker_color, 
                 marker=z_marker_type,
                 ms = 7,)
         ax.axes.get_yaxis().set_visible(False)
         
         ax = axs[1]
+        if cmap_over_color is not None:
+            cmap.set_over(cmap_over_color)
+        
+            
         im = ax.contourf(x_data, y_data, results[z_index],
                           cmap=cmap,
                          levels=w_levels,
+                         extend=extend_cmap
+                         
                          )
         
+        
+        
+        ax.xaxis.set_minor_locator(AutoMinorLocator(n_minor_ticks+1))
+        ax.yaxis.set_minor_locator(AutoMinorLocator(n_minor_ticks+1))
         # ########--########
-        # ax.tick_params(
-        #     axis='y',          # changes apply to the x-axis
-        #     which='both',      # both major and minor ticks are affected
-        #     direction='inout',
-        #     # right=True,
-        #     width=1,
-        #     )
+        ax.tick_params(
+            axis='y',          # changes apply to the x-axis
+            which='both',      # both major and minor ticks are affected
+            direction='inout',
+            # right=True,
+            width=0.65,
+            )
 
-        # ax.tick_params(
-        #     axis='y',          
-        #     which='major',      
-        #     length=5,
-        #     )
+        ax.tick_params(
+            axis='y',          
+            which='major',      
+            length=7,
+            )
 
-        # ax.tick_params(
-        #     axis='y',          
-        #     which='minor',      
-        #     length=3,
-        #     )
-        
-        
-        # ax.tick_params(
-        #     axis='x',          # changes apply to the x-axis
-        #     which='both',      # both major and minor ticks are affected
-        #     direction='inout',
-        #     # right=True,
-        #     # top=True,
-        #     width=1,
-        #     )
-        
+        ax.tick_params(
+            axis='y',          
+            which='minor',      
+            length=3.5,
+            )
+        
+        
+        ax.tick_params(
+            axis='x',          # changes apply to the x-axis
+            which='both',      # both major and minor ticks are affected
+            direction='inout',
+            right=True,
+            top=True,
+            width=0.65,
+            )
+        ax.tick_params(
+            axis='x',          
+            which='major',      
+            length=7,
+            )
+
+        ax.tick_params(
+            axis='x',          
+            which='minor',      
+            length=3.5,
+            )
         
         # ax2 = ax.twinx()
         
         
         # if not (y_ticks==[] or x_ticks==[]):
         #     ax.set_yticks(y_ticks)
         #     ax2.set_yticks(y_ticks)
@@ -167,27 +192,53 @@
         #     # right=True,
         #     labelright=False,
         #     width=1,
         #     )
         
         # ########--########
         
-        
+        if not comparison_range==[]:
+            [m1,n1] = np.where((results[z_index] > comparison_range[0]) & (results[z_index] < comparison_range[1]))
+            # [m2,n2] = np.where(results[z_index] < 7.5)
+            
+            z1 = np.zeros(results[z_index].shape)
+            z1[m1,n1] = 99
+            
+            # print(z1,)
+            plt.rcParams['hatch.linewidth'] = 0.6
+            plt.rcParams['hatch.color'] = 'white'
+            cs = ax.contourf(x_data, y_data, z1 ,1 , hatches=['', comparison_range_hatch_pattern],  alpha=0.,
+                             # extend=extend_cmap,
+                             )
+            
         clines = ax.contour(x_data, y_data, results[z_index],
                    levels=w_ticks,
                     colors='black',
                    linewidths=w_tick_width)
         
         ax.clabel(clines, 
                    w_ticks,
                    fmt=fmt_clabel, 
                   fontsize=clabel_fontsize,
                   colors='black',
                   )
         
+        if not comparison_range==[]:
+            clines2 = ax.contour(x_data, y_data, results[z_index],
+                       levels=comparison_range,
+                        colors='white',
+                       linewidths=w_tick_width)
+            
+            ax.clabel(clines2, 
+                       comparison_range,
+                       fmt=fmt_clabel, 
+                      fontsize=clabel_fontsize,
+                      colors='black',
+                      )
+        
         ax.set_ylabel(y_label + " [" + y_units + "]",  
                       fontsize=axis_title_fonts['size']['y'],
                       **fontname)
         ax.set_xlabel(x_label + " [" + x_units + "]", 
                       fontsize=axis_title_fonts['size']['x'],
                       **fontname)
         
@@ -201,19 +252,44 @@
         
         # if not cbar_ticks:
         #     cbar_ticks = w_levels
         cbar = plt.colorbar(
                             mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
                             # im,
                             cax=cax, 
-                     ticks = cbar_ticks).set_label(label=w_label + " [" + w_units + "]", 
-                                                           size=axis_title_fonts['size']['w'],
-                                                           loc='center',
-                                                           **fontname
-                                                           )
+                     ticks = cbar_ticks)
+        
+        cbar.set_label(label=w_label + " [" + w_units + "]", 
+                                              size=axis_title_fonts['size']['w'],
+                                              loc='center',
+                                              **fontname
+                                              )
+        
+        # cbar.ax.set_minor_locator(AutoMinorLocator(cbar_n_minor_ticks+1))
+        cbar.ax.minorticks_on()
+        
+        cbar.ax.tick_params(
+            axis='y',          # changes apply to the x-axis
+            which='both',      # both major and minor ticks are affected
+            direction='inout',
+            # right=True,
+            width=0.65,
+            )
+        cbar.ax.tick_params(
+            axis='x',          
+            which='major',      
+            length=7,
+            )
+
+        cbar.ax.tick_params(
+            axis='x',          
+            which='minor',      
+            length=3.5,
+            )
+        
         ax.set_title(' ', fontsize=gap_between_figures)
 
         plt.savefig(f'./{animated_contourplot_filename}_frame_{z_index}.png', 
                     transparent = False,  
                     facecolor = 'white',
                     bbox_inches='tight',
                     dpi=dpi,
```

### Comparing `contourplots-0.1.0/contourplots.egg-info/PKG-INFO` & `contourplots-0.2.0/contourplots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.1.0
+Version: 0.2.0
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.1.0/setup.py` & `contourplots-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from setuptools import setup
 
 setup(
     name='contourplots',
     packages=['contourplots'],
-    version='0.1.0',    
+    version='0.2.0',    
     description='A toolkit for generating multi-dimensional plots easily, usefully, and legibly.',
     url='https://github.com/sarangbhagwat/contourplots',
     author='Sarang S. Bhagwat',
     author_email='sarang.bhagwat.git@gmail.com',
     license='MIT',
     # packages=['contourplots'],
     install_requires=['matplotlib==3.5.2',
```

