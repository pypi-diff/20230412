# Comparing `tmp/autoplot-0.3.9.tar.gz` & `tmp/autoplot-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoplot-0.3.9.tar", last modified: Tue Dec  3 17:57:47 2019, max compression
+gzip compressed data, was "autoplot-0.4.1.tar", last modified: Wed Apr 12 17:05:33 2023, max compression
```

## Comparing `autoplot-0.3.9.tar` & `autoplot-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2019-12-03 17:57:06.000000 autoplot-0.3.9/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      760 2019-12-02 18:15:21.000000 autoplot-0.3.9/setup.py
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)    21476 2019-12-03 17:52:16.000000 autoplot-0.3.9/autoplot/autoplot.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      278 2019-12-02 18:16:16.000000 autoplot-0.3.9/autoplot/__init__.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2019-12-03 17:57:06.000000 autoplot-0.3.9/setup.cfg
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot.egg-info/
--rw-r--r--   0 jbf       (1210) jbf       (1210)        1 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot.egg-info/dependency_links.txt
--rw-r--r--   0 jbf       (1210) jbf       (1210)       13 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot.egg-info/requires.txt
--rw-r--r--   0 jbf       (1210) jbf       (1210)      220 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot.egg-info/SOURCES.txt
--rw-r--r--   0 jbf       (1210) jbf       (1210)        9 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot.egg-info/top_level.txt
--rw-r--r--   0 jbf       (1210) jbf       (1210)     2289 2019-12-03 17:57:06.000000 autoplot-0.3.9/autoplot.egg-info/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2289 2019-12-03 17:57:06.000000 autoplot-0.3.9/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1664 2019-11-26 17:49:11.000000 autoplot-0.3.9/README.rst
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-12 17:05:33.371171 autoplot-0.4.1/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.4.1/LICENSE.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1887 2023-04-12 17:05:33.371171 autoplot-0.4.1/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1636 2023-04-12 16:42:58.000000 autoplot-0.4.1/README.rst
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-12 17:05:33.371171 autoplot-0.4.1/autoplot/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      273 2023-04-12 16:41:46.000000 autoplot-0.4.1/autoplot/__init__.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)    21685 2023-04-12 16:24:38.000000 autoplot-0.4.1/autoplot/autoplot.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-12 17:05:33.371171 autoplot-0.4.1/autoplot.egg-info/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1887 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/requires.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-12 17:05:33.000000 autoplot-0.4.1/autoplot.egg-info/top_level.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-12 17:05:33.371171 autoplot-0.4.1/setup.cfg
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-12 16:51:15.000000 autoplot-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autoplot-0.3.9/setup.py` & `autoplot-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 install_requires = ["jpype1","numpy"]
 
 if sys.argv[1] == 'develop':
     install_requires.append("pytest")
 
 setup(
     name='autoplot',
-    version='0.3.9',
+    version='0.4.1',
     author='Jeremy Faden',
     author_email='faden@cottagesystems.com',
     packages=find_packages(), 
-    url='http://pypi.python.org/pypi/autoplot',
+    url='https://github.com/autoplot/python/',
     license='LICENSE.txt',
     description='Interface to Autoplot Java library',
     long_description=open('README.rst').read(),
     install_requires=install_requires
 )
```

### Comparing `autoplot-0.3.9/autoplot/autoplot.py` & `autoplot-0.4.1/autoplot/autoplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import print_function
 
+
 def version():
-    return '0.3.9'
+    return '0.4.1'
+
 
 def printNoNewline(s):
     print(s, end=' ')
-    
+
+
 def javaaddpath(url='', jdwpPort=-1):
-    '''Start up JVM, import JAR at URL, and import the paths starting with org 
+    """Start up JVM, import JAR at URL, and import the paths starting with org
     into the Python namespace.
       com= jpype.JPackage('com') 
     can be used to the com package into the Python namespace.
     Example:
-      org = javaaddpath('http://autoplot.org/devel/autoplot.jar')
+      javaaddpath('http://autoplot.org/devel/autoplot.jar')
     if no url is provided, then the default http://autoplot.org/latest/autoplot.jar is used.
-    '''
+    """
 
     import os
     import jpype
     import tempfile
 
     # TODO: Use requests package.
     try:
@@ -78,44 +81,49 @@
 
         else:
             print('Java is starting')
             jpype.startJVM(jpype.getDefaultJVMPath(), '-Djava.class.path='+cacheFile)
     else:
         print('Java is already running.')
 
-    return jpype.JPackage("org")
+
+def APDataSet():
+    """create a new container for loading data"""
+    import jpype
+    clas = jpype.JClass("org.autoplot.idlsupport.APDataSet")
+    return clas()
 
 
 def to_ndarray(apds, name):
-    'extract the data identified by name to numpy array, using datetime64 for times.'
+    """extract the data identified by name to numpy array, using datetime64 for times."""
     import numpy as np
     import jpype
-    org = jpype.JPackage('org')
+    Units = jpype.JClass('org.das2.datum.Units')
     apds.setPreferredUnits('microseconds since 2000-01-01T00:00')
-    u = org.das2.datum.Units.lookupUnits(apds.propertyAsString(name, 'UNITS'))
-    if u.isConvertibleTo(org.das2.datum.Units.us2000):
+    u = Units.lookupUnits(apds.propertyAsString(name, 'UNITS'))
+    if u.isConvertibleTo(Units.us2000):
         g_base = np.datetime64('2000-01-01T00:00:00Z')
         dd = apds.values(name)
         result = np.array([g_base + np.timedelta64(int(dd[i]*1000), 'ns') for i in range(len(dd))])
     else:
         dd = apds.values(name)
         result = np.array(dd)
     return result
 
 
 def to_qdataset(X, Y=None, Z=None):
-    '''convert the ndarrays or array like objects to Autoplot QDataSet objects.
-    datetime64 are handled by converting to QDataSet with Units.us2000'''
+    """convert the ndarrays or array like objects to Autoplot QDataSet objects.
+    datetime64 are handled by converting to QDataSet with Units.us2000"""
     import jpype
     if not jpype.isJVMStarted():
         raise Exception('Java is not running, use javaaddpath')
-    org = jpype.JPackage('org')
-    dataset = org.das2.qds.ops.Ops.dataset
-    link = org.das2.qds.ops.Ops.link
-    transpose = org.das2.qds.ops.Ops.transpose
+    Ops = jpype.JClass('org.das2.qds.ops.Ops')
+    dataset = Ops.dataset
+    link = Ops.link
+    transpose = Ops.transpose
     import numpy as np
 
     if Y is None and Z is None:
         if isinstance(X, jpype.JavaObject):
             xds = X  # assume it's a QDataSet already
         else:
             if not hasattr(X, 'dtype'):
@@ -141,17 +149,16 @@
         zds = to_qdataset(Z)
         return link(xds, yds, zds)
 
 
 def show_completions( s ):
     'print completions for the given URI.'
     import jpype
-    org= javaaddpath()
-    sc= org.autoplot.ScriptContext
-    xxs= sc.getCompletions( s )
+    sc = jpype.JClass('org.autoplot.ScriptContext')
+    xxs = sc.getCompletions(s)
     for x in xxs:
         print(x)
     
 
 #def applot(X, Y=None, Z=None):
 #    'plot Python arrays or ndarrays in Autoplot'
 #    import jpype
@@ -159,79 +166,82 @@
 #        raise Exception('Java is not running, use javaaddpath')
 #    ds = to_qdataset(X, Y, Z)
 #    org = jpype.JPackage('org')
 #    sc = org.autoplot.ScriptContext
 #    sc.plot(ds)
 
 def das2stream( dataStruct, filename, ytags=None, ascii=1, xunits='' ):
-
+    """Write the python data structure to a das2stream"""
     print( 'writing das2stream to ' + filename + ' using ' + version() )
     import time
 
-    streamHeader= [ '[00]xxxxxx<stream source="applot.pro" localDate="'+time.asctime()+'">', '</stream>' ]
-    contentLength= -10  # don't include the packet tag and content length
+    streamHeader = ['[00]xxxxxx<stream source="applot.pro" localDate="'+time.asctime()+'">', '</stream>']
+    contentLength = -10  # don't include the packet tag and content length
     for i in range( len( streamHeader ) ):
         contentLength += len( streamHeader[i] ) + 1
 
     x= streamHeader[0]
     x= '[00]' + '%06d' % contentLength + x[10:]
-    streamHeader[0]= x
+    streamHeader[0] = x
 
     if ascii:
-         xdatatype= 'ascii24'
+        xdatatype = 'ascii24'
     else:
-         xdatatype= 'sun_real8'
+        xdatatype = 'sun_real8'
     if ascii:
-         datatype= 'ascii16'
+        datatype = 'ascii16'
     else:
-         datatype='sun_real8'
+        datatype = 'sun_real8'
 
     packetDescriptor= [ '[01]xxxxxx<packet>' ]
     tags= dataStruct['tags']
     nt= len(tags)
     packetDescriptor.append( '   <x type="'+xdatatype+'" name="'+tags[0]+'" units="'+xunits+'" />' )
 
     totalItems=1
 
-    format=['%24.12f']
-    reclen= 4 + 24 + (nt-1) * 20
-    i=0
+    format = ['%24.12f']
+    reclen = 4 + 24 + (nt-1) * 20
+    i = 0
     for tag in tags:
         d= dataStruct[tag]
         if ( i==0 ):
             name=''
             i=i+1
             continue
         else:
             name= tags[i]    ### stream reader needs a default plane
         if ( isinstance( d, list ) ):
             rank= 1
         elif ( hasattr( d, "shape") ):  # check for numpy
             rank= len(d.shape)
 
-        if ( rank==1 ):
+        if (rank==1):
             packetDescriptor.append( '   <y type="'+datatype+'" name="'+name+'" units="" idlname="'+tags[i]+'" />' )
 
-            if ( i<nt-1 ): format.append('%16.4e')
-            else: format.append( '%15.3e' )
+            if (i<nt-1):
+                format.append('%16.4e')
+            else:
+                format.append('%15.3e')
             totalItems= totalItems + 1
         else:
-            if ytags==None: ytags= range(s[2])
-            sytags= ','.join( [ "%f"%n for n in ytags ] )
-            nitems= len(ytags)
+            if ytags==None:
+                ytags= range(s[2])
+            sytags = ','.join( [ "%f"%n for n in ytags ] )
+            nitems = len(ytags)
             packetDescriptor.append( '   <yscan type="' +datatype+'" name="' +name +'" units="" nitems="'+str(nitems) +'" yTags="'+sytags+'"' +' />' )
  
             for i in range(1,nitems):
                 format.append('%16.4e')
-            if ( i<nt-1 ):
+            if (i<nt-1):
                 format.append('%16.4e')
             else:
                 format.append('%15.4e')
-            totalItems+= nitems
-        i=i+1;
+            totalItems += nitems
+        i = i+1
 
     packetDescriptor.append( '</packet>' )
 
     contentLength= -10 # don't include the packet tag and content length
     for i in range(0,len(packetDescriptor)):
         contentLength += len( packetDescriptor[i] ) + 1
   
@@ -281,15 +291,15 @@
 
         if ( newline ): unit.write( bytes('\n','utf8') )
 
     unit.close() 
 
 
 def qstream(dataStruct, filename, ytags=None, ascii=True, xunits='', delta_plus=None, delta_minus=None):
-    """for rank 2, ytags must be specified ascii, boolean, use ascii transfer types"""
+    """Write the data to a qstream.  for rank 2, ytags must be specified ASCII, boolean, use ASCII transfer types"""
     tags = dataStruct['tags']
     nt = len(tags)
     name = tags[-1]
     tname = tags[0]
 
     print('writing qstream to ' + filename + ' using ' + version() )
     import time
@@ -476,15 +486,15 @@
 
 
 def sendCommand( s, cmd ):
     s.send( bytes(cmd,'utf8') )
     print('done')
 
 def applot( x=None, y=None, z=None, z4=None, xunits='', ylabel='', tmpfile=None, noplot=0, respawn=0, delta_plus=None, delta_minus=None ):
-    '''
+    """
 NAME:
     plot
 PURPOSE:
     Plot to Autoplot instead of the direct graphics plotting, by creating a temporary file of the data and sending a plot
     command to Autoplot with the server turned on.
 ARGUMENTS:
     X,Y,Z as with plot.  If X is an integer, then it is the position in Autoplot, so that multiple plots can be sent to 
@@ -496,15 +506,15 @@
 KEYWORDS:
    tmpfile=     explicitly set the file used to move data into Autoplot.  This can also be used with /noplot
    noplot=True  just make the tmpfile, don't actually try to plot.
    xunits=      units as a string, especially like "seconds since 2010-01-01T00:00"
    ylabel=''    label is currently ignored.
    delta_plus=  array of positive lengths showing the upper limit of the 1-sigma confidence interval.
    delta_minus= array of positive lengths showing the lower limit of the 1-sigma confidence interval.
-'''
+"""
 
     port= 12345
 
     useDas2Stream=False
 
     if useDas2Stream:    
         ext='d2s'
```

### Comparing `autoplot-0.3.9/autoplot.egg-info/PKG-INFO` & `autoplot-0.4.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,46 @@
-Metadata-Version: 1.0
-Name: autoplot
-Version: 0.3.9
-Summary: Interface to Autoplot Java library
-Home-page: http://pypi.python.org/pypi/autoplot
-Author: Jeremy Faden
-Author-email: faden@cottagesystems.com
-License: LICENSE.txt
-Description: Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
-        Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
-        
-        Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
-        These URIs can be created using the Autoplot application, available at http://autoplot.org/.
-        Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-        Helper procedures from the autoplot package convert QDataSets into ndarrays.
-        
-        Autoplot/Python Interface Tools
-        -------------------------------
-        
-        Install using `pip install autoplot`
-        
-        .. code:: python
-        
-          from autoplot import *
-        
-          # Download autoplot.jar if needed and return Python bridge object
-          org = javaaddpath('http://autoplot.org/latest/autoplot.jar')
-        
-          # Create Autoplot Data Set
-          apds = org.autoplot.idlsupport.APDataSet()
-        
-          # Set URI
-          apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
-        
-          # Get the data
-          apds.doGetDataSet()
-        
-          print(apds.toString())
-          # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
-          # data: data[dep0=288] (dimensionless)
-          # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
-        
-          # Extract data values
-          vv = to_ndarray(apds, 'data')
-          tt = to_ndarray(apds, 'dep0')
-        
-          from matplotlib import pyplot as plt
-          plt.plot(tt,vv)
-          plt.show()
-        
-        Contact
-        -------------------------------
-        Jeremy Faden <faden@cottagesystems.net>
-        
-        
-Platform: UNKNOWN
+Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
+
+Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
+These URIs can be created using the Autoplot application, available at http://autoplot.org/.
+Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
+Helper procedures from the autoplot package convert QDataSets into ndarrays.
+
+Autoplot/Python Interface Tools
+-------------------------------
+
+Install using `pip install autoplot`
+
+.. code:: python
+
+  from autoplot import *
+
+  # Download autoplot.jar if needed and return Python bridge object
+  javaaddpath('http://autoplot.org/latest/autoplot.jar')
+  
+  # Create Autoplot Data Set
+  apds = APDataSet()
+
+  # Set URI
+  apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
+
+  # Get the data
+  apds.doGetDataSet()
+
+  print(apds.toString())
+  # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
+  # data: data[dep0=288] (dimensionless)
+  # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
+
+  # Extract data values
+  vv = to_ndarray(apds, 'data')
+  tt = to_ndarray(apds, 'dep0')
+
+  from matplotlib import pyplot as plt
+  plt.plot(tt,vv)
+  plt.show()
+
+Contact
+-------------------------------
+Jeremy Faden <faden@cottagesystems.com>
+
```

### Comparing `autoplot-0.3.9/PKG-INFO` & `autoplot-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: autoplot
-Version: 0.3.9
+Version: 0.4.1
 Summary: Interface to Autoplot Java library
-Home-page: http://pypi.python.org/pypi/autoplot
+Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
-Description: Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
-        Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
-        
-        Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
-        These URIs can be created using the Autoplot application, available at http://autoplot.org/.
-        Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-        Helper procedures from the autoplot package convert QDataSets into ndarrays.
-        
-        Autoplot/Python Interface Tools
-        -------------------------------
-        
-        Install using `pip install autoplot`
-        
-        .. code:: python
-        
-          from autoplot import *
-        
-          # Download autoplot.jar if needed and return Python bridge object
-          org = javaaddpath('http://autoplot.org/latest/autoplot.jar')
-        
-          # Create Autoplot Data Set
-          apds = org.autoplot.idlsupport.APDataSet()
-        
-          # Set URI
-          apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
-        
-          # Get the data
-          apds.doGetDataSet()
-        
-          print(apds.toString())
-          # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
-          # data: data[dep0=288] (dimensionless)
-          # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
-        
-          # Extract data values
-          vv = to_ndarray(apds, 'data')
-          tt = to_ndarray(apds, 'dep0')
-        
-          from matplotlib import pyplot as plt
-          plt.plot(tt,vv)
-          plt.show()
-        
-        Contact
-        -------------------------------
-        Jeremy Faden <faden@cottagesystems.net>
-        
-        
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
+
+Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
+These URIs can be created using the Autoplot application, available at http://autoplot.org/.
+Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
+Helper procedures from the autoplot package convert QDataSets into ndarrays.
+
+Autoplot/Python Interface Tools
+-------------------------------
+
+Install using `pip install autoplot`
+
+.. code:: python
+
+  from autoplot import *
+
+  # Download autoplot.jar if needed and return Python bridge object
+  javaaddpath('http://autoplot.org/latest/autoplot.jar')
+  
+  # Create Autoplot Data Set
+  apds = APDataSet()
+
+  # Set URI
+  apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
+
+  # Get the data
+  apds.doGetDataSet()
+
+  print(apds.toString())
+  # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
+  # data: data[dep0=288] (dimensionless)
+  # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
+
+  # Extract data values
+  vv = to_ndarray(apds, 'data')
+  tt = to_ndarray(apds, 'dep0')
+
+  from matplotlib import pyplot as plt
+  plt.plot(tt,vv)
+  plt.show()
+
+Contact
+-------------------------------
+Jeremy Faden <faden@cottagesystems.com>
+
```

### Comparing `autoplot-0.3.9/README.rst` & `autoplot-0.4.1/autoplot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: autoplot
+Version: 0.4.1
+Summary: Interface to Autoplot Java library
+Home-page: https://github.com/autoplot/python/
+Author: Jeremy Faden
+Author-email: faden@cottagesystems.com
+License: LICENSE.txt
+License-File: LICENSE.txt
+
 Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
 Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
 
 Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
 These URIs can be created using the Autoplot application, available at http://autoplot.org/.
 Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
 Helper procedures from the autoplot package convert QDataSets into ndarrays.
@@ -12,18 +22,18 @@
 Install using `pip install autoplot`
 
 .. code:: python
 
   from autoplot import *
 
   # Download autoplot.jar if needed and return Python bridge object
-  org = javaaddpath('http://autoplot.org/latest/autoplot.jar')
-
+  javaaddpath('http://autoplot.org/latest/autoplot.jar')
+  
   # Create Autoplot Data Set
-  apds = org.autoplot.idlsupport.APDataSet()
+  apds = APDataSet()
 
   # Set URI
   apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
 
   # Get the data
   apds.doGetDataSet()
 
@@ -38,9 +48,9 @@
 
   from matplotlib import pyplot as plt
   plt.plot(tt,vv)
   plt.show()
 
 Contact
 -------------------------------
-Jeremy Faden <faden@cottagesystems.net>
+Jeremy Faden <faden@cottagesystems.com>
```

