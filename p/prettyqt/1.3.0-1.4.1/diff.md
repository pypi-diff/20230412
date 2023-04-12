# Comparing `tmp/prettyqt-1.3.0.tar.gz` & `tmp/prettyqt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyqt-1.3.0.tar", max compression
+gzip compressed data, was "prettyqt-1.4.1.tar", max compression
```

## Comparing `prettyqt-1.3.0.tar` & `prettyqt-1.4.1.tar`

### file list

```diff
@@ -1,747 +1,749 @@
--rw-r--r--   0        0        0     1078 2023-04-11 15:34:32.144385 prettyqt-1.3.0/LICENSE
--rw-r--r--   0        0        0     2867 2023-04-11 15:34:32.144385 prettyqt-1.3.0/docs/index.md
--rw-r--r--   0        0        0      687 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/__init__.py
--rw-r--r--   0        0        0      122 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      860 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/__pyinstaller/hook-prettyqt.py
--rw-r--r--   0        0        0      517 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/bluetooth/__init__.py
--rw-r--r--   0        0        0      334 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/bluetooth/bluetoothaddress.py
--rw-r--r--   0        0        0     2635 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py
--rw-r--r--   0        0        0     1421 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py
--rw-r--r--   0        0        0     1872 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/bluetooth/bluetoothserviceinfo.py
--rw-r--r--   0        0        0    11927 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/bluetooth/bluetoothuuid.py
--rw-r--r--   0        0        0     1792 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/abstractaxis.py
--rw-r--r--   0        0        0     1603 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/abstractbarseries.py
--rw-r--r--   0        0        0      554 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/abstractseries.py
--rw-r--r--   0        0        0      517 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/barcategoryaxis.py
--rw-r--r--   0        0        0      177 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/barseries.py
--rw-r--r--   0        0        0      932 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/barset.py
--rw-r--r--   0        0        0     1648 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/boxset.py
--rw-r--r--   0        0        0      609 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/candlestickset.py
--rw-r--r--   0        0        0     1767 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/categoryaxis.py
--rw-r--r--   0        0        0     5315 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/chart.py
--rw-r--r--   0        0        0     5665 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/chartview.py
--rw-r--r--   0        0        0      381 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/datetimeaxis.py
--rw-r--r--   0        0        0      197 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/horizontalbarseries.py
--rw-r--r--   0        0        0      217 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/horizontalpercentbarseries.py
--rw-r--r--   0        0        0      217 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/horizontalstackedbarseries.py
--rw-r--r--   0        0        0     2742 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/legend.py
--rw-r--r--   0        0        0      673 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/lineseries.py
--rw-r--r--   0        0        0      178 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/logvalueaxis.py
--rw-r--r--   0        0        0      191 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/percentbarseries.py
--rw-r--r--   0        0        0     2038 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/pieslice.py
--rw-r--r--   0        0        0      739 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/polarchart.py
--rw-r--r--   0        0        0      176 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/scatterseries.py
--rw-r--r--   0        0        0      191 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/stackedbarseries.py
--rw-r--r--   0        0        0     1044 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/valueaxis.py
--rw-r--r--   0        0        0     1219 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/charts/xyseries.py
--rw-r--r--   0        0        0    35081 2023-04-11 15:34:32.144385 prettyqt-1.3.0/prettyqt/constants/__init__.py
--rw-r--r--   0        0        0     8646 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/_calendar.py
--rw-r--r--   0        0        0     2000 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/_datetime.py
--rw-r--r--   0        0        0    16492 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/_locale.py
--rw-r--r--   0        0        0      478 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/_time.py
--rw-r--r--   0        0        0     3286 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstractanimation.py
--rw-r--r--   0        0        0      186 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstracteventdispatcher.py
--rw-r--r--   0        0        0     5236 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstractitemmodel.py
--rw-r--r--   0        0        0      250 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstractlistmodel.py
--rw-r--r--   0        0        0      146 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstractnativeeventfilter.py
--rw-r--r--   0        0        0      254 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstractproxymodel.py
--rw-r--r--   0        0        0      254 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/abstracttablemodel.py
--rw-r--r--   0        0        0     2060 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/animationgroup.py
--rw-r--r--   0        0        0      533 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/basictimer.py
--rw-r--r--   0        0        0      154 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/buffer.py
--rw-r--r--   0        0        0      173 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/bytearray.py
--rw-r--r--   0        0        0      369 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/bytearraymatcher.py
--rw-r--r--   0        0        0      959 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/collator.py
--rw-r--r--   0        0        0      126 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/collatorsortkey.py
--rw-r--r--   0        0        0      324 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/commandlineoption.py
--rw-r--r--   0        0        0     2231 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/commandlineparser.py
--rw-r--r--   0        0        0      211 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/concatenatetablesproxymodel.py
--rw-r--r--   0        0        0     3729 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/coreapplication.py
--rw-r--r--   0        0        0     2038 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/cryptographichash.py
--rw-r--r--   0        0        0     3426 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/datastream.py
--rw-r--r--   0        0        0      470 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/date.py
--rw-r--r--   0        0        0      766 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/deadlinetimer.py
--rw-r--r--   0        0        0     1153 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/debug.py
--rw-r--r--   0        0        0     4467 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/dir.py
--rw-r--r--   0        0        0      264 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/diriterator.py
--rw-r--r--   0        0        0     4527 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/easingcurve.py
--rw-r--r--   0        0        0      918 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/elapsedtimer.py
--rw-r--r--   0        0        0     7128 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/event.py
--rw-r--r--   0        0        0     1225 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/eventloop.py
--rw-r--r--   0        0        0      191 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/file.py
--rw-r--r--   0        0        0     3694 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/filedevice.py
--rw-r--r--   0        0        0     1492 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/fileinfo.py
--rw-r--r--   0        0        0      560 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/fileselector.py
--rw-r--r--   0        0        0      879 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/filesystemwatcher.py
--rw-r--r--   0        0        0      188 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/identityproxymodel.py
--rw-r--r--   0        0        0     1379 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/iodevice.py
--rw-r--r--   0        0        0      122 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/itemselection.py
--rw-r--r--   0        0        0      176 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/itemselectionmodel.py
--rw-r--r--   0        0        0      696 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/itemselectionrange.py
--rw-r--r--   0        0        0     1677 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/jsondocument.py
--rw-r--r--   0        0        0      538 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/jsonvalue.py
--rw-r--r--   0        0        0     1248 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/library.py
--rw-r--r--   0        0        0     1585 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/libraryinfo.py
--rw-r--r--   0        0        0     1868 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/line.py
--rw-r--r--   0        0        0     1997 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/linef.py
--rw-r--r--   0        0        0      810 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/lockfile.py
--rw-r--r--   0        0        0      708 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/margins.py
--rw-r--r--   0        0        0      713 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/marginsf.py
--rw-r--r--   0        0        0     1110 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/metaenum.py
--rw-r--r--   0        0        0     1423 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/metamethod.py
--rw-r--r--   0        0        0     3903 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/metaobject.py
--rw-r--r--   0        0        0      511 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/metaproperty.py
--rw-r--r--   0        0        0     5404 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/metatype.py
--rw-r--r--   0        0        0     1802 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/mimedata.py
--rw-r--r--   0        0        0      948 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/mimedatabase.py
--rw-r--r--   0        0        0      208 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/mimetype.py
--rw-r--r--   0        0        0      176 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/modelindex.py
--rw-r--r--   0        0        0      336 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/mutex.py
--rw-r--r--   0        0        0     3583 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/object.py
--rw-r--r--   0        0        0     2562 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/operatingsystemversion.py
--rw-r--r--   0        0        0      356 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/parallelanimationgroup.py
--rw-r--r--   0        0        0      253 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/pauseanimation.py
--rw-r--r--   0        0        0      338 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/persistentmodelindex.py
--rw-r--r--   0        0        0      811 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/pluginloader.py
--rw-r--r--   0        0        0      349 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/point.py
--rw-r--r--   0        0        0      353 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/pointf.py
--rw-r--r--   0        0        0     4839 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/process.py
--rw-r--r--   0        0        0     1340 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/processenvironment.py
--rw-r--r--   0        0        0      774 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/propertyanimation.py
--rw-r--r--   0        0        0      126 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/randomgenerator.py
--rw-r--r--   0        0        0      231 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/randomgenerator64.py
--rw-r--r--   0        0        0      878 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/rect.py
--rw-r--r--   0        0        0      442 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/rectf.py
--rw-r--r--   0        0        0     6495 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/regularexpression.py
--rw-r--r--   0        0        0     2579 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/regularexpressionmatch.py
--rw-r--r--   0        0        0      613 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/regularexpressionmatchiterator.py
--rw-r--r--   0        0        0     1702 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/resource.py
--rw-r--r--   0        0        0      112 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/runnable.py
--rw-r--r--   0        0        0      160 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/savefile.py
--rw-r--r--   0        0        0      281 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/semaphore.py
--rw-r--r--   0        0        0      202 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/sequentialanimationgroup.py
--rw-r--r--   0        0        0     6990 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/settings.py
--rw-r--r--   0        0        0      122 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/signalblocker.py
--rw-r--r--   0        0        0      451 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/signalmapper.py
--rw-r--r--   0        0        0     1124 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/size.py
--rw-r--r--   0        0        0     1142 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/sizef.py
--rw-r--r--   0        0        0      471 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/slot.py
--rw-r--r--   0        0        0      930 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/socketnotifier.py
--rw-r--r--   0        0        0     2681 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/sortfilterproxymodel.py
--rw-r--r--   0        0        0     2622 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/standardpaths.py
--rw-r--r--   0        0        0     1184 2023-04-11 15:34:32.148385 prettyqt-1.3.0/prettyqt/core/storageinfo.py
--rw-r--r--   0        0        0      339 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/stringlistmodel.py
--rw-r--r--   0        0        0      980 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/temporarydir.py
--rw-r--r--   0        0        0      164 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/temporaryfile.py
--rw-r--r--   0        0        0     2583 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/textboundaryfinder.py
--rw-r--r--   0        0        0     3862 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/textstream.py
--rw-r--r--   0        0        0      108 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/thread.py
--rw-r--r--   0        0        0      160 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/threadpool.py
--rw-r--r--   0        0        0     2318 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/timeline.py
--rw-r--r--   0        0        0     1770 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/timer.py
--rw-r--r--   0        0        0     2076 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/timezone.py
--rw-r--r--   0        0        0     1722 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/translator.py
--rw-r--r--   0        0        0      190 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/transposeproxymodel.py
--rw-r--r--   0        0        0     3968 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/url.py
--rw-r--r--   0        0        0      770 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/urlquery.py
--rw-r--r--   0        0        0     1837 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/uuid.py
--rw-r--r--   0        0        0     1501 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/variantanimation.py
--rw-r--r--   0        0        0     2614 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/versionnumber.py
--rw-r--r--   0        0        0     2614 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/core/xmlstreamreader.py
--rw-r--r--   0        0        0      253 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_animations/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_animations/bounceanimation.py
--rw-r--r--   0        0        0      644 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_animations/fadeinanimation.py
--rw-r--r--   0        0        0      978 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_animations/slideanimation.py
--rw-r--r--   0        0        0      535 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/__init__.py
--rw-r--r--   0        0        0      887 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/buttondelegate.py
--rw-r--r--   0        0        0     1001 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/checkboxdelegate.py
--rw-r--r--   0        0        0     2570 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/icondelegate.py
--rw-r--r--   0        0        0      596 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/nofocusdelegate.py
--rw-r--r--   0        0        0     1474 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/progressbardelegate.py
--rw-r--r--   0        0        0     4789 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/radiodelegate.py
--rw-r--r--   0        0        0     2574 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/renderlinkdelegate.py
--rw-r--r--   0        0        0     6634 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_delegates/stardelegate.py
--rw-r--r--   0        0        0      735 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/__init__.py
--rw-r--r--   0        0        0     5965 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/columnitemmodel.py
--rw-r--r--   0        0        0     3297 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/importlibdistributionmodel.py
--rw-r--r--   0        0        0     4313 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/jsonmodel.py
--rw-r--r--   0        0        0     3083 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/listmixin.py
--rw-r--r--   0        0        0     2562 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/modelmixin.py
--rw-r--r--   0        0        0     2298 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/nesteditem.py
--rw-r--r--   0        0        0     2177 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/nestedmodel.py
--rw-r--r--   0        0        0     2102 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/regexmatchesmodel.py
--rw-r--r--   0        0        0     1698 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/selectionmixin.py
--rw-r--r--   0        0        0     5288 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/storageinfomodel.py
--rw-r--r--   0        0        0     2858 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py
--rw-r--r--   0        0        0      635 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/__init__.py
--rw-r--r--   0        0        0     2060 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/compositevalidator.py
--rw-r--r--   0        0        0     1114 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/integervalidator.py
--rw-r--r--   0        0        0      704 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/notemptyvalidator.py
--rw-r--r--   0        0        0      700 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/notzerovalidator.py
--rw-r--r--   0        0        0      620 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/pathvalidator.py
--rw-r--r--   0        0        0     1554 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/regexpatternvalidator.py
--rw-r--r--   0        0        0     3143 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_validators/regexvalidators.py
--rw-r--r--   0        0        0     2704 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/__init__.py
--rw-r--r--   0        0        0     1638 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/booldicttoolbutton.py
--rw-r--r--   0        0        0     7718 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/borderlayout.py
--rw-r--r--   0        0        0     3046 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/codeeditor.py
--rw-r--r--   0        0        0     2588 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/collapsibleframe.py
--rw-r--r--   0        0        0     2468 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/colorchooserbutton.py
--rw-r--r--   0        0        0     7480 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/completionwidget.py
--rw-r--r--   0        0        0    17651 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/dataset.py
--rw-r--r--   0        0        0     2219 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/elidedlabel.py
--rw-r--r--   0        0        0     3429 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/expandableline.py
--rw-r--r--   0        0        0     3194 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/filechooserbutton.py
--rw-r--r--   0        0        0     2155 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/flagselectionwidget.py
--rw-r--r--   0        0        0     3847 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/flowlayout.py
--rw-r--r--   0        0        0     2156 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/fontchooserbutton.py
--rw-r--r--   0        0        0     9381 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/framelesswindow.py
--rw-r--r--   0        0        0     5371 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/iconbrowser.py
--rw-r--r--   0        0        0     1311 2023-04-11 15:34:32.152385 prettyqt-1.3.0/prettyqt/custom_widgets/iconlabel.py
--rw-r--r--   0        0        0     1661 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/iconwidget.py
--rw-r--r--   0        0        0     1292 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/image.py
--rw-r--r--   0        0        0      644 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/imageviewer.py
--rw-r--r--   0        0        0     1931 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/inputandslider.py
--rw-r--r--   0        0        0     2106 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/joystickbutton.py
--rw-r--r--   0        0        0     4165 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/labeledslider.py
--rw-r--r--   0        0        0     1214 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/listinput.py
--rw-r--r--   0        0        0     8209 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/logtextedit.py
--rw-r--r--   0        0        0      738 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/mappedcheckbox.py
--rw-r--r--   0        0        0     2388 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/markdownwidget.py
--rw-r--r--   0        0        0     6576 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/menurecentfiles.py
--rw-r--r--   0        0        0    18898 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/notification.py
--rw-r--r--   0        0        0     1038 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/optionalwidget.py
--rw-r--r--   0        0        0     1332 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/popupinfo.py
--rw-r--r--   0        0        0      145 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/__init__.py
--rw-r--r--   0        0        0      431 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/__main__.py
--rw-r--r--   0        0        0     1039 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/quick_ref.py
--rw-r--r--   0        0        0    19388 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/ref.html
--rw-r--r--   0        0        0     6186 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py
--rw-r--r--   0        0        0     3110 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/regexinput.py
--rw-r--r--   0        0        0    10698 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/roundprogressbar.py
--rw-r--r--   0        0        0     4284 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/selectionwidget.py
--rw-r--r--   0        0        0     6345 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/sidebarwidget.py
--rw-r--r--   0        0        0     1036 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/singlelinetextedit.py
--rw-r--r--   0        0        0    18739 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/spanslider.py
--rw-r--r--   0        0        0     1286 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/standardiconswidget.py
--rw-r--r--   0        0        0     2289 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/stringornumberwidget.py
--rw-r--r--   0        0        0     1774 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/subsequencecompleter.py
--rw-r--r--   0        0        0     8034 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/timeline.py
--rw-r--r--   0        0        0     9009 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/custom_widgets/waitingspinner.py
--rw-r--r--   0        0        0      255 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/eventfilters/__init__.py
--rw-r--r--   0        0        0     2613 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/eventfilters/animatedtooltipeventfilter.py
--rw-r--r--   0        0        0      751 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/eventfilters/hovericoneventfilter.py
--rw-r--r--   0        0        0     7915 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/__init__.py
--rw-r--r--   0        0        0     1051 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/abstractfileiconprovider.py
--rw-r--r--   0        0        0     1269 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/abstracttextdocumentlayout.py
--rw-r--r--   0        0        0      235 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/bitmap.py
--rw-r--r--   0        0        0     1451 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/brush.py
--rw-r--r--   0        0        0     2490 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/clipboard.py
--rw-r--r--   0        0        0     6808 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/color.py
--rw-r--r--   0        0        0     3045 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/colorspace.py
--rw-r--r--   0        0        0      485 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/conicalgradient.py
--rw-r--r--   0        0        0     1255 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/cursor.py
--rw-r--r--   0        0        0      439 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/desktopservices.py
--rw-r--r--   0        0        0     1094 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/doublevalidator.py
--rw-r--r--   0        0        0      973 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/drag.py
--rw-r--r--   0        0        0     9049 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/font.py
--rw-r--r--   0        0        0     4694 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/fontdatabase.py
--rw-r--r--   0        0        0      243 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/fontinfo.py
--rw-r--r--   0        0        0      889 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/fontmetrics.py
--rw-r--r--   0        0        0      719 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/fontmetricsf.py
--rw-r--r--   0        0        0     5331 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/gradient.py
--rw-r--r--   0        0        0     5027 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/guiapplication.py
--rw-r--r--   0        0        0     3986 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/icon.py
--rw-r--r--   0        0        0     4053 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/iconengine.py
--rw-r--r--   0        0        0     1630 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/image.py
--rw-r--r--   0        0        0     3778 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/imageiohandler.py
--rw-r--r--   0        0        0     3838 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/imagereader.py
--rw-r--r--   0        0        0     2791 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/imagewriter.py
--rw-r--r--   0        0        0     1315 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/inputmethod.py
--rw-r--r--   0        0        0      921 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/intvalidator.py
--rw-r--r--   0        0        0     6154 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/keysequence.py
--rw-r--r--   0        0        0      636 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/lineargradient.py
--rw-r--r--   0        0        0      302 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/matrix4x4.py
--rw-r--r--   0        0        0     1969 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/movie.py
--rw-r--r--   0        0        0      297 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/pagedpaintdevice.py
--rw-r--r--   0        0        0     2923 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/pagelayout.py
--rw-r--r--   0        0        0     7804 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/pagesize.py
--rw-r--r--   0        0        0     1676 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/paintdevice.py
--rw-r--r--   0        0        0      319 2023-04-11 15:34:32.156385 prettyqt-1.3.0/prettyqt/gui/paintdevicewindow.py
--rw-r--r--   0        0        0     7794 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/painter.py
--rw-r--r--   0        0        0     2425 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/painterpath.py
--rw-r--r--   0        0        0     1641 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/painterpathstroker.py
--rw-r--r--   0        0        0     5907 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/palette.py
--rw-r--r--   0        0        0     1026 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/pdfwriter.py
--rw-r--r--   0        0        0     2841 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/pen.py
--rw-r--r--   0        0        0      471 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/picture.py
--rw-r--r--   0        0        0     4827 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/pixmap.py
--rw-r--r--   0        0        0      796 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/pixmapcache.py
--rw-r--r--   0        0        0     3489 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/polygon.py
--rw-r--r--   0        0        0     4325 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/polygonf.py
--rw-r--r--   0        0        0      898 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/radialgradient.py
--rw-r--r--   0        0        0      220 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/rasterwindow.py
--rw-r--r--   0        0        0     1145 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/region.py
--rw-r--r--   0        0        0     1290 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/regularexpressionvalidator.py
--rw-r--r--   0        0        0     2963 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/screen.py
--rw-r--r--   0        0        0     1291 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/sessionmanager.py
--rw-r--r--   0        0        0     6203 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/standarditem.py
--rw-r--r--   0        0        0     4778 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/standarditemmodel.py
--rw-r--r--   0        0        0     2225 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/statictext.py
--rw-r--r--   0        0        0     1146 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/stylehints.py
--rw-r--r--   0        0        0     1303 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/surface.py
--rw-r--r--   0        0        0     1352 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/syntaxhighlighter.py
--rw-r--r--   0        0        0     5251 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textblock.py
--rw-r--r--   0        0        0      623 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textblockgroup.py
--rw-r--r--   0        0        0      536 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textblockuserdata.py
--rw-r--r--   0        0        0     4878 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textcharformat.py
--rw-r--r--   0        0        0     5551 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textcursor.py
--rw-r--r--   0        0        0     7781 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textdocument.py
--rw-r--r--   0        0        0      949 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textdocumentfragment.py
--rw-r--r--   0        0        0     1062 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textdocumentwriter.py
--rw-r--r--   0        0        0     3262 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textformat.py
--rw-r--r--   0        0        0      534 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textframe.py
--rw-r--r--   0        0        0     3627 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textframeformat.py
--rw-r--r--   0        0        0      297 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textimageformat.py
--rw-r--r--   0        0        0      517 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textlayout.py
--rw-r--r--   0        0        0      725 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textlength.py
--rw-r--r--   0        0        0     1649 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textline.py
--rw-r--r--   0        0        0     1327 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textlistformat.py
--rw-r--r--   0        0        0      445 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textobject.py
--rw-r--r--   0        0        0      199 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textobjectinterface.py
--rw-r--r--   0        0        0     1560 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/textoption.py
--rw-r--r--   0        0        0     4104 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/texttablecellformat.py
--rw-r--r--   0        0        0     2659 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/transform.py
--rw-r--r--   0        0        0      640 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/undocommand.py
--rw-r--r--   0        0        0      356 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/undogroup.py
--rw-r--r--   0        0        0      957 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/undostack.py
--rw-r--r--   0        0        0      755 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/validator.py
--rw-r--r--   0        0        0      575 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/vector3d.py
--rw-r--r--   0        0        0      578 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/vector4d.py
--rw-r--r--   0        0        0     2338 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/gui/window.py
--rw-r--r--   0        0        0    10227 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/animation.py
--rw-r--r--   0        0        0     3079 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/awesomefileiconprovider.py
--rw-r--r--   0        0        0      539 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/awesomequickimageprovider.py
--rw-r--r--   0        0        0      832 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/chariconengine.py
--rw-r--r--   0        0        0    10996 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/codicon-charmap.json
--rw-r--r--   0        0        0    68076 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/codicon.ttf
--rw-r--r--   0        0        0     7924 2023-04-11 15:34:32.160385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json
--rw-r--r--   0        0        0    79556 2023-04-11 15:34:32.164385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf
--rw-r--r--   0        0        0    11206 2023-04-11 15:34:32.164385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json
--rw-r--r--   0        0        0   134316 2023-04-11 15:34:32.164385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf
--rw-r--r--   0        0        0     3947 2023-04-11 15:34:32.164385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json
--rw-r--r--   0        0        0    33692 2023-04-11 15:34:32.164385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf
--rw-r--r--   0        0        0    25663 2023-04-11 15:34:32.164385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json
--rw-r--r--   0        0        0   203644 2023-04-11 15:34:32.168385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf
--rw-r--r--   0        0        0   200215 2023-04-11 15:34:32.168385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json
--rw-r--r--   0        0        0  1026284 2023-04-11 15:34:32.180385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf
--rw-r--r--   0        0        0   216192 2023-04-11 15:34:32.180385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json
--rw-r--r--   0        0        0  1108672 2023-04-11 15:34:32.180385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf
--rw-r--r--   0        0        0   151941 2023-04-11 15:34:32.180385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/phosphor-charmap.json
--rw-r--r--   0        0        0  1392088 2023-04-11 15:34:32.192385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/phosphor.ttf
--rw-r--r--   0        0        0    72655 2023-04-11 15:34:32.192385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/remixicon-charmap.json
--rw-r--r--   0        0        0   403056 2023-04-11 15:34:32.196385 prettyqt-1.3.0/prettyqt/iconprovider/fonts/remixicon.ttf
--rw-r--r--   0        0        0     8417 2023-04-11 15:34:32.196385 prettyqt-1.3.0/prettyqt/iconprovider/iconic_font.py
--rw-r--r--   0        0        0     2468 2023-04-11 15:34:32.196385 prettyqt-1.3.0/prettyqt/iconprovider/svgbuffericonengine.py
--rw-r--r--   0        0        0   154232 2023-04-11 15:34:32.196385 prettyqt-1.3.0/prettyqt/localization/language_ar.qm
--rw-r--r--   0        0        0   155315 2023-04-11 15:34:32.200385 prettyqt-1.3.0/prettyqt/localization/language_bg.qm
--rw-r--r--   0        0        0   178552 2023-04-11 15:34:32.200385 prettyqt-1.3.0/prettyqt/localization/language_ca.qm
--rw-r--r--   0        0        0   151054 2023-04-11 15:34:32.200385 prettyqt-1.3.0/prettyqt/localization/language_cs.qm
--rw-r--r--   0        0        0   179910 2023-04-11 15:34:32.200385 prettyqt-1.3.0/prettyqt/localization/language_da.qm
--rw-r--r--   0        0        0   212675 2023-04-11 15:34:32.204385 prettyqt-1.3.0/prettyqt/localization/language_de.qm
--rw-r--r--   0        0        0   154543 2023-04-11 15:34:32.204385 prettyqt-1.3.0/prettyqt/localization/language_es.qm
--rw-r--r--   0        0        0    97872 2023-04-11 15:34:32.204385 prettyqt-1.3.0/prettyqt/localization/language_fa.qm
--rw-r--r--   0        0        0   174500 2023-04-11 15:34:32.204385 prettyqt-1.3.0/prettyqt/localization/language_fi.qm
--rw-r--r--   0        0        0   154190 2023-04-11 15:34:32.208385 prettyqt-1.3.0/prettyqt/localization/language_fr.qm
--rw-r--r--   0        0        0   183091 2023-04-11 15:34:32.208385 prettyqt-1.3.0/prettyqt/localization/language_gd.qm
--rw-r--r--   0        0        0   108600 2023-04-11 15:34:32.208385 prettyqt-1.3.0/prettyqt/localization/language_gl.qm
--rw-r--r--   0        0        0   130568 2023-04-11 15:34:32.208385 prettyqt-1.3.0/prettyqt/localization/language_he.qm
--rw-r--r--   0        0        0   150033 2023-04-11 15:34:32.212385 prettyqt-1.3.0/prettyqt/localization/language_hu.qm
--rw-r--r--   0        0        0   153570 2023-04-11 15:34:32.212385 prettyqt-1.3.0/prettyqt/localization/language_it.qm
--rw-r--r--   0        0        0   122385 2023-04-11 15:34:32.212385 prettyqt-1.3.0/prettyqt/localization/language_ja.qm
--rw-r--r--   0        0        0   120318 2023-04-11 15:34:32.212385 prettyqt-1.3.0/prettyqt/localization/language_ko.qm
--rw-r--r--   0        0        0    90502 2023-04-11 15:34:32.212385 prettyqt-1.3.0/prettyqt/localization/language_lt.qm
--rw-r--r--   0        0        0   143558 2023-04-11 15:34:32.216385 prettyqt-1.3.0/prettyqt/localization/language_lv.qm
--rw-r--r--   0        0        0   161318 2023-04-11 15:34:32.216385 prettyqt-1.3.0/prettyqt/localization/language_pl.qm
--rw-r--r--   0        0        0    50541 2023-04-11 15:34:32.216385 prettyqt-1.3.0/prettyqt/localization/language_pt.qm
--rw-r--r--   0        0        0   197476 2023-04-11 15:34:32.216385 prettyqt-1.3.0/prettyqt/localization/language_ru.qm
--rw-r--r--   0        0        0   115250 2023-04-11 15:34:32.216385 prettyqt-1.3.0/prettyqt/localization/language_sk.qm
--rw-r--r--   0        0        0    96357 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/localization/language_sl.qm
--rw-r--r--   0        0        0    47206 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/localization/language_sv.qm
--rw-r--r--   0        0        0   148437 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/localization/language_uk.qm
--rw-r--r--   0        0        0    61089 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/localization/language_zh_CN.qm
--rw-r--r--   0        0        0   125250 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/localization/language_zh_TW.qm
--rw-r--r--   0        0        0     2384 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/__init__.py
--rw-r--r--   0        0        0      387 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/geocodingmanager.py
--rw-r--r--   0        0        0     2867 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/geomaneuver.py
--rw-r--r--   0        0        0     1055 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/georoute.py
--rw-r--r--   0        0        0     5266 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/georouterequest.py
--rw-r--r--   0        0        0      657 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/georoutesegment.py
--rw-r--r--   0        0        0     2021 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/georoutingmanager.py
--rw-r--r--   0        0        0     5880 2023-04-11 15:34:32.220385 prettyqt-1.3.0/prettyqt/location/geoserviceprovider.py
--rw-r--r--   0        0        0     2387 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/place.py
--rw-r--r--   0        0        0      864 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeattribute.py
--rw-r--r--   0        0        0      737 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placecategory.py
--rw-r--r--   0        0        0      844 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placecontactdetail.py
--rw-r--r--   0        0        0     1030 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placecontent.py
--rw-r--r--   0        0        0     1275 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placecontentreply.py
--rw-r--r--   0        0        0      947 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placecontentrequest.py
--rw-r--r--   0        0        0      562 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placedetailsreply.py
--rw-r--r--   0        0        0      849 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeicon.py
--rw-r--r--   0        0        0     1185 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeidreply.py
--rw-r--r--   0        0        0     2233 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placemanager.py
--rw-r--r--   0        0        0     1066 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placematchreply.py
--rw-r--r--   0        0        0      726 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placematchrequest.py
--rw-r--r--   0        0        0      223 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeproposedsearchresult.py
--rw-r--r--   0        0        0      316 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeratings.py
--rw-r--r--   0        0        0     1923 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placereply.py
--rw-r--r--   0        0        0      267 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeresult.py
--rw-r--r--   0        0        0     1651 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placesearchreply.py
--rw-r--r--   0        0        0     2230 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placesearchrequest.py
--rw-r--r--   0        0        0      884 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placesearchresult.py
--rw-r--r--   0        0        0      675 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placesupplier.py
--rw-r--r--   0        0        0      215 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/placeuser.py
--rw-r--r--   0        0        0      621 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/location/qlocation.py
--rw-r--r--   0        0        0      167 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/multimediawidgets/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/multimediawidgets/graphicsvideoitem.py
--rw-r--r--   0        0        0      872 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/multimediawidgets/videowidget.py
--rw-r--r--   0        0        0     1172 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/__init__.py
--rw-r--r--   0        0        0     8113 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/abstractsocket.py
--rw-r--r--   0        0        0     1775 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/hostaddress.py
--rw-r--r--   0        0        0     1465 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/httpmultipart.py
--rw-r--r--   0        0        0      823 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/httppart.py
--rw-r--r--   0        0        0     1310 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/localserver.py
--rw-r--r--   0        0        0     2392 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/localsocket.py
--rw-r--r--   0        0        0     2313 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkaccessmanager.py
--rw-r--r--   0        0        0     2000 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkaddressentry.py
--rw-r--r--   0        0        0     1551 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkcookie.py
--rw-r--r--   0        0        0      850 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkcookiejar.py
--rw-r--r--   0        0        0      627 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkdatagram.py
--rw-r--r--   0        0        0     3011 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkinterface.py
--rw-r--r--   0        0        0     3361 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkproxy.py
--rw-r--r--   0        0        0     6462 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/networkrequest.py
--rw-r--r--   0        0        0      779 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/tcpserver.py
--rw-r--r--   0        0        0      178 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/tcpsocket.py
--rw-r--r--   0        0        0      671 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/network/udpsocket.py
--rw-r--r--   0        0        0       26 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/objbrowser/__init__.py
--rw-r--r--   0        0        0     9193 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/objbrowser/attribute_model.py
--rw-r--r--   0        0        0    14897 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/objbrowser/objectbrowser.py
--rw-r--r--   0        0        0    18583 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/objbrowser/objectbrowsertreemodel.py
--rw-r--r--   0        0        0      356 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/paths.py
--rw-r--r--   0        0        0     1169 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/__init__.py
--rw-r--r--   0        0        0      171 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geoaddress.py
--rw-r--r--   0        0        0     1149 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geoareamonitorinfo.py
--rw-r--r--   0        0        0     1260 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geoareamonitorsource.py
--rw-r--r--   0        0        0     1072 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geocircle.py
--rw-r--r--   0        0        0     1172 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geocoordinate.py
--rw-r--r--   0        0        0      558 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geolocation.py
--rw-r--r--   0        0        0     1021 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geopath.py
--rw-r--r--   0        0        0     1145 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geopolygon.py
--rw-r--r--   0        0        0     1687 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geopositioninfo.py
--rw-r--r--   0        0        0     2960 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geopositioninfosource.py
--rw-r--r--   0        0        0      769 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/georectangle.py
--rw-r--r--   0        0        0     1861 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geosatelliteinfo.py
--rw-r--r--   0        0        0     1110 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geosatelliteinfosource.py
--rw-r--r--   0        0        0      755 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/geoshape.py
--rw-r--r--   0        0        0     1196 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/positioning/nmeapositioninginfosource.py
--rw-r--r--   0        0        0        0 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/py.typed
--rw-r--r--   0        0        0      943 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/jsengine.py
--rw-r--r--   0        0        0     2397 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/jsvalue.py
--rw-r--r--   0        0        0      295 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/jsvalueiterator.py
--rw-r--r--   0        0        0      955 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/qmlapplicationengine.py
--rw-r--r--   0        0        0      907 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/qmlcomponent.py
--rw-r--r--   0        0        0     2020 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/qmlengine.py
--rw-r--r--   0        0        0      536 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/qmlimageproviderbase.py
--rw-r--r--   0        0        0      185 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qml/qmlparserstatus.py
--rw-r--r--   0        0        0      203 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/Qsci/__init__.py
--rw-r--r--   0        0        0      213 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtBluetooth/__init__.py
--rw-r--r--   0        0        0      446 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtCharts/__init__.py
--rw-r--r--   0        0        0     2281 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtCore/__init__.py
--rw-r--r--   0        0        0      690 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtGui/__init__.py
--rw-r--r--   0        0        0      253 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtHelp/__init__.py
--rw-r--r--   0        0        0      281 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtLocation/__init__.py
--rw-r--r--   0        0        0      271 2023-04-11 15:34:32.224385 prettyqt-1.3.0/prettyqt/qt/QtMultimedia/__init__.py
--rw-r--r--   0        0        0      292 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtMultimediaWidgets/__init__.py
--rw-r--r--   0        0        0      278 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtNetwork/__init__.py
--rw-r--r--   0        0        0      274 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtPositioning/__init__.py
--rw-r--r--   0        0        0      266 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtQml/__init__.py
--rw-r--r--   0        0        0      272 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtQuick/__init__.py
--rw-r--r--   0        0        0      256 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtScxml/__init__.py
--rw-r--r--   0        0        0      274 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtStateMachine/__init__.py
--rw-r--r--   0        0        0      332 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtSvg/__init__.py
--rw-r--r--   0        0        0      269 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtTest/__init__.py
--rw-r--r--   0        0        0      277 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtTextToSpeech/__init__.py
--rw-r--r--   0        0        0      368 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtUiTools/__init__.py
--rw-r--r--   0        0        0      274 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtWebChannel/__init__.py
--rw-r--r--   0        0        0      280 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtWebEngineCore/__init__.py
--rw-r--r--   0        0        0      289 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtWebEngineWidgets/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/QtWidgets/__init__.py
--rw-r--r--   0        0        0     1200 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qt/__init__.py
--rw-r--r--   0        0        0      969 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/__init__.py
--rw-r--r--   0        0        0      271 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpcontentitem.py
--rw-r--r--   0        0        0      183 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpcontentmodel.py
--rw-r--r--   0        0        0      460 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpcontentwidget.py
--rw-r--r--   0        0        0      260 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpengine.py
--rw-r--r--   0        0        0      978 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpenginecore.py
--rw-r--r--   0        0        0      302 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpfilterengine.py
--rw-r--r--   0        0        0      177 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpindexmodel.py
--rw-r--r--   0        0        0      178 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpindexwidget.py
--rw-r--r--   0        0        0      442 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpsearchengine.py
--rw-r--r--   0        0        0      188 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpsearchquerywidget.py
--rw-r--r--   0        0        0      216 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpsearchresult.py
--rw-r--r--   0        0        0      403 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qthelp/helpsearchresultwidget.py
--rw-r--r--   0        0        0     8290 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/qtre.py
--rw-r--r--   0        0        0      868 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/__init__.py
--rw-r--r--   0        0        0      208 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickasyncimageprovider.py
--rw-r--r--   0        0        0      257 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickimageprovider.py
--rw-r--r--   0        0        0      239 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickimageresponse.py
--rw-r--r--   0        0        0     3753 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickitem.py
--rw-r--r--   0        0        0      519 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickitemgrabresult.py
--rw-r--r--   0        0        0     1495 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickpainteditem.py
--rw-r--r--   0        0        0      239 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickrendercontrol.py
--rw-r--r--   0        0        0      271 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quicktextdocument.py
--rw-r--r--   0        0        0     1204 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickview.py
--rw-r--r--   0        0        0     3624 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/quick/quickwindow.py
--rw-r--r--   0        0        0      123 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/scintilla/__init__.py
--rw-r--r--   0        0        0     9347 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/scintilla/sciscintilla.py
--rw-r--r--   0        0        0      193 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/scxml/__init__.py
--rw-r--r--   0        0        0      362 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/scxml/scxmlcompiler.py
--rw-r--r--   0        0        0      176 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/scxml/scxmlstatemachine.py
--rw-r--r--   0        0        0      785 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/__init__.py
--rw-r--r--   0        0        0      361 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/abstractstate.py
--rw-r--r--   0        0        0     1159 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/abstracttransition.py
--rw-r--r--   0        0        0      220 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/eventtransition.py
--rw-r--r--   0        0        0      199 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/finalstate.py
--rw-r--r--   0        0        0     1104 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/historystate.py
--rw-r--r--   0        0        0      223 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/keyeventtransition.py
--rw-r--r--   0        0        0      227 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/mouseeventtransition.py
--rw-r--r--   0        0        0      222 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/signaltransition.py
--rw-r--r--   0        0        0     1276 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/state.py
--rw-r--r--   0        0        0     2222 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/statemachine/statemachine.py
--rw-r--r--   0        0        0      170 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/svg/__init__.py
--rw-r--r--   0        0        0      182 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/svg/graphicssvgitem.py
--rw-r--r--   0        0        0      405 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/svg/svggenerator.py
--rw-r--r--   0        0        0     1080 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/svg/svgrenderer.py
--rw-r--r--   0        0        0      279 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/svg/svgwidget.py
--rw-r--r--   0        0        0      675 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/highlightrule.py
--rw-r--r--   0        0        0     1271 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/jsonhighlighter.py
--rw-r--r--   0        0        0     3178 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/markdownhighlighter.py
--rw-r--r--   0        0        0      872 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py
--rw-r--r--   0        0        0     8585 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py
--rw-r--r--   0        0        0     4836 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/pythonhighlighter.py
--rw-r--r--   0        0        0     2079 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py
--rw-r--r--   0        0        0     2192 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/xmlhighlighter.py
--rw-r--r--   0        0        0     2106 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/syntaxhighlighters/yamlhighlighter.py
--rw-r--r--   0        0        0      180 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/texttospeech/__init__.py
--rw-r--r--   0        0        0     1328 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/texttospeech/texttospeech.py
--rw-r--r--   0        0        0      944 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/texttospeech/voice.py
--rw-r--r--   0        0        0    15547 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/themes/darktheme.qss
--rw-r--r--   0        0        0      845 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/utils/__init__.py
--rw-r--r--   0        0        0     3561 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/utils/autoslot.py
--rw-r--r--   0        0        0     3307 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/utils/colors.py
--rw-r--r--   0        0        0     2161 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/utils/debugging.py
--rw-r--r--   0        0        0     3598 2023-04-11 15:34:32.228385 prettyqt-1.3.0/prettyqt/utils/helpers.py
--rw-r--r--   0        0        0      894 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/mappers.py
--rw-r--r--   0        0        0     1054 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/prettyprinter.py
--rw-r--r--   0        0        0     5546 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/searchandreplacemixin.py
--rw-r--r--   0        0        0      629 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/signallogger.py
--rw-r--r--   0        0        0     2306 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/singleapplication.py
--rw-r--r--   0        0        0      493 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/singleton.py
--rw-r--r--   0        0        0     2110 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/syncedproperty.py
--rw-r--r--   0        0        0     1887 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/treeitem.py
--rw-r--r--   0        0        0     4119 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/utils/types.py
--rw-r--r--   0        0        0      303 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webchannel/__init__.py
--rw-r--r--   0        0        0      228 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webchannel/webchannel.py
--rw-r--r--   0        0        0     1337 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/__init__.py
--rw-r--r--   0        0        0     3315 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginecontextmenurequest.py
--rw-r--r--   0        0        0     4498 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginedownloadrequest.py
--rw-r--r--   0        0        0     1299 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginehistory.py
--rw-r--r--   0        0        0      422 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginehistoryitem.py
--rw-r--r--   0        0        0     1776 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginehttprequest.py
--rw-r--r--   0        0        0    14262 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginepage.py
--rw-r--r--   0        0        0     2461 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webengineprofile.py
--rw-r--r--   0        0        0     1574 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginescript.py
--rw-r--r--   0        0        0     1278 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginescriptcollection.py
--rw-r--r--   0        0        0     7469 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webenginesettings.py
--rw-r--r--   0        0        0     2044 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webengineurlscheme.py
--rw-r--r--   0        0        0      282 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginecore/webengineurlschemehandler.py
--rw-r--r--   0        0        0      330 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginewidgets/__init__.py
--rw-r--r--   0        0        0     4602 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/webenginewidgets/webengineview.py
--rw-r--r--   0        0        0    13448 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/__init__.py
--rw-r--r--   0        0        0     3797 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractbutton.py
--rw-r--r--   0        0        0      406 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractgraphicsshapeitem.py
--rw-r--r--   0        0        0      257 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractitemdelegate.py
--rw-r--r--   0        0        0    11883 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractitemview.py
--rw-r--r--   0        0        0     5361 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractscrollarea.py
--rw-r--r--   0        0        0     5646 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractslider.py
--rw-r--r--   0        0        0     3715 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/abstractspinbox.py
--rw-r--r--   0        0        0     8208 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/action.py
--rw-r--r--   0        0        0     2143 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/actiongroup.py
--rw-r--r--   0        0        0     8020 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/application.py
--rw-r--r--   0        0        0     2754 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/boxlayout.py
--rw-r--r--   0        0        0      342 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/buttongroup.py
--rw-r--r--   0        0        0     2960 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/calendarwidget.py
--rw-r--r--   0        0        0     1647 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/checkbox.py
--rw-r--r--   0        0        0     3856 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/colordialog.py
--rw-r--r--   0        0        0      331 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/columnview.py
--rw-r--r--   0        0        0     7000 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/combobox.py
--rw-r--r--   0        0        0      365 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/commandlinkbutton.py
--rw-r--r--   0        0        0      281 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/commonstyle.py
--rw-r--r--   0        0        0     3501 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/completer.py
--rw-r--r--   0        0        0     2700 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/datawidgetmapper.py
--rw-r--r--   0        0        0     1412 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/dateedit.py
--rw-r--r--   0        0        0     4324 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/datetimeedit.py
--rw-r--r--   0        0        0     1079 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/dial.py
--rw-r--r--   0        0        0     2824 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/dialog.py
--rw-r--r--   0        0        0     5950 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/dialogbuttonbox.py
--rw-r--r--   0        0        0     2356 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/dockwidget.py
--rw-r--r--   0        0        0     1772 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/doublespinbox.py
--rw-r--r--   0        0        0      328 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/errormessage.py
--rw-r--r--   0        0        0     7417 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/filedialog.py
--rw-r--r--   0        0        0      805 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/fileiconprovider.py
--rw-r--r--   0        0        0     3513 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/filesystemmodel.py
--rw-r--r--   0        0        0      289 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/focusframe.py
--rw-r--r--   0        0        0     2477 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/fontcombobox.py
--rw-r--r--   0        0        0      363 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/fontdialog.py
--rw-r--r--   0        0        0     4998 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/formlayout.py
--rw-r--r--   0        0        0     2540 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/frame.py
--rw-r--r--   0        0        0     1822 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/gesture.py
--rw-r--r--   0        0        0     2334 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsanchorlayout.py
--rw-r--r--   0        0        0     1360 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsblureffect.py
--rw-r--r--   0        0        0      469 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicscolorizeeffect.py
--rw-r--r--   0        0        0      435 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsdropshadoweffect.py
--rw-r--r--   0        0        0      416 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicseffect.py
--rw-r--r--   0        0        0      559 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsellipseitem.py
--rw-r--r--   0        0        0     3589 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsgridlayout.py
--rw-r--r--   0        0        0     4923 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsitem.py
--rw-r--r--   0        0        0      192 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicsitemgroup.py
--rw-r--r--   0        0        0     1173 2023-04-11 15:34:32.232385 prettyqt-1.3.0/prettyqt/widgets/graphicslayout.py
--rw-r--r--   0        0        0      262 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicslayoutitem.py
--rw-r--r--   0        0        0     1098 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicslinearlayout.py
--rw-r--r--   0        0        0      651 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicslineitem.py
--rw-r--r--   0        0        0      700 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsobject.py
--rw-r--r--   0        0        0      538 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsopacityeffect.py
--rw-r--r--   0        0        0      209 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicspathitem.py
--rw-r--r--   0        0        0     2241 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicspixmapitem.py
--rw-r--r--   0        0        0      800 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicspolygonitem.py
--rw-r--r--   0        0        0      198 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsproxywidget.py
--rw-r--r--   0        0        0      542 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsrectitem.py
--rw-r--r--   0        0        0      754 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsrotation.py
--rw-r--r--   0        0        0      490 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsscale.py
--rw-r--r--   0        0        0     8525 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsscene.py
--rw-r--r--   0        0        0      293 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicssimpletextitem.py
--rw-r--r--   0        0        0      707 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicstextitem.py
--rw-r--r--   0        0        0      310 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicstransform.py
--rw-r--r--   0        0        0     8619 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicsview.py
--rw-r--r--   0        0        0     2770 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/graphicswidget.py
--rw-r--r--   0        0        0     4159 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/gridlayout.py
--rw-r--r--   0        0        0     1955 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/groupbox.py
--rw-r--r--   0        0        0     5318 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/headerview.py
--rw-r--r--   0        0        0     3755 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/inputdialog.py
--rw-r--r--   0        0        0      190 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/itemdelegate.py
--rw-r--r--   0        0        0      144 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/itemeditorcreatorbase.py
--rw-r--r--   0        0        0     2331 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/itemeditorfactory.py
--rw-r--r--   0        0        0      846 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/keysequenceedit.py
--rw-r--r--   0        0        0     8483 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/label.py
--rw-r--r--   0        0        0     3961 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/layout.py
--rw-r--r--   0        0        0     1272 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/layoutitem.py
--rw-r--r--   0        0        0     2416 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/lcdnumber.py
--rw-r--r--   0        0        0     6525 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/lineedit.py
--rw-r--r--   0        0        0     5606 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/listview.py
--rw-r--r--   0        0        0     5823 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/listwidget.py
--rw-r--r--   0        0        0     2851 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/listwidgetitem.py
--rw-r--r--   0        0        0     6705 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/mainwindow.py
--rw-r--r--   0        0        0     4591 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/mdiarea.py
--rw-r--r--   0        0        0      689 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/mdisubwindow.py
--rw-r--r--   0        0        0     4397 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/menu.py
--rw-r--r--   0        0        0     2145 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/menubar.py
--rw-r--r--   0        0        0     7314 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/messagebox.py
--rw-r--r--   0        0        0      542 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/pangesture.py
--rw-r--r--   0        0        0     1902 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/pinchgesture.py
--rw-r--r--   0        0        0      415 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/plaintextdocumentlayout.py
--rw-r--r--   0        0        0     9079 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/plaintextedit.py
--rw-r--r--   0        0        0     3564 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/progressbar.py
--rw-r--r--   0        0        0     1029 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/progressdialog.py
--rw-r--r--   0        0        0      231 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/proxystyle.py
--rw-r--r--   0        0        0      804 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/pushbutton.py
--rw-r--r--   0        0        0      517 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/radiobutton.py
--rw-r--r--   0        0        0      758 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/rubberband.py
--rw-r--r--   0        0        0      611 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/scrollarea.py
--rw-r--r--   0        0        0      707 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/scrollbar.py
--rw-r--r--   0        0        0     3060 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/scroller.py
--rw-r--r--   0        0        0     3937 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/scrollerproperties.py
--rw-r--r--   0        0        0     1399 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/shortcut.py
--rw-r--r--   0        0        0      309 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/sizegrip.py
--rw-r--r--   0        0        0     5373 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/sizepolicy.py
--rw-r--r--   0        0        0     2654 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/slider.py
--rw-r--r--   0        0        0     1297 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/spaceritem.py
--rw-r--r--   0        0        0     1837 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/spinbox.py
--rw-r--r--   0        0        0     1181 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/splashscreen.py
--rw-r--r--   0        0        0     3920 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/splitter.py
--rw-r--r--   0        0        0     1417 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/splitterhandle.py
--rw-r--r--   0        0        0      983 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/stackedlayout.py
--rw-r--r--   0        0        0     1372 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/stackedwidget.py
--rw-r--r--   0        0        0     1677 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/statusbar.py
--rw-r--r--   0        0        0    19383 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/style.py
--rw-r--r--   0        0        0      208 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleditemdelegate.py
--rw-r--r--   0        0        0      126 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/stylefactory.py
--rw-r--r--   0        0        0      318 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoption.py
--rw-r--r--   0        0        0      686 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionbutton.py
--rw-r--r--   0        0        0      208 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptioncombobox.py
--rw-r--r--   0        0        0      260 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptioncomplex.py
--rw-r--r--   0        0        0      199 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiondockwidget.py
--rw-r--r--   0        0        0      197 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionfocusrect.py
--rw-r--r--   0        0        0      189 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionframe.py
--rw-r--r--   0        0        0      209 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiongraphicsitem.py
--rw-r--r--   0        0        0      197 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiongroupbox.py
--rw-r--r--   0        0        0      911 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionheader.py
--rw-r--r--   0        0        0     1032 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionmenuitem.py
--rw-r--r--   0        0        0      201 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionprogressbar.py
--rw-r--r--   0        0        0      199 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionrubberband.py
--rw-r--r--   0        0        0      208 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionsizegrip.py
--rw-r--r--   0        0        0     1046 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionslider.py
--rw-r--r--   0        0        0      195 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptionspinbox.py
--rw-r--r--   0        0        0     1135 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontab.py
--rw-r--r--   0        0        0      199 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontabbarbase.py
--rw-r--r--   0        0        0      213 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontabwidgetframe.py
--rw-r--r--   0        0        0      197 2023-04-11 15:34:32.236385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontitlebar.py
--rw-r--r--   0        0        0      397 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontoolbar.py
--rw-r--r--   0        0        0     1176 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontoolbox.py
--rw-r--r--   0        0        0      201 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/styleoptiontoolbutton.py
--rw-r--r--   0        0        0     1344 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/styleoptionviewitem.py
--rw-r--r--   0        0        0      397 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/stylepainter.py
--rw-r--r--   0        0        0     1311 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/swipegesture.py
--rw-r--r--   0        0        0     1732 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/systemtrayicon.py
--rw-r--r--   0        0        0     5232 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tabbar.py
--rw-r--r--   0        0        0     3112 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tableview.py
--rw-r--r--   0        0        0     1085 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tablewidget.py
--rw-r--r--   0        0        0     3334 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tablewidgetitem.py
--rw-r--r--   0        0        0     1920 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tablewidgetselectionrange.py
--rw-r--r--   0        0        0    10591 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tabwidget.py
--rw-r--r--   0        0        0      392 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tapandholdgesture.py
--rw-r--r--   0        0        0      371 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tapgesture.py
--rw-r--r--   0        0        0     2400 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/textbrowser.py
--rw-r--r--   0        0        0     6089 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/textedit.py
--rw-r--r--   0        0        0     1526 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/timeedit.py
--rw-r--r--   0        0        0     5008 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/toolbar.py
--rw-r--r--   0        0        0     2568 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/toolbox.py
--rw-r--r--   0        0        0     3175 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/toolbutton.py
--rw-r--r--   0        0        0      710 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/tooltip.py
--rw-r--r--   0        0        0     2532 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/treeview.py
--rw-r--r--   0        0        0      630 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/treewidget.py
--rw-r--r--   0        0        0     4841 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/treewidgetitem.py
--rw-r--r--   0        0        0     4142 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/treewidgetitemiterator.py
--rw-r--r--   0        0        0     1003 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/undoview.py
--rw-r--r--   0        0        0      552 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/whatsthis.py
--rw-r--r--   0        0        0    19395 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/widget.py
--rw-r--r--   0        0        0      545 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/widgetaction.py
--rw-r--r--   0        0        0      248 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/widgetitem.py
--rw-r--r--   0        0        0     9052 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/wizard.py
--rw-r--r--   0        0        0     1997 2023-04-11 15:34:32.240385 prettyqt-1.3.0/prettyqt/widgets/wizardpage.py
--rw-r--r--   0        0        0     4509 2023-04-11 15:34:32.240385 prettyqt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 prettyqt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-12 17:01:45.920375 prettyqt-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2746 2023-04-12 17:01:45.924375 prettyqt-1.4.1/docs/index.md
+-rw-r--r--   0        0        0      687 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/__init__.py
+-rw-r--r--   0        0        0      122 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/__pyinstaller/hook-prettyqt.py
+-rw-r--r--   0        0        0      517 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/bluetooth/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/bluetooth/bluetoothaddress.py
+-rw-r--r--   0        0        0     2635 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py
+-rw-r--r--   0        0        0     1421 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/bluetooth/bluetoothservicediscoveryagent.py
+-rw-r--r--   0        0        0     1872 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/bluetooth/bluetoothserviceinfo.py
+-rw-r--r--   0        0        0    11927 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/bluetooth/bluetoothuuid.py
+-rw-r--r--   0        0        0     1792 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/abstractaxis.py
+-rw-r--r--   0        0        0     1603 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/abstractbarseries.py
+-rw-r--r--   0        0        0      554 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/abstractseries.py
+-rw-r--r--   0        0        0      517 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/barcategoryaxis.py
+-rw-r--r--   0        0        0      177 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/barseries.py
+-rw-r--r--   0        0        0      932 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/barset.py
+-rw-r--r--   0        0        0     1648 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/boxset.py
+-rw-r--r--   0        0        0      609 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/candlestickset.py
+-rw-r--r--   0        0        0     1767 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/categoryaxis.py
+-rw-r--r--   0        0        0     5315 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/chart.py
+-rw-r--r--   0        0        0     5665 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/chartview.py
+-rw-r--r--   0        0        0      381 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/datetimeaxis.py
+-rw-r--r--   0        0        0      197 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/horizontalbarseries.py
+-rw-r--r--   0        0        0      217 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/horizontalpercentbarseries.py
+-rw-r--r--   0        0        0      217 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/horizontalstackedbarseries.py
+-rw-r--r--   0        0        0     2742 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/legend.py
+-rw-r--r--   0        0        0      673 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/lineseries.py
+-rw-r--r--   0        0        0      178 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/logvalueaxis.py
+-rw-r--r--   0        0        0      191 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/percentbarseries.py
+-rw-r--r--   0        0        0     2038 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/pieslice.py
+-rw-r--r--   0        0        0      739 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/polarchart.py
+-rw-r--r--   0        0        0      176 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/scatterseries.py
+-rw-r--r--   0        0        0      191 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/stackedbarseries.py
+-rw-r--r--   0        0        0     1044 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/valueaxis.py
+-rw-r--r--   0        0        0     1219 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/charts/xyseries.py
+-rw-r--r--   0        0        0    50840 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/constants/__init__.py
+-rw-r--r--   0        0        0     8711 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/_calendar.py
+-rw-r--r--   0        0        0     2000 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/_datetime.py
+-rw-r--r--   0        0        0    16492 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/_locale.py
+-rw-r--r--   0        0        0      478 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/_time.py
+-rw-r--r--   0        0        0     3286 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstractanimation.py
+-rw-r--r--   0        0        0      186 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstracteventdispatcher.py
+-rw-r--r--   0        0        0     5236 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstractitemmodel.py
+-rw-r--r--   0        0        0      250 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstractlistmodel.py
+-rw-r--r--   0        0        0      146 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstractnativeeventfilter.py
+-rw-r--r--   0        0        0      254 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstractproxymodel.py
+-rw-r--r--   0        0        0      254 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/abstracttablemodel.py
+-rw-r--r--   0        0        0     2060 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/animationgroup.py
+-rw-r--r--   0        0        0      533 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/basictimer.py
+-rw-r--r--   0        0        0      154 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/buffer.py
+-rw-r--r--   0        0        0      173 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/bytearray.py
+-rw-r--r--   0        0        0      369 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/bytearraymatcher.py
+-rw-r--r--   0        0        0      959 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/collator.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/collatorsortkey.py
+-rw-r--r--   0        0        0      324 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/commandlineoption.py
+-rw-r--r--   0        0        0     2231 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/commandlineparser.py
+-rw-r--r--   0        0        0      211 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/concatenatetablesproxymodel.py
+-rw-r--r--   0        0        0     3729 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/coreapplication.py
+-rw-r--r--   0        0        0     2038 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/cryptographichash.py
+-rw-r--r--   0        0        0     3426 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/datastream.py
+-rw-r--r--   0        0        0      470 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/date.py
+-rw-r--r--   0        0        0      766 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/deadlinetimer.py
+-rw-r--r--   0        0        0     1153 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/debug.py
+-rw-r--r--   0        0        0     4467 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/dir.py
+-rw-r--r--   0        0        0      264 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/diriterator.py
+-rw-r--r--   0        0        0     4527 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/easingcurve.py
+-rw-r--r--   0        0        0      918 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/elapsedtimer.py
+-rw-r--r--   0        0        0     7128 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/event.py
+-rw-r--r--   0        0        0     1225 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/eventloop.py
+-rw-r--r--   0        0        0      191 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/file.py
+-rw-r--r--   0        0        0     3694 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/filedevice.py
+-rw-r--r--   0        0        0     1492 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/fileinfo.py
+-rw-r--r--   0        0        0      560 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/fileselector.py
+-rw-r--r--   0        0        0      879 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/filesystemwatcher.py
+-rw-r--r--   0        0        0      188 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/identityproxymodel.py
+-rw-r--r--   0        0        0     1379 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/iodevice.py
+-rw-r--r--   0        0        0      122 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/itemselection.py
+-rw-r--r--   0        0        0      176 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/itemselectionmodel.py
+-rw-r--r--   0        0        0      696 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/itemselectionrange.py
+-rw-r--r--   0        0        0     1677 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/jsondocument.py
+-rw-r--r--   0        0        0      538 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/jsonvalue.py
+-rw-r--r--   0        0        0      726 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/keycombination.py
+-rw-r--r--   0        0        0     1248 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/library.py
+-rw-r--r--   0        0        0     1585 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/libraryinfo.py
+-rw-r--r--   0        0        0     1868 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/line.py
+-rw-r--r--   0        0        0     1997 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/linef.py
+-rw-r--r--   0        0        0      810 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/lockfile.py
+-rw-r--r--   0        0        0      708 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/margins.py
+-rw-r--r--   0        0        0      713 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/marginsf.py
+-rw-r--r--   0        0        0     1110 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/metaenum.py
+-rw-r--r--   0        0        0     1423 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/metamethod.py
+-rw-r--r--   0        0        0     3903 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/metaobject.py
+-rw-r--r--   0        0        0      511 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/metaproperty.py
+-rw-r--r--   0        0        0     5404 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/metatype.py
+-rw-r--r--   0        0        0     1802 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/mimedata.py
+-rw-r--r--   0        0        0      948 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/mimedatabase.py
+-rw-r--r--   0        0        0      208 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/mimetype.py
+-rw-r--r--   0        0        0      176 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/modelindex.py
+-rw-r--r--   0        0        0      336 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/mutex.py
+-rw-r--r--   0        0        0     3583 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/object.py
+-rw-r--r--   0        0        0     2562 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/operatingsystemversion.py
+-rw-r--r--   0        0        0      356 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/parallelanimationgroup.py
+-rw-r--r--   0        0        0      253 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/pauseanimation.py
+-rw-r--r--   0        0        0      338 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/persistentmodelindex.py
+-rw-r--r--   0        0        0      811 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/pluginloader.py
+-rw-r--r--   0        0        0      349 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/point.py
+-rw-r--r--   0        0        0      353 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/pointf.py
+-rw-r--r--   0        0        0     4839 2023-04-12 17:01:45.924375 prettyqt-1.4.1/prettyqt/core/process.py
+-rw-r--r--   0        0        0     1340 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/processenvironment.py
+-rw-r--r--   0        0        0      774 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/propertyanimation.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/randomgenerator.py
+-rw-r--r--   0        0        0      231 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/randomgenerator64.py
+-rw-r--r--   0        0        0      878 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/rect.py
+-rw-r--r--   0        0        0      442 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/rectf.py
+-rw-r--r--   0        0        0     6495 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/regularexpression.py
+-rw-r--r--   0        0        0     2579 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/regularexpressionmatch.py
+-rw-r--r--   0        0        0      613 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/regularexpressionmatchiterator.py
+-rw-r--r--   0        0        0     1702 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/resource.py
+-rw-r--r--   0        0        0      112 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/runnable.py
+-rw-r--r--   0        0        0      160 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/savefile.py
+-rw-r--r--   0        0        0      281 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/semaphore.py
+-rw-r--r--   0        0        0      202 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/sequentialanimationgroup.py
+-rw-r--r--   0        0        0     6990 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/settings.py
+-rw-r--r--   0        0        0      122 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/signalblocker.py
+-rw-r--r--   0        0        0      451 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/signalmapper.py
+-rw-r--r--   0        0        0     1124 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/size.py
+-rw-r--r--   0        0        0     1142 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/sizef.py
+-rw-r--r--   0        0        0      471 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/slot.py
+-rw-r--r--   0        0        0      930 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/socketnotifier.py
+-rw-r--r--   0        0        0     2681 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/sortfilterproxymodel.py
+-rw-r--r--   0        0        0     2622 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/standardpaths.py
+-rw-r--r--   0        0        0     1184 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/storageinfo.py
+-rw-r--r--   0        0        0      339 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/stringlistmodel.py
+-rw-r--r--   0        0        0      980 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/temporarydir.py
+-rw-r--r--   0        0        0      164 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/temporaryfile.py
+-rw-r--r--   0        0        0     2583 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/textboundaryfinder.py
+-rw-r--r--   0        0        0     3862 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/textstream.py
+-rw-r--r--   0        0        0      108 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/thread.py
+-rw-r--r--   0        0        0      160 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/threadpool.py
+-rw-r--r--   0        0        0     2318 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/timeline.py
+-rw-r--r--   0        0        0     1770 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/timer.py
+-rw-r--r--   0        0        0     2076 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/timezone.py
+-rw-r--r--   0        0        0     1722 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/translator.py
+-rw-r--r--   0        0        0      190 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/transposeproxymodel.py
+-rw-r--r--   0        0        0     3968 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/url.py
+-rw-r--r--   0        0        0      770 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/urlquery.py
+-rw-r--r--   0        0        0     1837 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/uuid.py
+-rw-r--r--   0        0        0     1501 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/variantanimation.py
+-rw-r--r--   0        0        0     2614 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/versionnumber.py
+-rw-r--r--   0        0        0     2614 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/core/xmlstreamreader.py
+-rw-r--r--   0        0        0      253 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_animations/__init__.py
+-rw-r--r--   0        0        0     1579 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_animations/bounceanimation.py
+-rw-r--r--   0        0        0      644 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_animations/fadeinanimation.py
+-rw-r--r--   0        0        0      978 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_animations/slideanimation.py
+-rw-r--r--   0        0        0      535 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/__init__.py
+-rw-r--r--   0        0        0      887 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/buttondelegate.py
+-rw-r--r--   0        0        0     1001 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/checkboxdelegate.py
+-rw-r--r--   0        0        0     2570 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/icondelegate.py
+-rw-r--r--   0        0        0      596 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/nofocusdelegate.py
+-rw-r--r--   0        0        0     1474 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/progressbardelegate.py
+-rw-r--r--   0        0        0     4789 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/radiodelegate.py
+-rw-r--r--   0        0        0     2574 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/renderlinkdelegate.py
+-rw-r--r--   0        0        0     6634 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_delegates/stardelegate.py
+-rw-r--r--   0        0        0      735 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/__init__.py
+-rw-r--r--   0        0        0     5965 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/columnitemmodel.py
+-rw-r--r--   0        0        0     3285 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/importlibdistributionmodel.py
+-rw-r--r--   0        0        0     4175 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/jsonmodel.py
+-rw-r--r--   0        0        0     3083 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/listmixin.py
+-rw-r--r--   0        0        0     2562 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/modelmixin.py
+-rw-r--r--   0        0        0     2298 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/nesteditem.py
+-rw-r--r--   0        0        0     2177 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/nestedmodel.py
+-rw-r--r--   0        0        0     2126 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/regexmatchesmodel.py
+-rw-r--r--   0        0        0     1698 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/selectionmixin.py
+-rw-r--r--   0        0        0     5288 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/storageinfomodel.py
+-rw-r--r--   0        0        0     2858 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_models/subsequencesortfilterproxymodel.py
+-rw-r--r--   0        0        0      635 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/__init__.py
+-rw-r--r--   0        0        0     2060 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/compositevalidator.py
+-rw-r--r--   0        0        0     1114 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/integervalidator.py
+-rw-r--r--   0        0        0      704 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/notemptyvalidator.py
+-rw-r--r--   0        0        0      700 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/notzerovalidator.py
+-rw-r--r--   0        0        0      620 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/pathvalidator.py
+-rw-r--r--   0        0        0     1554 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/regexpatternvalidator.py
+-rw-r--r--   0        0        0     3143 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_validators/regexvalidators.py
+-rw-r--r--   0        0        0     2704 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/__init__.py
+-rw-r--r--   0        0        0     1638 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/booldicttoolbutton.py
+-rw-r--r--   0        0        0     7718 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/borderlayout.py
+-rw-r--r--   0        0        0     3046 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/codeeditor.py
+-rw-r--r--   0        0        0     2588 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/collapsibleframe.py
+-rw-r--r--   0        0        0     2468 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/colorchooserbutton.py
+-rw-r--r--   0        0        0     7480 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/completionwidget.py
+-rw-r--r--   0        0        0    17651 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/dataset.py
+-rw-r--r--   0        0        0     2219 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/elidedlabel.py
+-rw-r--r--   0        0        0     3429 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/expandableline.py
+-rw-r--r--   0        0        0     3194 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/filechooserbutton.py
+-rw-r--r--   0        0        0     2155 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/flagselectionwidget.py
+-rw-r--r--   0        0        0     3847 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/flowlayout.py
+-rw-r--r--   0        0        0     2156 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/fontchooserbutton.py
+-rw-r--r--   0        0        0     9381 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/framelesswindow.py
+-rw-r--r--   0        0        0     5371 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/iconbrowser.py
+-rw-r--r--   0        0        0     1311 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/iconlabel.py
+-rw-r--r--   0        0        0     1661 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/iconwidget.py
+-rw-r--r--   0        0        0     1292 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/image.py
+-rw-r--r--   0        0        0      644 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/imageviewer.py
+-rw-r--r--   0        0        0     1931 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/inputandslider.py
+-rw-r--r--   0        0        0     2106 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/joystickbutton.py
+-rw-r--r--   0        0        0     4165 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/labeledslider.py
+-rw-r--r--   0        0        0     1214 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/listinput.py
+-rw-r--r--   0        0        0     8209 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/logtextedit.py
+-rw-r--r--   0        0        0      738 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/mappedcheckbox.py
+-rw-r--r--   0        0        0     2388 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/markdownwidget.py
+-rw-r--r--   0        0        0     6576 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/menurecentfiles.py
+-rw-r--r--   0        0        0    18898 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/notification.py
+-rw-r--r--   0        0        0     1038 2023-04-12 17:01:45.928375 prettyqt-1.4.1/prettyqt/custom_widgets/optionalwidget.py
+-rw-r--r--   0        0        0     1332 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/popupinfo.py
+-rw-r--r--   0        0        0      145 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/__main__.py
+-rw-r--r--   0        0        0     1039 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/quick_ref.py
+-rw-r--r--   0        0        0    19388 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/ref.html
+-rw-r--r--   0        0        0     6186 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py
+-rw-r--r--   0        0        0     3110 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/regexinput.py
+-rw-r--r--   0        0        0    10698 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/roundprogressbar.py
+-rw-r--r--   0        0        0     4284 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/selectionwidget.py
+-rw-r--r--   0        0        0     6345 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/sidebarwidget.py
+-rw-r--r--   0        0        0     1036 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/singlelinetextedit.py
+-rw-r--r--   0        0        0    18739 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/spanslider.py
+-rw-r--r--   0        0        0     1286 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/standardiconswidget.py
+-rw-r--r--   0        0        0     2289 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/stringornumberwidget.py
+-rw-r--r--   0        0        0     1774 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/subsequencecompleter.py
+-rw-r--r--   0        0        0     8034 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/timeline.py
+-rw-r--r--   0        0        0     9009 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/custom_widgets/waitingspinner.py
+-rw-r--r--   0        0        0      255 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/eventfilters/__init__.py
+-rw-r--r--   0        0        0     2613 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/eventfilters/animatedtooltipeventfilter.py
+-rw-r--r--   0        0        0      751 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/eventfilters/hovericoneventfilter.py
+-rw-r--r--   0        0        0     7915 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/__init__.py
+-rw-r--r--   0        0        0     1051 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/abstractfileiconprovider.py
+-rw-r--r--   0        0        0     1269 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/abstracttextdocumentlayout.py
+-rw-r--r--   0        0        0      235 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/bitmap.py
+-rw-r--r--   0        0        0     1451 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/brush.py
+-rw-r--r--   0        0        0     2490 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/clipboard.py
+-rw-r--r--   0        0        0     7632 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/color.py
+-rw-r--r--   0        0        0     3045 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/colorspace.py
+-rw-r--r--   0        0        0      485 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/conicalgradient.py
+-rw-r--r--   0        0        0     1255 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/cursor.py
+-rw-r--r--   0        0        0      439 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/desktopservices.py
+-rw-r--r--   0        0        0     1094 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/doublevalidator.py
+-rw-r--r--   0        0        0      973 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/drag.py
+-rw-r--r--   0        0        0     9049 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/font.py
+-rw-r--r--   0        0        0     4694 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/fontdatabase.py
+-rw-r--r--   0        0        0      243 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/fontinfo.py
+-rw-r--r--   0        0        0      889 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/fontmetrics.py
+-rw-r--r--   0        0        0      719 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/fontmetricsf.py
+-rw-r--r--   0        0        0     5331 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/gradient.py
+-rw-r--r--   0        0        0     5027 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/guiapplication.py
+-rw-r--r--   0        0        0     3986 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/icon.py
+-rw-r--r--   0        0        0     4053 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/iconengine.py
+-rw-r--r--   0        0        0     1630 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/image.py
+-rw-r--r--   0        0        0     3778 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/imageiohandler.py
+-rw-r--r--   0        0        0     3838 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/imagereader.py
+-rw-r--r--   0        0        0     2791 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/imagewriter.py
+-rw-r--r--   0        0        0     1315 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/inputmethod.py
+-rw-r--r--   0        0        0      921 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/intvalidator.py
+-rw-r--r--   0        0        0     6154 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/keysequence.py
+-rw-r--r--   0        0        0      636 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/lineargradient.py
+-rw-r--r--   0        0        0      302 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/matrix4x4.py
+-rw-r--r--   0        0        0     1969 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/movie.py
+-rw-r--r--   0        0        0      297 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pagedpaintdevice.py
+-rw-r--r--   0        0        0     2923 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pagelayout.py
+-rw-r--r--   0        0        0     7804 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pagesize.py
+-rw-r--r--   0        0        0     1676 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/paintdevice.py
+-rw-r--r--   0        0        0      319 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/paintdevicewindow.py
+-rw-r--r--   0        0        0     7794 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/painter.py
+-rw-r--r--   0        0        0     2425 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/painterpath.py
+-rw-r--r--   0        0        0     1641 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/painterpathstroker.py
+-rw-r--r--   0        0        0     5907 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/palette.py
+-rw-r--r--   0        0        0     1026 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pdfwriter.py
+-rw-r--r--   0        0        0     2841 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pen.py
+-rw-r--r--   0        0        0      471 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/picture.py
+-rw-r--r--   0        0        0     4827 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pixmap.py
+-rw-r--r--   0        0        0      796 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/pixmapcache.py
+-rw-r--r--   0        0        0     3489 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/polygon.py
+-rw-r--r--   0        0        0     4325 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/polygonf.py
+-rw-r--r--   0        0        0      898 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/radialgradient.py
+-rw-r--r--   0        0        0      220 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/rasterwindow.py
+-rw-r--r--   0        0        0     1145 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/region.py
+-rw-r--r--   0        0        0     1290 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/regularexpressionvalidator.py
+-rw-r--r--   0        0        0     2963 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/screen.py
+-rw-r--r--   0        0        0     1291 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/sessionmanager.py
+-rw-r--r--   0        0        0     6203 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/standarditem.py
+-rw-r--r--   0        0        0     4778 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/standarditemmodel.py
+-rw-r--r--   0        0        0     2225 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/statictext.py
+-rw-r--r--   0        0        0     1146 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/stylehints.py
+-rw-r--r--   0        0        0     1303 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/surface.py
+-rw-r--r--   0        0        0     1352 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/syntaxhighlighter.py
+-rw-r--r--   0        0        0     5251 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textblock.py
+-rw-r--r--   0        0        0      623 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textblockgroup.py
+-rw-r--r--   0        0        0      536 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textblockuserdata.py
+-rw-r--r--   0        0        0     4878 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textcharformat.py
+-rw-r--r--   0        0        0     5551 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textcursor.py
+-rw-r--r--   0        0        0     7781 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textdocument.py
+-rw-r--r--   0        0        0      949 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textdocumentfragment.py
+-rw-r--r--   0        0        0     1062 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textdocumentwriter.py
+-rw-r--r--   0        0        0     3262 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textformat.py
+-rw-r--r--   0        0        0      534 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textframe.py
+-rw-r--r--   0        0        0     3627 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textframeformat.py
+-rw-r--r--   0        0        0      297 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textimageformat.py
+-rw-r--r--   0        0        0      517 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textlayout.py
+-rw-r--r--   0        0        0      725 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textlength.py
+-rw-r--r--   0        0        0     1649 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textline.py
+-rw-r--r--   0        0        0     1327 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textlistformat.py
+-rw-r--r--   0        0        0      445 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textobject.py
+-rw-r--r--   0        0        0      199 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textobjectinterface.py
+-rw-r--r--   0        0        0     1560 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/textoption.py
+-rw-r--r--   0        0        0     4104 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/texttablecellformat.py
+-rw-r--r--   0        0        0     2482 2023-04-12 17:01:45.932375 prettyqt-1.4.1/prettyqt/gui/transform.py
+-rw-r--r--   0        0        0      640 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/undocommand.py
+-rw-r--r--   0        0        0      356 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/undogroup.py
+-rw-r--r--   0        0        0      957 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/undostack.py
+-rw-r--r--   0        0        0      755 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/validator.py
+-rw-r--r--   0        0        0      575 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/vector3d.py
+-rw-r--r--   0        0        0      578 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/vector4d.py
+-rw-r--r--   0        0        0     2338 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/gui/window.py
+-rw-r--r--   0        0        0    10227 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/__init__.py
+-rw-r--r--   0        0        0     1387 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/animation.py
+-rw-r--r--   0        0        0     3079 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/awesomefileiconprovider.py
+-rw-r--r--   0        0        0      539 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/awesomequickimageprovider.py
+-rw-r--r--   0        0        0      832 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/chariconengine.py
+-rw-r--r--   0        0        0    10996 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/codicon-charmap.json
+-rw-r--r--   0        0        0    68076 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/codicon.ttf
+-rw-r--r--   0        0        0     7924 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json
+-rw-r--r--   0        0        0    79556 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf
+-rw-r--r--   0        0        0    11206 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json
+-rw-r--r--   0        0        0   134316 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf
+-rw-r--r--   0        0        0     3947 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json
+-rw-r--r--   0        0        0    33692 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf
+-rw-r--r--   0        0        0    25663 2023-04-12 17:01:45.936375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json
+-rw-r--r--   0        0        0   203644 2023-04-12 17:01:45.940375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf
+-rw-r--r--   0        0        0   200215 2023-04-12 17:01:45.940375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json
+-rw-r--r--   0        0        0  1026284 2023-04-12 17:01:45.948375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf
+-rw-r--r--   0        0        0   216192 2023-04-12 17:01:45.948375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json
+-rw-r--r--   0        0        0  1108672 2023-04-12 17:01:45.952375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf
+-rw-r--r--   0        0        0   151941 2023-04-12 17:01:45.952375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/phosphor-charmap.json
+-rw-r--r--   0        0        0  1392088 2023-04-12 17:01:45.960375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/phosphor.ttf
+-rw-r--r--   0        0        0    72655 2023-04-12 17:01:45.960375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/remixicon-charmap.json
+-rw-r--r--   0        0        0   403056 2023-04-12 17:01:45.964375 prettyqt-1.4.1/prettyqt/iconprovider/fonts/remixicon.ttf
+-rw-r--r--   0        0        0     8417 2023-04-12 17:01:45.964375 prettyqt-1.4.1/prettyqt/iconprovider/iconic_font.py
+-rw-r--r--   0        0        0     2468 2023-04-12 17:01:45.964375 prettyqt-1.4.1/prettyqt/iconprovider/svgbuffericonengine.py
+-rw-r--r--   0        0        0   154232 2023-04-12 17:01:45.964375 prettyqt-1.4.1/prettyqt/localization/language_ar.qm
+-rw-r--r--   0        0        0   155315 2023-04-12 17:01:45.964375 prettyqt-1.4.1/prettyqt/localization/language_bg.qm
+-rw-r--r--   0        0        0   178552 2023-04-12 17:01:45.964375 prettyqt-1.4.1/prettyqt/localization/language_ca.qm
+-rw-r--r--   0        0        0   151054 2023-04-12 17:01:45.968375 prettyqt-1.4.1/prettyqt/localization/language_cs.qm
+-rw-r--r--   0        0        0   179910 2023-04-12 17:01:45.968375 prettyqt-1.4.1/prettyqt/localization/language_da.qm
+-rw-r--r--   0        0        0   212675 2023-04-12 17:01:45.968375 prettyqt-1.4.1/prettyqt/localization/language_de.qm
+-rw-r--r--   0        0        0   154543 2023-04-12 17:01:45.968375 prettyqt-1.4.1/prettyqt/localization/language_es.qm
+-rw-r--r--   0        0        0    97872 2023-04-12 17:01:45.972375 prettyqt-1.4.1/prettyqt/localization/language_fa.qm
+-rw-r--r--   0        0        0   174500 2023-04-12 17:01:45.972375 prettyqt-1.4.1/prettyqt/localization/language_fi.qm
+-rw-r--r--   0        0        0   154190 2023-04-12 17:01:45.972375 prettyqt-1.4.1/prettyqt/localization/language_fr.qm
+-rw-r--r--   0        0        0   183091 2023-04-12 17:01:45.972375 prettyqt-1.4.1/prettyqt/localization/language_gd.qm
+-rw-r--r--   0        0        0   108600 2023-04-12 17:01:45.972375 prettyqt-1.4.1/prettyqt/localization/language_gl.qm
+-rw-r--r--   0        0        0   130568 2023-04-12 17:01:45.976375 prettyqt-1.4.1/prettyqt/localization/language_he.qm
+-rw-r--r--   0        0        0   150033 2023-04-12 17:01:45.976375 prettyqt-1.4.1/prettyqt/localization/language_hu.qm
+-rw-r--r--   0        0        0   153570 2023-04-12 17:01:45.976375 prettyqt-1.4.1/prettyqt/localization/language_it.qm
+-rw-r--r--   0        0        0   122385 2023-04-12 17:01:45.976375 prettyqt-1.4.1/prettyqt/localization/language_ja.qm
+-rw-r--r--   0        0        0   120318 2023-04-12 17:01:45.976375 prettyqt-1.4.1/prettyqt/localization/language_ko.qm
+-rw-r--r--   0        0        0    90502 2023-04-12 17:01:45.976375 prettyqt-1.4.1/prettyqt/localization/language_lt.qm
+-rw-r--r--   0        0        0   143558 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_lv.qm
+-rw-r--r--   0        0        0   161318 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_pl.qm
+-rw-r--r--   0        0        0    50541 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_pt.qm
+-rw-r--r--   0        0        0   197476 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_ru.qm
+-rw-r--r--   0        0        0   115250 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_sk.qm
+-rw-r--r--   0        0        0    96357 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_sl.qm
+-rw-r--r--   0        0        0    47206 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_sv.qm
+-rw-r--r--   0        0        0   148437 2023-04-12 17:01:45.980375 prettyqt-1.4.1/prettyqt/localization/language_uk.qm
+-rw-r--r--   0        0        0    61089 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/localization/language_zh_CN.qm
+-rw-r--r--   0        0        0   125250 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/localization/language_zh_TW.qm
+-rw-r--r--   0        0        0     2384 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/geocodingmanager.py
+-rw-r--r--   0        0        0     2867 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/geomaneuver.py
+-rw-r--r--   0        0        0     1055 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/georoute.py
+-rw-r--r--   0        0        0     5266 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/georouterequest.py
+-rw-r--r--   0        0        0      657 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/georoutesegment.py
+-rw-r--r--   0        0        0     2021 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/georoutingmanager.py
+-rw-r--r--   0        0        0     5880 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/geoserviceprovider.py
+-rw-r--r--   0        0        0     2387 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/place.py
+-rw-r--r--   0        0        0      864 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeattribute.py
+-rw-r--r--   0        0        0      737 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placecategory.py
+-rw-r--r--   0        0        0      844 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placecontactdetail.py
+-rw-r--r--   0        0        0     1030 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placecontent.py
+-rw-r--r--   0        0        0     1275 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placecontentreply.py
+-rw-r--r--   0        0        0      947 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placecontentrequest.py
+-rw-r--r--   0        0        0      562 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placedetailsreply.py
+-rw-r--r--   0        0        0      849 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeicon.py
+-rw-r--r--   0        0        0     1185 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeidreply.py
+-rw-r--r--   0        0        0     2233 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placemanager.py
+-rw-r--r--   0        0        0     1066 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placematchreply.py
+-rw-r--r--   0        0        0      726 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placematchrequest.py
+-rw-r--r--   0        0        0      223 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeproposedsearchresult.py
+-rw-r--r--   0        0        0      316 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeratings.py
+-rw-r--r--   0        0        0     1923 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placereply.py
+-rw-r--r--   0        0        0      267 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeresult.py
+-rw-r--r--   0        0        0     1651 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placesearchreply.py
+-rw-r--r--   0        0        0     2230 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placesearchrequest.py
+-rw-r--r--   0        0        0      884 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placesearchresult.py
+-rw-r--r--   0        0        0      675 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placesupplier.py
+-rw-r--r--   0        0        0      215 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/placeuser.py
+-rw-r--r--   0        0        0      621 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/location/qlocation.py
+-rw-r--r--   0        0        0      167 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/multimediawidgets/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/multimediawidgets/graphicsvideoitem.py
+-rw-r--r--   0        0        0      872 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/multimediawidgets/videowidget.py
+-rw-r--r--   0        0        0     1172 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/__init__.py
+-rw-r--r--   0        0        0     8113 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/abstractsocket.py
+-rw-r--r--   0        0        0     1775 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/hostaddress.py
+-rw-r--r--   0        0        0     1465 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/httpmultipart.py
+-rw-r--r--   0        0        0      823 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/httppart.py
+-rw-r--r--   0        0        0     1310 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/localserver.py
+-rw-r--r--   0        0        0     2392 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/localsocket.py
+-rw-r--r--   0        0        0     2313 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkaccessmanager.py
+-rw-r--r--   0        0        0     2000 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkaddressentry.py
+-rw-r--r--   0        0        0     1551 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkcookie.py
+-rw-r--r--   0        0        0      850 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkcookiejar.py
+-rw-r--r--   0        0        0      627 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkdatagram.py
+-rw-r--r--   0        0        0     3011 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkinterface.py
+-rw-r--r--   0        0        0     3361 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkproxy.py
+-rw-r--r--   0        0        0     6462 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/networkrequest.py
+-rw-r--r--   0        0        0      779 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/tcpserver.py
+-rw-r--r--   0        0        0      178 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/tcpsocket.py
+-rw-r--r--   0        0        0      671 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/network/udpsocket.py
+-rw-r--r--   0        0        0       26 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/objbrowser/__init__.py
+-rw-r--r--   0        0        0     9193 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/objbrowser/attribute_model.py
+-rw-r--r--   0        0        0    14897 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/objbrowser/objectbrowser.py
+-rw-r--r--   0        0        0    18451 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/objbrowser/objectbrowsertreemodel.py
+-rw-r--r--   0        0        0      356 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/paths.py
+-rw-r--r--   0        0        0     1169 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geoaddress.py
+-rw-r--r--   0        0        0     1149 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geoareamonitorinfo.py
+-rw-r--r--   0        0        0     1260 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geoareamonitorsource.py
+-rw-r--r--   0        0        0     1072 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geocircle.py
+-rw-r--r--   0        0        0     1172 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geocoordinate.py
+-rw-r--r--   0        0        0      558 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geolocation.py
+-rw-r--r--   0        0        0     1021 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geopath.py
+-rw-r--r--   0        0        0     1145 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geopolygon.py
+-rw-r--r--   0        0        0     1687 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geopositioninfo.py
+-rw-r--r--   0        0        0     2960 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geopositioninfosource.py
+-rw-r--r--   0        0        0      769 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/georectangle.py
+-rw-r--r--   0        0        0     1861 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geosatelliteinfo.py
+-rw-r--r--   0        0        0     1110 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geosatelliteinfosource.py
+-rw-r--r--   0        0        0      755 2023-04-12 17:01:45.984375 prettyqt-1.4.1/prettyqt/positioning/geoshape.py
+-rw-r--r--   0        0        0     1196 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/positioning/nmeapositioninginfosource.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/py.typed
+-rw-r--r--   0        0        0      943 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/jsengine.py
+-rw-r--r--   0        0        0     2397 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/jsvalue.py
+-rw-r--r--   0        0        0      295 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/jsvalueiterator.py
+-rw-r--r--   0        0        0      955 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/qmlapplicationengine.py
+-rw-r--r--   0        0        0      907 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/qmlcomponent.py
+-rw-r--r--   0        0        0     2020 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/qmlengine.py
+-rw-r--r--   0        0        0      536 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/qmlimageproviderbase.py
+-rw-r--r--   0        0        0      185 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qml/qmlparserstatus.py
+-rw-r--r--   0        0        0      203 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/Qsci/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtBluetooth/__init__.py
+-rw-r--r--   0        0        0      446 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtCharts/__init__.py
+-rw-r--r--   0        0        0     2281 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtCore/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtGui/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtHelp/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtLocation/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtMultimedia/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtMultimediaWidgets/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtNetwork/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtPositioning/__init__.py
+-rw-r--r--   0        0        0      266 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtQml/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtQuick/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtScxml/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtStateMachine/__init__.py
+-rw-r--r--   0        0        0      332 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtSvg/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtTest/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtTextToSpeech/__init__.py
+-rw-r--r--   0        0        0      368 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtUiTools/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtWebChannel/__init__.py
+-rw-r--r--   0        0        0      280 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtWebEngineCore/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtWebEngineWidgets/__init__.py
+-rw-r--r--   0        0        0     1548 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/QtWidgets/__init__.py
+-rw-r--r--   0        0        0     1200 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qt/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpcontentitem.py
+-rw-r--r--   0        0        0      443 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpcontentmodel.py
+-rw-r--r--   0        0        0      460 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpcontentwidget.py
+-rw-r--r--   0        0        0      371 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpengine.py
+-rw-r--r--   0        0        0     1107 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpenginecore.py
+-rw-r--r--   0        0        0      661 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpfilterdata.py
+-rw-r--r--   0        0        0      739 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpfilterengine.py
+-rw-r--r--   0        0        0      177 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpindexmodel.py
+-rw-r--r--   0        0        0      178 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpindexwidget.py
+-rw-r--r--   0        0        0      729 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpsearchengine.py
+-rw-r--r--   0        0        0      188 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpsearchquerywidget.py
+-rw-r--r--   0        0        0      216 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpsearchresult.py
+-rw-r--r--   0        0        0      832 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qthelp/helpsearchresultwidget.py
+-rw-r--r--   0        0        0     8290 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/qtre.py
+-rw-r--r--   0        0        0      868 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickasyncimageprovider.py
+-rw-r--r--   0        0        0      257 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickimageprovider.py
+-rw-r--r--   0        0        0      239 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickimageresponse.py
+-rw-r--r--   0        0        0     3753 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickitem.py
+-rw-r--r--   0        0        0      519 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickitemgrabresult.py
+-rw-r--r--   0        0        0     1495 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickpainteditem.py
+-rw-r--r--   0        0        0      239 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickrendercontrol.py
+-rw-r--r--   0        0        0      271 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quicktextdocument.py
+-rw-r--r--   0        0        0     1204 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickview.py
+-rw-r--r--   0        0        0     3624 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/quick/quickwindow.py
+-rw-r--r--   0        0        0      123 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/scintilla/__init__.py
+-rw-r--r--   0        0        0     9347 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/scintilla/sciscintilla.py
+-rw-r--r--   0        0        0      193 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/scxml/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/scxml/scxmlcompiler.py
+-rw-r--r--   0        0        0      176 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/scxml/scxmlstatemachine.py
+-rw-r--r--   0        0        0      785 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/__init__.py
+-rw-r--r--   0        0        0      361 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/abstractstate.py
+-rw-r--r--   0        0        0     1159 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/abstracttransition.py
+-rw-r--r--   0        0        0      220 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/eventtransition.py
+-rw-r--r--   0        0        0      199 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/finalstate.py
+-rw-r--r--   0        0        0     1104 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/historystate.py
+-rw-r--r--   0        0        0      223 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/keyeventtransition.py
+-rw-r--r--   0        0        0      227 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/mouseeventtransition.py
+-rw-r--r--   0        0        0      222 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/signaltransition.py
+-rw-r--r--   0        0        0     1276 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/state.py
+-rw-r--r--   0        0        0     2222 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/statemachine/statemachine.py
+-rw-r--r--   0        0        0      170 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/svg/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/svg/graphicssvgitem.py
+-rw-r--r--   0        0        0      405 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/svg/svggenerator.py
+-rw-r--r--   0        0        0     1080 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/svg/svgrenderer.py
+-rw-r--r--   0        0        0      279 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/svg/svgwidget.py
+-rw-r--r--   0        0        0      675 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/highlightrule.py
+-rw-r--r--   0        0        0     1271 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/jsonhighlighter.py
+-rw-r--r--   0        0        0     3178 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/markdownhighlighter.py
+-rw-r--r--   0        0        0      872 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py
+-rw-r--r--   0        0        0     8585 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/pygmentshighlighter.py
+-rw-r--r--   0        0        0     4836 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/pythonhighlighter.py
+-rw-r--r--   0        0        0     2079 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/regexmatchhighlighter.py
+-rw-r--r--   0        0        0     2192 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/xmlhighlighter.py
+-rw-r--r--   0        0        0     2106 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/syntaxhighlighters/yamlhighlighter.py
+-rw-r--r--   0        0        0      180 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/texttospeech/__init__.py
+-rw-r--r--   0        0        0     1328 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/texttospeech/texttospeech.py
+-rw-r--r--   0        0        0      944 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/texttospeech/voice.py
+-rw-r--r--   0        0        0    15547 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/themes/darktheme.qss
+-rw-r--r--   0        0        0      845 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/__init__.py
+-rw-r--r--   0        0        0     3561 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/autoslot.py
+-rw-r--r--   0        0        0     3307 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/colors.py
+-rw-r--r--   0        0        0     2161 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/debugging.py
+-rw-r--r--   0        0        0     3598 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/helpers.py
+-rw-r--r--   0        0        0      894 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/mappers.py
+-rw-r--r--   0        0        0     1054 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/prettyprinter.py
+-rw-r--r--   0        0        0     5546 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/searchandreplacemixin.py
+-rw-r--r--   0        0        0      629 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/signallogger.py
+-rw-r--r--   0        0        0     2306 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/singleapplication.py
+-rw-r--r--   0        0        0      493 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/singleton.py
+-rw-r--r--   0        0        0     2110 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/syncedproperty.py
+-rw-r--r--   0        0        0     1887 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/treeitem.py
+-rw-r--r--   0        0        0     4119 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/utils/types.py
+-rw-r--r--   0        0        0      303 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/webchannel/__init__.py
+-rw-r--r--   0        0        0      228 2023-04-12 17:01:45.988375 prettyqt-1.4.1/prettyqt/webchannel/webchannel.py
+-rw-r--r--   0        0        0     1337 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/__init__.py
+-rw-r--r--   0        0        0     3315 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginecontextmenurequest.py
+-rw-r--r--   0        0        0     4498 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginedownloadrequest.py
+-rw-r--r--   0        0        0     1299 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginehistory.py
+-rw-r--r--   0        0        0      422 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginehistoryitem.py
+-rw-r--r--   0        0        0     1776 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginehttprequest.py
+-rw-r--r--   0        0        0    14262 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginepage.py
+-rw-r--r--   0        0        0     2461 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webengineprofile.py
+-rw-r--r--   0        0        0     1574 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginescript.py
+-rw-r--r--   0        0        0     1278 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginescriptcollection.py
+-rw-r--r--   0        0        0     7469 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webenginesettings.py
+-rw-r--r--   0        0        0     2044 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webengineurlscheme.py
+-rw-r--r--   0        0        0      282 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginecore/webengineurlschemehandler.py
+-rw-r--r--   0        0        0      330 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginewidgets/__init__.py
+-rw-r--r--   0        0        0     4602 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/webenginewidgets/webengineview.py
+-rw-r--r--   0        0        0    13448 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/__init__.py
+-rw-r--r--   0        0        0     3797 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractbutton.py
+-rw-r--r--   0        0        0      406 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractgraphicsshapeitem.py
+-rw-r--r--   0        0        0      257 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractitemdelegate.py
+-rw-r--r--   0        0        0    11883 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractitemview.py
+-rw-r--r--   0        0        0     5361 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractscrollarea.py
+-rw-r--r--   0        0        0     5646 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractslider.py
+-rw-r--r--   0        0        0     3715 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/abstractspinbox.py
+-rw-r--r--   0        0        0     8208 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/action.py
+-rw-r--r--   0        0        0     2143 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/actiongroup.py
+-rw-r--r--   0        0        0     8020 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/application.py
+-rw-r--r--   0        0        0     2754 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/boxlayout.py
+-rw-r--r--   0        0        0      342 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/buttongroup.py
+-rw-r--r--   0        0        0     2960 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/calendarwidget.py
+-rw-r--r--   0        0        0     1647 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/checkbox.py
+-rw-r--r--   0        0        0     3856 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/colordialog.py
+-rw-r--r--   0        0        0      331 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/columnview.py
+-rw-r--r--   0        0        0     7000 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/combobox.py
+-rw-r--r--   0        0        0      365 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/commandlinkbutton.py
+-rw-r--r--   0        0        0      281 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/commonstyle.py
+-rw-r--r--   0        0        0     3501 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/completer.py
+-rw-r--r--   0        0        0     2700 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/datawidgetmapper.py
+-rw-r--r--   0        0        0     1412 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/dateedit.py
+-rw-r--r--   0        0        0     4324 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/datetimeedit.py
+-rw-r--r--   0        0        0     1079 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/dial.py
+-rw-r--r--   0        0        0     2813 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/dialog.py
+-rw-r--r--   0        0        0     5950 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/dialogbuttonbox.py
+-rw-r--r--   0        0        0     2356 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/dockwidget.py
+-rw-r--r--   0        0        0     1772 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/doublespinbox.py
+-rw-r--r--   0        0        0      328 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/errormessage.py
+-rw-r--r--   0        0        0     7417 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/filedialog.py
+-rw-r--r--   0        0        0      805 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/fileiconprovider.py
+-rw-r--r--   0        0        0     3541 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/filesystemmodel.py
+-rw-r--r--   0        0        0      289 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/focusframe.py
+-rw-r--r--   0        0        0     2477 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/fontcombobox.py
+-rw-r--r--   0        0        0      363 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/fontdialog.py
+-rw-r--r--   0        0        0     4998 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/formlayout.py
+-rw-r--r--   0        0        0     2540 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/frame.py
+-rw-r--r--   0        0        0     1822 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/gesture.py
+-rw-r--r--   0        0        0     2334 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsanchorlayout.py
+-rw-r--r--   0        0        0     1360 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsblureffect.py
+-rw-r--r--   0        0        0      469 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicscolorizeeffect.py
+-rw-r--r--   0        0        0      435 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsdropshadoweffect.py
+-rw-r--r--   0        0        0      416 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicseffect.py
+-rw-r--r--   0        0        0      559 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsellipseitem.py
+-rw-r--r--   0        0        0     3589 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsgridlayout.py
+-rw-r--r--   0        0        0     4923 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsitem.py
+-rw-r--r--   0        0        0      192 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsitemgroup.py
+-rw-r--r--   0        0        0     1173 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicslayout.py
+-rw-r--r--   0        0        0      262 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicslayoutitem.py
+-rw-r--r--   0        0        0     1098 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicslinearlayout.py
+-rw-r--r--   0        0        0      651 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicslineitem.py
+-rw-r--r--   0        0        0      700 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsobject.py
+-rw-r--r--   0        0        0      538 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsopacityeffect.py
+-rw-r--r--   0        0        0      209 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicspathitem.py
+-rw-r--r--   0        0        0     2241 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicspixmapitem.py
+-rw-r--r--   0        0        0      800 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicspolygonitem.py
+-rw-r--r--   0        0        0      198 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsproxywidget.py
+-rw-r--r--   0        0        0      542 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsrectitem.py
+-rw-r--r--   0        0        0      754 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsrotation.py
+-rw-r--r--   0        0        0      490 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsscale.py
+-rw-r--r--   0        0        0     8525 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsscene.py
+-rw-r--r--   0        0        0      293 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicssimpletextitem.py
+-rw-r--r--   0        0        0      707 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicstextitem.py
+-rw-r--r--   0        0        0      310 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicstransform.py
+-rw-r--r--   0        0        0     8619 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicsview.py
+-rw-r--r--   0        0        0     2770 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/graphicswidget.py
+-rw-r--r--   0        0        0     4159 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/gridlayout.py
+-rw-r--r--   0        0        0     1955 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/groupbox.py
+-rw-r--r--   0        0        0     5318 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/headerview.py
+-rw-r--r--   0        0        0     3755 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/inputdialog.py
+-rw-r--r--   0        0        0      190 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/itemdelegate.py
+-rw-r--r--   0        0        0      144 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/itemeditorcreatorbase.py
+-rw-r--r--   0        0        0     2331 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/itemeditorfactory.py
+-rw-r--r--   0        0        0      846 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/keysequenceedit.py
+-rw-r--r--   0        0        0     8483 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/label.py
+-rw-r--r--   0        0        0     3961 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/layout.py
+-rw-r--r--   0        0        0     1272 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/layoutitem.py
+-rw-r--r--   0        0        0     2416 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/lcdnumber.py
+-rw-r--r--   0        0        0     6546 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/lineedit.py
+-rw-r--r--   0        0        0     5606 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/listview.py
+-rw-r--r--   0        0        0     5823 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/listwidget.py
+-rw-r--r--   0        0        0     2851 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/listwidgetitem.py
+-rw-r--r--   0        0        0     6705 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/mainwindow.py
+-rw-r--r--   0        0        0     4591 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/mdiarea.py
+-rw-r--r--   0        0        0      689 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/mdisubwindow.py
+-rw-r--r--   0        0        0     4397 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/menu.py
+-rw-r--r--   0        0        0     2145 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/menubar.py
+-rw-r--r--   0        0        0     7314 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/messagebox.py
+-rw-r--r--   0        0        0      542 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/pangesture.py
+-rw-r--r--   0        0        0     1902 2023-04-12 17:01:45.992375 prettyqt-1.4.1/prettyqt/widgets/pinchgesture.py
+-rw-r--r--   0        0        0      415 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/plaintextdocumentlayout.py
+-rw-r--r--   0        0        0     9079 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/plaintextedit.py
+-rw-r--r--   0        0        0     3564 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/progressbar.py
+-rw-r--r--   0        0        0     1029 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/progressdialog.py
+-rw-r--r--   0        0        0      231 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/proxystyle.py
+-rw-r--r--   0        0        0      804 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/pushbutton.py
+-rw-r--r--   0        0        0      517 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/radiobutton.py
+-rw-r--r--   0        0        0      758 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/rubberband.py
+-rw-r--r--   0        0        0      611 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/scrollarea.py
+-rw-r--r--   0        0        0      707 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/scrollbar.py
+-rw-r--r--   0        0        0     3060 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/scroller.py
+-rw-r--r--   0        0        0     3937 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/scrollerproperties.py
+-rw-r--r--   0        0        0     1399 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/shortcut.py
+-rw-r--r--   0        0        0      309 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/sizegrip.py
+-rw-r--r--   0        0        0     5373 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/sizepolicy.py
+-rw-r--r--   0        0        0     2654 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/slider.py
+-rw-r--r--   0        0        0     1297 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/spaceritem.py
+-rw-r--r--   0        0        0     1837 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/spinbox.py
+-rw-r--r--   0        0        0     1181 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/splashscreen.py
+-rw-r--r--   0        0        0     3920 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/splitter.py
+-rw-r--r--   0        0        0     1417 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/splitterhandle.py
+-rw-r--r--   0        0        0      983 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/stackedlayout.py
+-rw-r--r--   0        0        0     1372 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/stackedwidget.py
+-rw-r--r--   0        0        0     1677 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/statusbar.py
+-rw-r--r--   0        0        0    19383 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/style.py
+-rw-r--r--   0        0        0      208 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleditemdelegate.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/stylefactory.py
+-rw-r--r--   0        0        0      318 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoption.py
+-rw-r--r--   0        0        0      686 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionbutton.py
+-rw-r--r--   0        0        0      208 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptioncombobox.py
+-rw-r--r--   0        0        0      260 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptioncomplex.py
+-rw-r--r--   0        0        0      199 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiondockwidget.py
+-rw-r--r--   0        0        0      197 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionfocusrect.py
+-rw-r--r--   0        0        0      189 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionframe.py
+-rw-r--r--   0        0        0      209 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiongraphicsitem.py
+-rw-r--r--   0        0        0      197 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiongroupbox.py
+-rw-r--r--   0        0        0      911 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionheader.py
+-rw-r--r--   0        0        0     1032 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionmenuitem.py
+-rw-r--r--   0        0        0      201 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionprogressbar.py
+-rw-r--r--   0        0        0      199 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionrubberband.py
+-rw-r--r--   0        0        0      208 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionsizegrip.py
+-rw-r--r--   0        0        0     1046 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionslider.py
+-rw-r--r--   0        0        0      195 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionspinbox.py
+-rw-r--r--   0        0        0     1135 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontab.py
+-rw-r--r--   0        0        0      199 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontabbarbase.py
+-rw-r--r--   0        0        0      213 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontabwidgetframe.py
+-rw-r--r--   0        0        0      197 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontitlebar.py
+-rw-r--r--   0        0        0      397 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontoolbar.py
+-rw-r--r--   0        0        0     1176 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontoolbox.py
+-rw-r--r--   0        0        0      201 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptiontoolbutton.py
+-rw-r--r--   0        0        0     1344 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/styleoptionviewitem.py
+-rw-r--r--   0        0        0      397 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/stylepainter.py
+-rw-r--r--   0        0        0     1311 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/swipegesture.py
+-rw-r--r--   0        0        0     1732 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/systemtrayicon.py
+-rw-r--r--   0        0        0     5232 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tabbar.py
+-rw-r--r--   0        0        0     3112 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tableview.py
+-rw-r--r--   0        0        0     1085 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tablewidget.py
+-rw-r--r--   0        0        0     3334 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tablewidgetitem.py
+-rw-r--r--   0        0        0     1920 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tablewidgetselectionrange.py
+-rw-r--r--   0        0        0    10591 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tabwidget.py
+-rw-r--r--   0        0        0      392 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tapandholdgesture.py
+-rw-r--r--   0        0        0      371 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tapgesture.py
+-rw-r--r--   0        0        0     2400 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/textbrowser.py
+-rw-r--r--   0        0        0     6089 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/textedit.py
+-rw-r--r--   0        0        0     1526 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/timeedit.py
+-rw-r--r--   0        0        0     5008 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/toolbar.py
+-rw-r--r--   0        0        0     2568 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/toolbox.py
+-rw-r--r--   0        0        0     3175 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/toolbutton.py
+-rw-r--r--   0        0        0      710 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/tooltip.py
+-rw-r--r--   0        0        0     2532 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/treeview.py
+-rw-r--r--   0        0        0      630 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/treewidget.py
+-rw-r--r--   0        0        0     4841 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/treewidgetitem.py
+-rw-r--r--   0        0        0     4142 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/treewidgetitemiterator.py
+-rw-r--r--   0        0        0     1003 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/undoview.py
+-rw-r--r--   0        0        0      552 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/whatsthis.py
+-rw-r--r--   0        0        0    19395 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/widget.py
+-rw-r--r--   0        0        0      545 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/widgetaction.py
+-rw-r--r--   0        0        0      248 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/widgetitem.py
+-rw-r--r--   0        0        0     9052 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/wizard.py
+-rw-r--r--   0        0        0     1997 2023-04-12 17:01:45.996375 prettyqt-1.4.1/prettyqt/widgets/wizardpage.py
+-rw-r--r--   0        0        0     4492 2023-04-12 17:01:45.996375 prettyqt-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 prettyqt-1.4.1/PKG-INFO
```

### Comparing `prettyqt-1.3.0/LICENSE` & `prettyqt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/docs/index.md` & `prettyqt-1.4.1/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # prettyqt: Pythonic layer on top of PyQt5 / PyQt6 / PySide6
 [![PyPI Latest Release](https://img.shields.io/pypi/v/prettyqt.svg)](https://pypi.org/project/prettyqt/)
 [![Package Status](https://img.shields.io/pypi/status/prettyqt.svg)](https://pypi.org/project/prettyqt/)
 [![License](https://img.shields.io/pypi/l/prettyqt.svg)](https://github.com/phil65/PrettyQt/blob/master/LICENSE)
-[![Travis Build Status](https://travis-ci.org/phil65/prettyqt.svg?branch=master)](https://travis-ci.org/phil65/prettyqt)
 [![CodeCov](https://codecov.io/gh/phil65/PrettyQt/branch/master/graph/badge.svg)](https://codecov.io/gh/phil65/PrettyQt)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyUp](https://pyup.io/repos/github/phil65/PrettyQt/shield.svg)](https://pyup.io/repos/github/phil65/PrettyQt/)
 
 ## What is it?
 
 **PrettyQt** is a Python package that provides a pythonic layer on top of the GUI frameworks PyQt6 / PySide6.
```

### Comparing `prettyqt-1.3.0/prettyqt/__init__.py` & `prettyqt-1.4.1/prettyqt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for PrettyQt."""
 
 __author__ = """Philipp Temminghoff"""
 __email__ = "phil65@kodi.tv"
-__version__ = "1.3.0"
+__version__ = "1.4.1"
 
 
 def debug():
     """Print the local variables in the caller's frame."""
     import inspect
 
     frame = inspect.currentframe()
```

### Comparing `prettyqt-1.3.0/prettyqt/__pyinstaller/hook-prettyqt.py` & `prettyqt-1.4.1/prettyqt/__pyinstaller/hook-prettyqt.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/bluetooth/__init__.py` & `prettyqt-1.4.1/prettyqt/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py` & `prettyqt-1.4.1/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py` & `prettyqt-1.4.1/prettyqt/bluetooth/bluetoothservicediscoveryagent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/bluetooth/bluetoothserviceinfo.py` & `prettyqt-1.4.1/prettyqt/bluetooth/bluetoothserviceinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/bluetooth/bluetoothuuid.py` & `prettyqt-1.4.1/prettyqt/bluetooth/bluetoothuuid.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/__init__.py` & `prettyqt-1.4.1/prettyqt/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/abstractaxis.py` & `prettyqt-1.4.1/prettyqt/charts/abstractaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/abstractbarseries.py` & `prettyqt-1.4.1/prettyqt/charts/abstractbarseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/abstractseries.py` & `prettyqt-1.4.1/prettyqt/charts/abstractseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/barcategoryaxis.py` & `prettyqt-1.4.1/prettyqt/charts/barcategoryaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/barset.py` & `prettyqt-1.4.1/prettyqt/charts/barset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/boxset.py` & `prettyqt-1.4.1/prettyqt/charts/boxset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/candlestickset.py` & `prettyqt-1.4.1/prettyqt/charts/candlestickset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/categoryaxis.py` & `prettyqt-1.4.1/prettyqt/charts/categoryaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/chart.py` & `prettyqt-1.4.1/prettyqt/charts/chart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/chartview.py` & `prettyqt-1.4.1/prettyqt/charts/chartview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/legend.py` & `prettyqt-1.4.1/prettyqt/charts/legend.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/lineseries.py` & `prettyqt-1.4.1/prettyqt/charts/lineseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/pieslice.py` & `prettyqt-1.4.1/prettyqt/charts/pieslice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/polarchart.py` & `prettyqt-1.4.1/prettyqt/charts/polarchart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/valueaxis.py` & `prettyqt-1.4.1/prettyqt/charts/valueaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/charts/xyseries.py` & `prettyqt-1.4.1/prettyqt/charts/xyseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/__init__.py` & `prettyqt-1.4.1/prettyqt/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 from .runnable import Runnable
 
 # from .modelindex import ModelIndex
 from .threadpool import ThreadPool
 from .dir import Dir
 from .temporaryfile import TemporaryFile
 from .temporarydir import TemporaryDir
+from .keycombination import KeyCombination
 
 # from .event import Event
 from .itemselectionmodel import ItemSelectionModel
 from .itemselection import ItemSelection
 from .itemselectionrange import ItemSelectionRange
 from .diriterator import DirIterator
 from .abstractitemmodel import AbstractItemModel, AbstractItemModelMixin
@@ -253,14 +254,15 @@
     "Rect",
     "RectF",
     "MimeType",
     "MimeData",
     "MimeDatabase",
     "Dir",
     "TemporaryDir",
+    "KeyCombination",
     "DirIterator",
     "ItemSelectionModel",
     "ItemSelection",
     "ItemSelectionRange",
     "Slot",
     "Property",
     "RegularExpressionMatch",
```

### Comparing `prettyqt-1.3.0/prettyqt/core/_calendar.py` & `prettyqt-1.4.1/prettyqt/core/_calendar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/_datetime.py` & `prettyqt-1.4.1/prettyqt/core/_datetime.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/_locale.py` & `prettyqt-1.4.1/prettyqt/core/_locale.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/abstractanimation.py` & `prettyqt-1.4.1/prettyqt/core/abstractanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/abstractitemmodel.py` & `prettyqt-1.4.1/prettyqt/core/abstractitemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/animationgroup.py` & `prettyqt-1.4.1/prettyqt/core/animationgroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/basictimer.py` & `prettyqt-1.4.1/prettyqt/core/basictimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/collator.py` & `prettyqt-1.4.1/prettyqt/core/collator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/commandlineparser.py` & `prettyqt-1.4.1/prettyqt/core/commandlineparser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/coreapplication.py` & `prettyqt-1.4.1/prettyqt/core/coreapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/cryptographichash.py` & `prettyqt-1.4.1/prettyqt/core/cryptographichash.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/datastream.py` & `prettyqt-1.4.1/prettyqt/core/datastream.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/deadlinetimer.py` & `prettyqt-1.4.1/prettyqt/core/deadlinetimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/debug.py` & `prettyqt-1.4.1/prettyqt/core/debug.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/dir.py` & `prettyqt-1.4.1/prettyqt/core/dir.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/easingcurve.py` & `prettyqt-1.4.1/prettyqt/core/easingcurve.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/elapsedtimer.py` & `prettyqt-1.4.1/prettyqt/core/elapsedtimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/event.py` & `prettyqt-1.4.1/prettyqt/core/event.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/eventloop.py` & `prettyqt-1.4.1/prettyqt/core/eventloop.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/filedevice.py` & `prettyqt-1.4.1/prettyqt/core/filedevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/fileinfo.py` & `prettyqt-1.4.1/prettyqt/core/fileinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/fileselector.py` & `prettyqt-1.4.1/prettyqt/core/fileselector.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/filesystemwatcher.py` & `prettyqt-1.4.1/prettyqt/core/filesystemwatcher.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/iodevice.py` & `prettyqt-1.4.1/prettyqt/core/iodevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/itemselectionrange.py` & `prettyqt-1.4.1/prettyqt/core/itemselectionrange.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/jsondocument.py` & `prettyqt-1.4.1/prettyqt/core/jsondocument.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/jsonvalue.py` & `prettyqt-1.4.1/prettyqt/core/jsonvalue.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/library.py` & `prettyqt-1.4.1/prettyqt/core/library.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/libraryinfo.py` & `prettyqt-1.4.1/prettyqt/core/libraryinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/line.py` & `prettyqt-1.4.1/prettyqt/core/line.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/linef.py` & `prettyqt-1.4.1/prettyqt/core/linef.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/lockfile.py` & `prettyqt-1.4.1/prettyqt/core/lockfile.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/margins.py` & `prettyqt-1.4.1/prettyqt/core/margins.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/marginsf.py` & `prettyqt-1.4.1/prettyqt/core/marginsf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/metaenum.py` & `prettyqt-1.4.1/prettyqt/core/metaenum.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/metamethod.py` & `prettyqt-1.4.1/prettyqt/core/metamethod.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/metaobject.py` & `prettyqt-1.4.1/prettyqt/core/metaobject.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/metatype.py` & `prettyqt-1.4.1/prettyqt/core/metatype.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/mimedata.py` & `prettyqt-1.4.1/prettyqt/core/mimedata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/mimedatabase.py` & `prettyqt-1.4.1/prettyqt/core/mimedatabase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/object.py` & `prettyqt-1.4.1/prettyqt/core/object.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/operatingsystemversion.py` & `prettyqt-1.4.1/prettyqt/core/operatingsystemversion.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/pluginloader.py` & `prettyqt-1.4.1/prettyqt/core/pluginloader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/process.py` & `prettyqt-1.4.1/prettyqt/core/process.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/processenvironment.py` & `prettyqt-1.4.1/prettyqt/core/processenvironment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/propertyanimation.py` & `prettyqt-1.4.1/prettyqt/core/propertyanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/rect.py` & `prettyqt-1.4.1/prettyqt/core/rect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/regularexpression.py` & `prettyqt-1.4.1/prettyqt/core/regularexpression.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/regularexpressionmatch.py` & `prettyqt-1.4.1/prettyqt/core/regularexpressionmatch.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/regularexpressionmatchiterator.py` & `prettyqt-1.4.1/prettyqt/core/regularexpressionmatchiterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/resource.py` & `prettyqt-1.4.1/prettyqt/core/resource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/settings.py` & `prettyqt-1.4.1/prettyqt/core/settings.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/size.py` & `prettyqt-1.4.1/prettyqt/core/size.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/sizef.py` & `prettyqt-1.4.1/prettyqt/core/sizef.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/socketnotifier.py` & `prettyqt-1.4.1/prettyqt/core/socketnotifier.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/sortfilterproxymodel.py` & `prettyqt-1.4.1/prettyqt/core/sortfilterproxymodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/standardpaths.py` & `prettyqt-1.4.1/prettyqt/core/standardpaths.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/storageinfo.py` & `prettyqt-1.4.1/prettyqt/core/storageinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/temporarydir.py` & `prettyqt-1.4.1/prettyqt/core/temporarydir.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/textboundaryfinder.py` & `prettyqt-1.4.1/prettyqt/core/textboundaryfinder.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/textstream.py` & `prettyqt-1.4.1/prettyqt/core/textstream.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/timeline.py` & `prettyqt-1.4.1/prettyqt/core/timeline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/timer.py` & `prettyqt-1.4.1/prettyqt/core/timer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/timezone.py` & `prettyqt-1.4.1/prettyqt/core/timezone.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/translator.py` & `prettyqt-1.4.1/prettyqt/core/translator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/url.py` & `prettyqt-1.4.1/prettyqt/core/url.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/urlquery.py` & `prettyqt-1.4.1/prettyqt/core/urlquery.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/uuid.py` & `prettyqt-1.4.1/prettyqt/core/uuid.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/variantanimation.py` & `prettyqt-1.4.1/prettyqt/core/variantanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/versionnumber.py` & `prettyqt-1.4.1/prettyqt/core/versionnumber.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/core/xmlstreamreader.py` & `prettyqt-1.4.1/prettyqt/core/xmlstreamreader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_animations/bounceanimation.py` & `prettyqt-1.4.1/prettyqt/custom_animations/bounceanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_animations/fadeinanimation.py` & `prettyqt-1.4.1/prettyqt/custom_animations/fadeinanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_animations/slideanimation.py` & `prettyqt-1.4.1/prettyqt/custom_animations/slideanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/__init__.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/buttondelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/buttondelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/checkboxdelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/checkboxdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/icondelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/icondelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/nofocusdelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/nofocusdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/progressbardelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/progressbardelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/radiodelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/radiodelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/renderlinkdelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/renderlinkdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_delegates/stardelegate.py` & `prettyqt-1.4.1/prettyqt/custom_delegates/stardelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/__init__.py` & `prettyqt-1.4.1/prettyqt/custom_models/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/columnitemmodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/columnitemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/importlibdistributionmodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/importlibdistributionmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,30 +50,28 @@
             if orientation == constants.HORIZONTAL:
                 return self.HEADER[offset]
 
     def data(self, index, role=constants.DISPLAY_ROLE):
         if not index.isValid():
             return None
         dist = self.distributions[index.row()]
-        match role:
-            case constants.DISPLAY_ROLE:
-                match index.column():
-                    case 0:
-                        return dist.metadata["Name"]
-                    case 1:
-                        return dist.version
-                    case 2:
-                        return dist.metadata["Summary"]
-                    case 3:
-                        return dist.metadata["Home-Page"]
-                    case 4:
-                        return dist.metadata["Author"]
-                    case 5:
-                        return dist.metadata["License"]
-            case constants.USER_ROLE:
+        match role, index.column():
+            case constants.DISPLAY_ROLE, 0:
+                return dist.metadata["Name"]
+            case constants.DISPLAY_ROLE, 1:
+                return dist.version
+            case constants.DISPLAY_ROLE, 2:
+                return dist.metadata["Summary"]
+            case constants.DISPLAY_ROLE, 3:
+                return dist.metadata["Home-Page"]
+            case constants.DISPLAY_ROLE, 4:
+                return dist.metadata["Author"]
+            case constants.DISPLAY_ROLE, 5:
+                return dist.metadata["License"]
+            case constants.USER_ROLE, _:
                 return dist
 
     @classmethod
     def from_system(
         cls, parent: QtCore.QObject | None = None
     ) -> ImportlibDistributionModel:
         distributions = list_system_modules()
```

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/jsonmodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/jsonmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,29 +88,23 @@
         return True
 
     def data(self, index, role):
         if not index.isValid():
             return None
 
         item = index.internalPointer()
-        match role:
-            case constants.DISPLAY_ROLE | constants.EDIT_ROLE:
-                match index.column():
-                    case 0:
-                        return repr(item.key)
-                    case 1:
-                        if item.type in (dict, list, tuple):
-                            return ""
-                        else:
-                            if role == constants.DISPLAY_ROLE:
-                                return repr(item.value)
-                            else:
-                                return item.value
-                    case 2:
-                        return item.type.__name__
+        match role, index.column():
+            case constants.DISPLAY_ROLE | constants.EDIT_ROLE, 0:
+                return repr(item.key)
+            case constants.DISPLAY_ROLE, 1:
+                return "" if item.type in (dict, list, tuple) else repr(item.value)
+            case constants.EDIT_ROLE, 1:
+                return "" if item.type in (dict, list, tuple) else item.value
+            case constants.DISPLAY_ROLE | constants.EDIT_ROLE, 2:
+                return item.type.__name__
 
     def setData(self, index, value, role):
         if role == constants.EDIT_ROLE:
             if index.column() == 1:
                 item = index.internalPointer()
                 item.value = str(value)
                 self.update_row(index.row())
```

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/listmixin.py` & `prettyqt-1.4.1/prettyqt/custom_models/listmixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/modelmixin.py` & `prettyqt-1.4.1/prettyqt/custom_models/modelmixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/nesteditem.py` & `prettyqt-1.4.1/prettyqt/custom_models/nesteditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/nestedmodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/nestedmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/regexmatchesmodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/regexmatchesmodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,26 +21,25 @@
             if orientation == constants.HORIZONTAL:
                 return self.HEADER[section]
 
     def data(self, index, role):
         if not index.isValid():
             return None
         item = self.matches[index.row()]
-        if role in [constants.DISPLAY_ROLE]:
-            match index.column():
-                case 0:
-                    return str(item.span()[0])
-                case 1:
-                    return str(item.span()[1])
-                case 2:
-                    return repr(item.group())
-                case 3:
-                    return str(len(item.groups()))
-        if role in [constants.USER_ROLE]:
-            return item.span()
+        match role, index.column():
+            case constants.DISPLAY_ROLE, 0:
+                return str(item.span()[0])
+            case constants.DISPLAY_ROLE, 1:
+                return str(item.span()[1])
+            case constants.DISPLAY_ROLE, 2:
+                return repr(item.group())
+            case constants.DISPLAY_ROLE, 3:
+                return str(len(item.groups()))
+            case constants.USER_ROLE, _:
+                return item.span()
 
     def rowCount(self, parent=None):
         """Override for AbstractitemModel base method."""
         return len(self.matches)
 
 
 if __name__ == "__main__":
```

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/selectionmixin.py` & `prettyqt-1.4.1/prettyqt/custom_models/selectionmixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/storageinfomodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/storageinfomodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py` & `prettyqt-1.4.1/prettyqt/custom_models/subsequencesortfilterproxymodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/__init__.py` & `prettyqt-1.4.1/prettyqt/custom_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/compositevalidator.py` & `prettyqt-1.4.1/prettyqt/custom_validators/compositevalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/integervalidator.py` & `prettyqt-1.4.1/prettyqt/custom_validators/integervalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/notemptyvalidator.py` & `prettyqt-1.4.1/prettyqt/custom_validators/notemptyvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/notzerovalidator.py` & `prettyqt-1.4.1/prettyqt/custom_validators/notzerovalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/pathvalidator.py` & `prettyqt-1.4.1/prettyqt/custom_validators/pathvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/regexpatternvalidator.py` & `prettyqt-1.4.1/prettyqt/custom_validators/regexpatternvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_validators/regexvalidators.py` & `prettyqt-1.4.1/prettyqt/custom_validators/regexvalidators.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/__init__.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/booldicttoolbutton.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/booldicttoolbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/borderlayout.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/borderlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/codeeditor.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/collapsibleframe.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/collapsibleframe.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/colorchooserbutton.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/colorchooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/completionwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/completionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/dataset.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/dataset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/elidedlabel.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/elidedlabel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/expandableline.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/expandableline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/filechooserbutton.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/filechooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/flagselectionwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/flagselectionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/flowlayout.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/flowlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/fontchooserbutton.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/fontchooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/framelesswindow.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/framelesswindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/iconbrowser.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/iconbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/iconlabel.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/iconlabel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/iconwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/iconwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/image.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/image.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/imageviewer.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/imageviewer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/inputandslider.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/inputandslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/joystickbutton.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/joystickbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/labeledslider.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/labeledslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/listinput.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/listinput.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/logtextedit.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/logtextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/mappedcheckbox.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/mappedcheckbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/markdownwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/markdownwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/menurecentfiles.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/menurecentfiles.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/notification.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/notification.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/optionalwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/optionalwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/popupinfo.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/popupinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/quick_ref.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/quick_ref.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/ref.html` & `prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/ref.html`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/regexinput.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/regexinput.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/roundprogressbar.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/roundprogressbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/selectionwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/selectionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/sidebarwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/sidebarwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/singlelinetextedit.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/singlelinetextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/spanslider.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/spanslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/standardiconswidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/standardiconswidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/stringornumberwidget.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/stringornumberwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/subsequencecompleter.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/subsequencecompleter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/timeline.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/timeline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/custom_widgets/waitingspinner.py` & `prettyqt-1.4.1/prettyqt/custom_widgets/waitingspinner.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/eventfilters/animatedtooltipeventfilter.py` & `prettyqt-1.4.1/prettyqt/eventfilters/animatedtooltipeventfilter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/eventfilters/hovericoneventfilter.py` & `prettyqt-1.4.1/prettyqt/eventfilters/hovericoneventfilter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/__init__.py` & `prettyqt-1.4.1/prettyqt/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/abstractfileiconprovider.py` & `prettyqt-1.4.1/prettyqt/gui/abstractfileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/abstracttextdocumentlayout.py` & `prettyqt-1.4.1/prettyqt/gui/abstracttextdocumentlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/brush.py` & `prettyqt-1.4.1/prettyqt/gui/brush.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/clipboard.py` & `prettyqt-1.4.1/prettyqt/gui/clipboard.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/color.py` & `prettyqt-1.4.1/prettyqt/gui/color.py`

 * *Files 9% similar despite different names*

```diff
@@ -137,23 +137,45 @@
         out = out.convertTo(start.spec())
         return out
 
     def is_dark(self) -> bool:
         """Check whether a color is 'dark'."""
         return self.lightness() < 128
 
+    def get_spec(self) -> SpecStr:
+        return SPEC.inv[self.spec()]
+
+    def convert_to(self, spec: SpecStr) -> Color:
+        # return Color(self.convertTo(SPEC[spec]))
+        color = Color()
+        match spec:
+            case "rgb":
+                rgb = self.getRgb()
+                color.setRgb(*rgb)
+            case "hsv":
+                hsv = self.getHsv()
+                color.setHsv(*hsv)
+            case "cmyk":
+                cmyk = self.getCmyk()
+                color.setCmyk(*cmyk)
+            case "hsl":
+                hsl = self.getHsl()
+                color.setHsl(*hsl)
+            case "extended_rgb":
+                ergb = self.getRgbF()
+                color.setRgbF(*ergb)
+        return color
+
     def get_name(self, name_format: NameStr = "hex_argb") -> str:
         match name_format:
+            case "svg_rgb" | "svg_argb" if not self.isValid():
+                return 'fill=""'
             case "svg_rgb":
-                if not self.isValid():
-                    return 'fill=""'
                 return f'fill="rgb({self.red()}, {self.green()}, {self.blue()})"'
             case "svg_argb":
-                if not self.isValid():
-                    return 'fill=""'
                 fill_str = f"rgb({self.red()}, {self.green()}, {self.blue()})"
                 return f'fill="{fill_str}" fill-opacity="{self.alpha()}"'
             case "qcss_argb":
                 return (
                     f"rgba({self.red()}, {self.green()}, {self.blue()}, {self.alpha()})"
                 )
             case "qcss_rgb":
@@ -163,15 +185,15 @@
 
     @deprecated(reason="This method is deprecated, use Color.get_name instead.")
     def to_qsscolor(self) -> str:
         """Convert Color to a string that can be used in a QStyleSheet."""
         return f"rgba({self.red()}, {self.green()}, {self.blue()}, {self.alpha()})"
 
     def as_qt(self) -> QtGui.QColor:
-        return QtGui.QColor(self)
+        return self.convertTo(self.spec())
 
     def inverted(self, invert_alpha: bool = False) -> Color:
         return Color(
             255 - self.red(),
             255 - self.green(),
             255 - self.blue(),
             255 - self.alpha() if invert_alpha else self.alpha(),
@@ -191,7 +213,14 @@
         if base_color.lightness() > 128:
             return base_color.darker(factor)
         else:
             if base_color == Color("#000000"):
                 return cls.drift_color(cls("#101010"), factor + 20)
             else:
                 return base_color.lighter(factor + 10)
+
+
+if __name__ == "__main__":
+    color = Color()
+    color = color.convert_to("hsv")
+    print(color.get_spec())
+    print(color.as_qt())
```

### Comparing `prettyqt-1.3.0/prettyqt/gui/colorspace.py` & `prettyqt-1.4.1/prettyqt/gui/colorspace.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/cursor.py` & `prettyqt-1.4.1/prettyqt/gui/cursor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/doublevalidator.py` & `prettyqt-1.4.1/prettyqt/gui/doublevalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/drag.py` & `prettyqt-1.4.1/prettyqt/gui/drag.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/font.py` & `prettyqt-1.4.1/prettyqt/gui/font.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/fontdatabase.py` & `prettyqt-1.4.1/prettyqt/gui/fontdatabase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/fontmetrics.py` & `prettyqt-1.4.1/prettyqt/gui/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/fontmetricsf.py` & `prettyqt-1.4.1/prettyqt/gui/fontmetricsf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/gradient.py` & `prettyqt-1.4.1/prettyqt/gui/gradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/guiapplication.py` & `prettyqt-1.4.1/prettyqt/gui/guiapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/icon.py` & `prettyqt-1.4.1/prettyqt/gui/icon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/iconengine.py` & `prettyqt-1.4.1/prettyqt/gui/iconengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/image.py` & `prettyqt-1.4.1/prettyqt/gui/image.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/imageiohandler.py` & `prettyqt-1.4.1/prettyqt/gui/imageiohandler.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/imagereader.py` & `prettyqt-1.4.1/prettyqt/gui/imagereader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/imagewriter.py` & `prettyqt-1.4.1/prettyqt/gui/imagewriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/inputmethod.py` & `prettyqt-1.4.1/prettyqt/gui/inputmethod.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/intvalidator.py` & `prettyqt-1.4.1/prettyqt/gui/intvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/keysequence.py` & `prettyqt-1.4.1/prettyqt/gui/keysequence.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/lineargradient.py` & `prettyqt-1.4.1/prettyqt/gui/lineargradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/movie.py` & `prettyqt-1.4.1/prettyqt/gui/movie.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/pagelayout.py` & `prettyqt-1.4.1/prettyqt/gui/pagelayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/pagesize.py` & `prettyqt-1.4.1/prettyqt/gui/pagesize.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/paintdevice.py` & `prettyqt-1.4.1/prettyqt/gui/paintdevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/painter.py` & `prettyqt-1.4.1/prettyqt/gui/painter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/painterpath.py` & `prettyqt-1.4.1/prettyqt/gui/painterpath.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/painterpathstroker.py` & `prettyqt-1.4.1/prettyqt/gui/painterpathstroker.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/palette.py` & `prettyqt-1.4.1/prettyqt/gui/palette.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/pdfwriter.py` & `prettyqt-1.4.1/prettyqt/gui/pdfwriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/pen.py` & `prettyqt-1.4.1/prettyqt/gui/pen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/pixmap.py` & `prettyqt-1.4.1/prettyqt/gui/pixmap.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/pixmapcache.py` & `prettyqt-1.4.1/prettyqt/gui/pixmapcache.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/polygon.py` & `prettyqt-1.4.1/prettyqt/gui/polygon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/polygonf.py` & `prettyqt-1.4.1/prettyqt/gui/polygonf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/radialgradient.py` & `prettyqt-1.4.1/prettyqt/gui/radialgradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/region.py` & `prettyqt-1.4.1/prettyqt/gui/region.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/regularexpressionvalidator.py` & `prettyqt-1.4.1/prettyqt/gui/regularexpressionvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/screen.py` & `prettyqt-1.4.1/prettyqt/gui/screen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/sessionmanager.py` & `prettyqt-1.4.1/prettyqt/gui/sessionmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/standarditem.py` & `prettyqt-1.4.1/prettyqt/gui/standarditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/standarditemmodel.py` & `prettyqt-1.4.1/prettyqt/gui/standarditemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/statictext.py` & `prettyqt-1.4.1/prettyqt/gui/statictext.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/stylehints.py` & `prettyqt-1.4.1/prettyqt/gui/stylehints.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/surface.py` & `prettyqt-1.4.1/prettyqt/gui/surface.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/syntaxhighlighter.py` & `prettyqt-1.4.1/prettyqt/gui/syntaxhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textblock.py` & `prettyqt-1.4.1/prettyqt/gui/textblock.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textblockgroup.py` & `prettyqt-1.4.1/prettyqt/gui/textblockgroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textblockuserdata.py` & `prettyqt-1.4.1/prettyqt/gui/textblockuserdata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textcharformat.py` & `prettyqt-1.4.1/prettyqt/gui/textcharformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textcursor.py` & `prettyqt-1.4.1/prettyqt/gui/textcursor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textdocument.py` & `prettyqt-1.4.1/prettyqt/gui/textdocument.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textdocumentfragment.py` & `prettyqt-1.4.1/prettyqt/gui/textdocumentfragment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textdocumentwriter.py` & `prettyqt-1.4.1/prettyqt/gui/textdocumentwriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textformat.py` & `prettyqt-1.4.1/prettyqt/gui/textformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textframe.py` & `prettyqt-1.4.1/prettyqt/gui/textframe.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textframeformat.py` & `prettyqt-1.4.1/prettyqt/gui/textframeformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textlayout.py` & `prettyqt-1.4.1/prettyqt/gui/textlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textlength.py` & `prettyqt-1.4.1/prettyqt/gui/textlength.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textline.py` & `prettyqt-1.4.1/prettyqt/gui/textline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textlistformat.py` & `prettyqt-1.4.1/prettyqt/gui/textlistformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/textoption.py` & `prettyqt-1.4.1/prettyqt/gui/textoption.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/texttablecellformat.py` & `prettyqt-1.4.1/prettyqt/gui/texttablecellformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/transform.py` & `prettyqt-1.4.1/prettyqt/gui/transform.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,38 +35,33 @@
     def __reduce__(self):
         return type(self), (), self.__getstate__()
 
     def __setstate__(self, ba):
         core.DataStream.write_bytearray(ba, self)
 
     def __getitem__(self, value: tuple[int, int]) -> float:
-        if value[0] == 0:
-            match value[1]:
-                case 0:
-                    return self.m11()
-                case 1:
-                    return self.m12()
-                case 2:
-                    return self.m13()
-        elif value[0] == 1:
-            match value[1]:
-                case 0:
-                    return self.m21()
-                case 1:
-                    return self.m22()
-                case 2:
-                    return self.m23()
-        elif value[0] == 2:
-            match value[1]:
-                case 0:
-                    return self.m31()
-                case 1:
-                    return self.m32()
-                case 2:
-                    return self.m33()
+        match value[0], value[1]:
+            case 0, 0:
+                return self.m11()
+            case 0, 1:
+                return self.m12()
+            case 0, 2:
+                return self.m13()
+            case 1, 0:
+                return self.m21()
+            case 1, 1:
+                return self.m22()
+            case 1, 2:
+                return self.m23()
+            case 2, 0:
+                return self.m31()
+            case 2, 1:
+                return self.m32()
+            case 2, 2:
+                return self.m33()
         raise ValueError(f"Wrong value {value}")
 
     def __bytes__(self):
         ba = core.DataStream.create_bytearray(self)
         return bytes(ba)
 
     @classmethod
```

### Comparing `prettyqt-1.3.0/prettyqt/gui/undocommand.py` & `prettyqt-1.4.1/prettyqt/gui/undocommand.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/undostack.py` & `prettyqt-1.4.1/prettyqt/gui/undostack.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/validator.py` & `prettyqt-1.4.1/prettyqt/gui/validator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/vector3d.py` & `prettyqt-1.4.1/prettyqt/gui/vector3d.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/vector4d.py` & `prettyqt-1.4.1/prettyqt/gui/vector4d.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/gui/window.py` & `prettyqt-1.4.1/prettyqt/gui/window.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/__init__.py` & `prettyqt-1.4.1/prettyqt/iconprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/animation.py` & `prettyqt-1.4.1/prettyqt/iconprovider/animation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/awesomefileiconprovider.py` & `prettyqt-1.4.1/prettyqt/iconprovider/awesomefileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/awesomequickimageprovider.py` & `prettyqt-1.4.1/prettyqt/iconprovider/awesomequickimageprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/chariconengine.py` & `prettyqt-1.4.1/prettyqt/iconprovider/chariconengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/codicon-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/codicon-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/codicon.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/codicon.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/phosphor-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/phosphor-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/phosphor.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/phosphor.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/remixicon-charmap.json` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/remixicon-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/fonts/remixicon.ttf` & `prettyqt-1.4.1/prettyqt/iconprovider/fonts/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/iconic_font.py` & `prettyqt-1.4.1/prettyqt/iconprovider/iconic_font.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/iconprovider/svgbuffericonengine.py` & `prettyqt-1.4.1/prettyqt/iconprovider/svgbuffericonengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_ar.qm` & `prettyqt-1.4.1/prettyqt/localization/language_ar.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_bg.qm` & `prettyqt-1.4.1/prettyqt/localization/language_bg.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_ca.qm` & `prettyqt-1.4.1/prettyqt/localization/language_ca.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_cs.qm` & `prettyqt-1.4.1/prettyqt/localization/language_cs.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_da.qm` & `prettyqt-1.4.1/prettyqt/localization/language_da.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_de.qm` & `prettyqt-1.4.1/prettyqt/localization/language_de.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_es.qm` & `prettyqt-1.4.1/prettyqt/localization/language_es.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_fa.qm` & `prettyqt-1.4.1/prettyqt/localization/language_fa.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_fi.qm` & `prettyqt-1.4.1/prettyqt/localization/language_fi.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_fr.qm` & `prettyqt-1.4.1/prettyqt/localization/language_fr.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_gd.qm` & `prettyqt-1.4.1/prettyqt/localization/language_gd.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_gl.qm` & `prettyqt-1.4.1/prettyqt/localization/language_gl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_he.qm` & `prettyqt-1.4.1/prettyqt/localization/language_he.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_hu.qm` & `prettyqt-1.4.1/prettyqt/localization/language_hu.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_it.qm` & `prettyqt-1.4.1/prettyqt/localization/language_it.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_ja.qm` & `prettyqt-1.4.1/prettyqt/localization/language_ja.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_ko.qm` & `prettyqt-1.4.1/prettyqt/localization/language_ko.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_lt.qm` & `prettyqt-1.4.1/prettyqt/localization/language_lt.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_lv.qm` & `prettyqt-1.4.1/prettyqt/localization/language_lv.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_pl.qm` & `prettyqt-1.4.1/prettyqt/localization/language_pl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_pt.qm` & `prettyqt-1.4.1/prettyqt/localization/language_pt.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_ru.qm` & `prettyqt-1.4.1/prettyqt/localization/language_ru.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_sk.qm` & `prettyqt-1.4.1/prettyqt/localization/language_sk.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_sl.qm` & `prettyqt-1.4.1/prettyqt/localization/language_sl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_sv.qm` & `prettyqt-1.4.1/prettyqt/localization/language_sv.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_uk.qm` & `prettyqt-1.4.1/prettyqt/localization/language_uk.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_zh_CN.qm` & `prettyqt-1.4.1/prettyqt/localization/language_zh_CN.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/localization/language_zh_TW.qm` & `prettyqt-1.4.1/prettyqt/localization/language_zh_TW.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/__init__.py` & `prettyqt-1.4.1/prettyqt/location/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/geomaneuver.py` & `prettyqt-1.4.1/prettyqt/location/geomaneuver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/georoute.py` & `prettyqt-1.4.1/prettyqt/location/georoute.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/georouterequest.py` & `prettyqt-1.4.1/prettyqt/location/georouterequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/georoutesegment.py` & `prettyqt-1.4.1/prettyqt/location/georoutesegment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/georoutingmanager.py` & `prettyqt-1.4.1/prettyqt/location/georoutingmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/geoserviceprovider.py` & `prettyqt-1.4.1/prettyqt/location/geoserviceprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/place.py` & `prettyqt-1.4.1/prettyqt/location/place.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placeattribute.py` & `prettyqt-1.4.1/prettyqt/location/placeattribute.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placecategory.py` & `prettyqt-1.4.1/prettyqt/location/placecategory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placecontactdetail.py` & `prettyqt-1.4.1/prettyqt/location/placecontactdetail.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placecontent.py` & `prettyqt-1.4.1/prettyqt/location/placecontent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placecontentreply.py` & `prettyqt-1.4.1/prettyqt/location/placecontentreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placecontentrequest.py` & `prettyqt-1.4.1/prettyqt/location/placecontentrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placedetailsreply.py` & `prettyqt-1.4.1/prettyqt/location/placedetailsreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placeicon.py` & `prettyqt-1.4.1/prettyqt/location/placeicon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placeidreply.py` & `prettyqt-1.4.1/prettyqt/location/placeidreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placemanager.py` & `prettyqt-1.4.1/prettyqt/location/placemanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placematchreply.py` & `prettyqt-1.4.1/prettyqt/location/placematchreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placematchrequest.py` & `prettyqt-1.4.1/prettyqt/location/placematchrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placereply.py` & `prettyqt-1.4.1/prettyqt/location/placereply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placesearchreply.py` & `prettyqt-1.4.1/prettyqt/location/placesearchreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placesearchrequest.py` & `prettyqt-1.4.1/prettyqt/location/placesearchrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placesearchresult.py` & `prettyqt-1.4.1/prettyqt/location/placesearchresult.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/placesupplier.py` & `prettyqt-1.4.1/prettyqt/location/placesupplier.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/location/qlocation.py` & `prettyqt-1.4.1/prettyqt/location/qlocation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/multimediawidgets/graphicsvideoitem.py` & `prettyqt-1.4.1/prettyqt/multimediawidgets/graphicsvideoitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/multimediawidgets/videowidget.py` & `prettyqt-1.4.1/prettyqt/multimediawidgets/videowidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/__init__.py` & `prettyqt-1.4.1/prettyqt/network/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/abstractsocket.py` & `prettyqt-1.4.1/prettyqt/network/abstractsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/hostaddress.py` & `prettyqt-1.4.1/prettyqt/network/hostaddress.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/httpmultipart.py` & `prettyqt-1.4.1/prettyqt/network/httpmultipart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/httppart.py` & `prettyqt-1.4.1/prettyqt/network/httppart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/localserver.py` & `prettyqt-1.4.1/prettyqt/network/localserver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/localsocket.py` & `prettyqt-1.4.1/prettyqt/network/localsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkaccessmanager.py` & `prettyqt-1.4.1/prettyqt/network/networkaccessmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkaddressentry.py` & `prettyqt-1.4.1/prettyqt/network/networkaddressentry.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkcookie.py` & `prettyqt-1.4.1/prettyqt/network/networkcookie.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkcookiejar.py` & `prettyqt-1.4.1/prettyqt/network/networkcookiejar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkdatagram.py` & `prettyqt-1.4.1/prettyqt/network/networkdatagram.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkinterface.py` & `prettyqt-1.4.1/prettyqt/network/networkinterface.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkproxy.py` & `prettyqt-1.4.1/prettyqt/network/networkproxy.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/networkrequest.py` & `prettyqt-1.4.1/prettyqt/network/networkrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/tcpserver.py` & `prettyqt-1.4.1/prettyqt/network/tcpserver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/network/udpsocket.py` & `prettyqt-1.4.1/prettyqt/network/udpsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/objbrowser/attribute_model.py` & `prettyqt-1.4.1/prettyqt/objbrowser/attribute_model.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/objbrowser/objectbrowser.py` & `prettyqt-1.4.1/prettyqt/objbrowser/objectbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/objbrowser/objectbrowsertreemodel.py` & `prettyqt-1.4.1/prettyqt/objbrowser/objectbrowsertreemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,22 +262,18 @@
 
         # Object attributes
         for attr_name, attr_value in sorted(inspect.getmembers(obj)):
             obj_children.append((attr_name, attr_value))
             path_strings.append(f"{obj_path}.{attr_name}" if obj_path else attr_name)
             is_attr_list.append(True)
 
-        tree_items = []
-        for item, path_str, is_attr in zip(obj_children, path_strings, is_attr_list):
-            attr_name, attr_value = item
-            tree_item = ObjectBrowserTreeItem(
-                obj=attr_value, name=attr_name, obj_path=path_str, is_attribute=is_attr
-            )
-            tree_items.append(tree_item)
-
+        tree_items = [
+            ObjectBrowserTreeItem(obj=val, name=name, obj_path=p, is_attribute=is_attr)
+            for (name, val), p, is_attr in zip(obj_children, path_strings, is_attr_list)
+        ]
         return tree_items
 
     def _aux_refresh_tree(self, tree_index: core.ModelIndex):
         """Refresh the tree nodes recursively, auxiliary.
 
         If the underlying Python object has been changed, we don't want to delete the old
         tree model and create a new one from scratch because this loses all information
```

### Comparing `prettyqt-1.3.0/prettyqt/positioning/__init__.py` & `prettyqt-1.4.1/prettyqt/positioning/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geoareamonitorinfo.py` & `prettyqt-1.4.1/prettyqt/positioning/geoareamonitorinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geoareamonitorsource.py` & `prettyqt-1.4.1/prettyqt/positioning/geoareamonitorsource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geocircle.py` & `prettyqt-1.4.1/prettyqt/positioning/geocircle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geocoordinate.py` & `prettyqt-1.4.1/prettyqt/positioning/geocoordinate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geolocation.py` & `prettyqt-1.4.1/prettyqt/positioning/geolocation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geopath.py` & `prettyqt-1.4.1/prettyqt/positioning/geopath.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geopolygon.py` & `prettyqt-1.4.1/prettyqt/positioning/geopolygon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geopositioninfo.py` & `prettyqt-1.4.1/prettyqt/positioning/geopositioninfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geopositioninfosource.py` & `prettyqt-1.4.1/prettyqt/positioning/geopositioninfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/georectangle.py` & `prettyqt-1.4.1/prettyqt/positioning/georectangle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geosatelliteinfo.py` & `prettyqt-1.4.1/prettyqt/positioning/geosatelliteinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geosatelliteinfosource.py` & `prettyqt-1.4.1/prettyqt/positioning/geosatelliteinfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/geoshape.py` & `prettyqt-1.4.1/prettyqt/positioning/geoshape.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/positioning/nmeapositioninginfosource.py` & `prettyqt-1.4.1/prettyqt/positioning/nmeapositioninginfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/__init__.py` & `prettyqt-1.4.1/prettyqt/qml/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/jsengine.py` & `prettyqt-1.4.1/prettyqt/qml/jsengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/jsvalue.py` & `prettyqt-1.4.1/prettyqt/qml/jsvalue.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/qmlapplicationengine.py` & `prettyqt-1.4.1/prettyqt/qml/qmlapplicationengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/qmlcomponent.py` & `prettyqt-1.4.1/prettyqt/qml/qmlcomponent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/qmlengine.py` & `prettyqt-1.4.1/prettyqt/qml/qmlengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qml/qmlimageproviderbase.py` & `prettyqt-1.4.1/prettyqt/qml/qmlimageproviderbase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qt/QtCore/__init__.py` & `prettyqt-1.4.1/prettyqt/qt/QtCore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qt/QtGui/__init__.py` & `prettyqt-1.4.1/prettyqt/qt/QtGui/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qt/__init__.py` & `prettyqt-1.4.1/prettyqt/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/qthelp/__init__.py` & `prettyqt-1.4.1/prettyqt/qthelp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """qthelp module.
 
 contains QtHelp-based classes
 """
 
 from .helpindexmodel import HelpIndexModel
+from .helpfilterdata import HelpFilterData
 from .helpcontentitem import HelpContentItem
 from .helpsearchresult import HelpSearchResult
 from .helpcontentmodel import HelpContentModel
 from .helpcontentwidget import HelpContentWidget
 from .helpindexwidget import HelpIndexWidget
 from .helpsearchresultwidget import HelpSearchResultWidget
 from .helpsearchquerywidget import HelpSearchQueryWidget
 from .helpenginecore import HelpEngineCore, HelpEngineCoreMixin
 from .helpengine import HelpEngine
 from .helpsearchengine import HelpSearchEngine
 from .helpfilterengine import HelpFilterEngine
 
 __all__ = [
     "HelpIndexModel",
+    "HelpFilterData",
     "HelpContentItem",
     "HelpSearchResult",
     "HelpContentModel",
     "HelpContentWidget",
     "HelpIndexWidget",
     "HelpSearchEngine",
     "HelpSearchResultWidget",
```

### Comparing `prettyqt-1.3.0/prettyqt/qthelp/helpenginecore.py` & `prettyqt-1.4.1/prettyqt/qthelp/helpenginecore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from prettyqt import core
+from prettyqt import core, qthelp
 from prettyqt.qt import QtCore, QtHelp
 from prettyqt.utils import types
 
 
 class HelpEngineCoreMixin(core.ObjectMixin):
     def get_file_data(self, url: QtCore.QUrl) -> bytes:
         return bytes(self.fileData(url))
@@ -22,14 +22,17 @@
         ]
 
     def find_file(self, url: types.UrlType) -> core.Url:
         if not isinstance(url, QtCore.QUrl):
             url = QtCore.QUrl(url)
         return core.Url(self.findFile(url))
 
+    def get_filter_engine(self) -> qthelp.HelpFilterEngine:
+        return qthelp.HelpFilterEngine(self.filterEngine())
+
 
 class HelpEngineCore(HelpEngineCoreMixin, QtHelp.QHelpEngineCore):
     pass
 
 
 if __name__ == "__main__":
     engine = HelpEngineCore("")
```

### Comparing `prettyqt-1.3.0/prettyqt/qtre.py` & `prettyqt-1.4.1/prettyqt/qtre.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/quick/__init__.py` & `prettyqt-1.4.1/prettyqt/quick/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/quick/quickitem.py` & `prettyqt-1.4.1/prettyqt/quick/quickitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/quick/quickitemgrabresult.py` & `prettyqt-1.4.1/prettyqt/quick/quickitemgrabresult.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/quick/quickpainteditem.py` & `prettyqt-1.4.1/prettyqt/quick/quickpainteditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/quick/quickview.py` & `prettyqt-1.4.1/prettyqt/quick/quickview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/quick/quickwindow.py` & `prettyqt-1.4.1/prettyqt/quick/quickwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/scintilla/sciscintilla.py` & `prettyqt-1.4.1/prettyqt/scintilla/sciscintilla.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/statemachine/__init__.py` & `prettyqt-1.4.1/prettyqt/statemachine/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/statemachine/abstracttransition.py` & `prettyqt-1.4.1/prettyqt/statemachine/abstracttransition.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/statemachine/historystate.py` & `prettyqt-1.4.1/prettyqt/statemachine/historystate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/statemachine/state.py` & `prettyqt-1.4.1/prettyqt/statemachine/state.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/statemachine/statemachine.py` & `prettyqt-1.4.1/prettyqt/statemachine/statemachine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/svg/svgrenderer.py` & `prettyqt-1.4.1/prettyqt/svg/svgrenderer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/__init__.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/highlightrule.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/highlightrule.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/jsonhighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/jsonhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/markdownhighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/markdownhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/pygmentshighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/pythonhighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/pythonhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/regexmatchhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/xmlhighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/xmlhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/syntaxhighlighters/yamlhighlighter.py` & `prettyqt-1.4.1/prettyqt/syntaxhighlighters/yamlhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/texttospeech/texttospeech.py` & `prettyqt-1.4.1/prettyqt/texttospeech/texttospeech.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/texttospeech/voice.py` & `prettyqt-1.4.1/prettyqt/texttospeech/voice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/themes/darktheme.qss` & `prettyqt-1.4.1/prettyqt/themes/darktheme.qss`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/__init__.py` & `prettyqt-1.4.1/prettyqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/autoslot.py` & `prettyqt-1.4.1/prettyqt/utils/autoslot.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/colors.py` & `prettyqt-1.4.1/prettyqt/utils/colors.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/debugging.py` & `prettyqt-1.4.1/prettyqt/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/helpers.py` & `prettyqt-1.4.1/prettyqt/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/mappers.py` & `prettyqt-1.4.1/prettyqt/utils/mappers.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/prettyprinter.py` & `prettyqt-1.4.1/prettyqt/utils/prettyprinter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/searchandreplacemixin.py` & `prettyqt-1.4.1/prettyqt/utils/searchandreplacemixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/signallogger.py` & `prettyqt-1.4.1/prettyqt/utils/signallogger.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/singleapplication.py` & `prettyqt-1.4.1/prettyqt/utils/singleapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/syncedproperty.py` & `prettyqt-1.4.1/prettyqt/utils/syncedproperty.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/treeitem.py` & `prettyqt-1.4.1/prettyqt/utils/treeitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/utils/types.py` & `prettyqt-1.4.1/prettyqt/utils/types.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/__init__.py` & `prettyqt-1.4.1/prettyqt/webenginecore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginecontextmenurequest.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginecontextmenurequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginedownloadrequest.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginedownloadrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginehistory.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginehistory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginehttprequest.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginehttprequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginepage.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginepage.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webengineprofile.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webengineprofile.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginescript.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginescript.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginescriptcollection.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginescriptcollection.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webenginesettings.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webenginesettings.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginecore/webengineurlscheme.py` & `prettyqt-1.4.1/prettyqt/webenginecore/webengineurlscheme.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/webenginewidgets/webengineview.py` & `prettyqt-1.4.1/prettyqt/webenginewidgets/webengineview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/__init__.py` & `prettyqt-1.4.1/prettyqt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/abstractbutton.py` & `prettyqt-1.4.1/prettyqt/widgets/abstractbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/abstractitemview.py` & `prettyqt-1.4.1/prettyqt/widgets/abstractitemview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/abstractscrollarea.py` & `prettyqt-1.4.1/prettyqt/widgets/abstractscrollarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/abstractslider.py` & `prettyqt-1.4.1/prettyqt/widgets/abstractslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/abstractspinbox.py` & `prettyqt-1.4.1/prettyqt/widgets/abstractspinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/action.py` & `prettyqt-1.4.1/prettyqt/widgets/action.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/actiongroup.py` & `prettyqt-1.4.1/prettyqt/widgets/actiongroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/application.py` & `prettyqt-1.4.1/prettyqt/widgets/application.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/boxlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/boxlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/calendarwidget.py` & `prettyqt-1.4.1/prettyqt/widgets/calendarwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/checkbox.py` & `prettyqt-1.4.1/prettyqt/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/colordialog.py` & `prettyqt-1.4.1/prettyqt/widgets/colordialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/combobox.py` & `prettyqt-1.4.1/prettyqt/widgets/combobox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/completer.py` & `prettyqt-1.4.1/prettyqt/widgets/completer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/datawidgetmapper.py` & `prettyqt-1.4.1/prettyqt/widgets/datawidgetmapper.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/dateedit.py` & `prettyqt-1.4.1/prettyqt/widgets/dateedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/datetimeedit.py` & `prettyqt-1.4.1/prettyqt/widgets/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/dial.py` & `prettyqt-1.4.1/prettyqt/widgets/dial.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/dialog.py` & `prettyqt-1.4.1/prettyqt/widgets/dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from prettyqt import qt, widgets
+from prettyqt import widgets
 from prettyqt.qt import QtCore, QtWidgets
 from prettyqt.utils import types
 
 
 class DialogMixin(widgets.WidgetMixin):
     def __init__(
         self,
@@ -43,20 +43,23 @@
         self.resize(*state["size"])
         self.setSizeGripEnabled(state["size_grip_enabled"])
 
     def __reduce__(self):
         return type(self), (), self.__getstate__()
 
     def keyPressEvent(self, e):
-        if e.key() == QtCore.Qt.Key.Key_Escape:
-            self.close()
-        elif e.key() == QtCore.Qt.Key.Key_F11:
-            self.showNormal() if self.isMaximized() else self.showMaximized()
-        else:
-            super().keyPressEvent(e)
+        match e.key():
+            case QtCore.Qt.Key.Key_Escape:
+                self.close()
+            case QtCore.Qt.Key.Key_F11 if self.isMaximized():
+                self.showNormal()
+            case QtCore.Qt.Key.Key_F11:
+                self.showMaximized()
+            case _:
+                super().keyPressEvent(e)
 
     def delete_on_close(self):
         self.setAttribute(QtCore.Qt.WidgetAttribute.WA_DeleteOnClose)
 
     def add_widget(self, widget: QtWidgets.QWidget) -> QtWidgets.QWidget:
         self.box += widget
         return widget
@@ -70,18 +73,15 @@
         self.show()
         return bool(self.main_loop())
 
     def is_accepted(self) -> bool:
         return self.result() == QtWidgets.QDialog.DialogCode.Accepted
 
     def main_loop(self) -> int:
-        if qt.API.startswith("pyqt"):
-            return self.exec()
-        else:
-            return self.exec_()
+        return self.exec_()
 
 
 class Dialog(DialogMixin, QtWidgets.QDialog):
     pass
 
 
 if __name__ == "__main__":
```

### Comparing `prettyqt-1.3.0/prettyqt/widgets/dialogbuttonbox.py` & `prettyqt-1.4.1/prettyqt/widgets/dialogbuttonbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/dockwidget.py` & `prettyqt-1.4.1/prettyqt/widgets/dockwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/doublespinbox.py` & `prettyqt-1.4.1/prettyqt/widgets/doublespinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/filedialog.py` & `prettyqt-1.4.1/prettyqt/widgets/filedialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/fileiconprovider.py` & `prettyqt-1.4.1/prettyqt/widgets/fileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/filesystemmodel.py` & `prettyqt-1.4.1/prettyqt/widgets/filesystemmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,24 +54,25 @@
     def watch_for_changes(self, watch: bool):
         self.setOption(OPTIONS["dont_watch_changes"], not watch)
 
     def use_custom_icons(self, use: bool):
         self.setOption(OPTIONS["no_custom_icons"], not use)
 
     def set_root_path(self, path: types.PathType) -> QtCore.QModelIndex:
-        path = os.fspath(path)
         match path:
             case "/" | "root":
                 path = core.Dir.rootPath()
             case "home":
                 path = core.Dir.homePath()
             case "temp":
                 path = core.Dir.tempPath()
             case "current":
                 path = core.Dir.currentPath()
+            case _:
+                path = os.fspath(path)
         return self.setRootPath(path)
 
     def set_name_filters(self, filters, hide: bool = False):
         self.setNameFilters(filters)
         self.setNameFilterDisables(not hide)
 
     def set_filter(self, filter_mode: core.dir.FilterStr):
```

### Comparing `prettyqt-1.3.0/prettyqt/widgets/fontcombobox.py` & `prettyqt-1.4.1/prettyqt/widgets/fontcombobox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/formlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/formlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/frame.py` & `prettyqt-1.4.1/prettyqt/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/gesture.py` & `prettyqt-1.4.1/prettyqt/widgets/gesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsanchorlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsanchorlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsblureffect.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsblureffect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsellipseitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsellipseitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsgridlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsgridlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicslayout.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicslayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicslinearlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicslinearlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicslineitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicslineitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsobject.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsobject.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsopacityeffect.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsopacityeffect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicspixmapitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicspixmapitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicspolygonitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicspolygonitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsrectitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsrectitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsrotation.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsrotation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsscene.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsscene.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicstextitem.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicstextitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicsview.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicsview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/graphicswidget.py` & `prettyqt-1.4.1/prettyqt/widgets/graphicswidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/gridlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/gridlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/groupbox.py` & `prettyqt-1.4.1/prettyqt/widgets/groupbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/headerview.py` & `prettyqt-1.4.1/prettyqt/widgets/headerview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/inputdialog.py` & `prettyqt-1.4.1/prettyqt/widgets/inputdialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/itemeditorfactory.py` & `prettyqt-1.4.1/prettyqt/widgets/itemeditorfactory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/keysequenceedit.py` & `prettyqt-1.4.1/prettyqt/widgets/keysequenceedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/label.py` & `prettyqt-1.4.1/prettyqt/widgets/label.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/layout.py` & `prettyqt-1.4.1/prettyqt/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/layoutitem.py` & `prettyqt-1.4.1/prettyqt/widgets/layoutitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/lcdnumber.py` & `prettyqt-1.4.1/prettyqt/widgets/lcdnumber.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/lineedit.py` & `prettyqt-1.4.1/prettyqt/widgets/lineedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,17 @@
         )
 
     def focusOutEvent(self, event):
         self.focusLost.emit()
         return super().focusOutEvent(event)
 
     def keyPressEvent(self, event):
-        if event.key() in [QtCore.Qt.Key.Key_Enter, QtCore.Qt.Key.Key_Return]:
-            self.enterPressed.emit()
+        match event.key():
+            case QtCore.Qt.Key.Key_Enter | QtCore.Qt.Key.Key_Return:
+                self.enterPressed.emit()
         return super().keyPressEvent(event)
 
     def _on_edit_complete(self):
         self.editComplete.emit(self.text())
 
     def font(self) -> gui.Font:
         return gui.Font(super().font())
```

### Comparing `prettyqt-1.3.0/prettyqt/widgets/listview.py` & `prettyqt-1.4.1/prettyqt/widgets/listview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/listwidget.py` & `prettyqt-1.4.1/prettyqt/widgets/listwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/listwidgetitem.py` & `prettyqt-1.4.1/prettyqt/widgets/listwidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/mainwindow.py` & `prettyqt-1.4.1/prettyqt/widgets/mainwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/mdiarea.py` & `prettyqt-1.4.1/prettyqt/widgets/mdiarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/mdisubwindow.py` & `prettyqt-1.4.1/prettyqt/widgets/mdisubwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/menu.py` & `prettyqt-1.4.1/prettyqt/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/menubar.py` & `prettyqt-1.4.1/prettyqt/widgets/menubar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/messagebox.py` & `prettyqt-1.4.1/prettyqt/widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/pangesture.py` & `prettyqt-1.4.1/prettyqt/widgets/pangesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/pinchgesture.py` & `prettyqt-1.4.1/prettyqt/widgets/pinchgesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/plaintextedit.py` & `prettyqt-1.4.1/prettyqt/widgets/plaintextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/progressbar.py` & `prettyqt-1.4.1/prettyqt/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/progressdialog.py` & `prettyqt-1.4.1/prettyqt/widgets/progressdialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/pushbutton.py` & `prettyqt-1.4.1/prettyqt/widgets/pushbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/radiobutton.py` & `prettyqt-1.4.1/prettyqt/widgets/radiobutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/rubberband.py` & `prettyqt-1.4.1/prettyqt/widgets/rubberband.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/scrollarea.py` & `prettyqt-1.4.1/prettyqt/widgets/scrollarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/scrollbar.py` & `prettyqt-1.4.1/prettyqt/widgets/scrollbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/scroller.py` & `prettyqt-1.4.1/prettyqt/widgets/scroller.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/scrollerproperties.py` & `prettyqt-1.4.1/prettyqt/widgets/scrollerproperties.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/shortcut.py` & `prettyqt-1.4.1/prettyqt/widgets/shortcut.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/sizepolicy.py` & `prettyqt-1.4.1/prettyqt/widgets/sizepolicy.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/slider.py` & `prettyqt-1.4.1/prettyqt/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/spaceritem.py` & `prettyqt-1.4.1/prettyqt/widgets/spaceritem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/spinbox.py` & `prettyqt-1.4.1/prettyqt/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/splashscreen.py` & `prettyqt-1.4.1/prettyqt/widgets/splashscreen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/splitter.py` & `prettyqt-1.4.1/prettyqt/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/splitterhandle.py` & `prettyqt-1.4.1/prettyqt/widgets/splitterhandle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/stackedlayout.py` & `prettyqt-1.4.1/prettyqt/widgets/stackedlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/stackedwidget.py` & `prettyqt-1.4.1/prettyqt/widgets/stackedwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/statusbar.py` & `prettyqt-1.4.1/prettyqt/widgets/statusbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/style.py` & `prettyqt-1.4.1/prettyqt/widgets/style.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptionbutton.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptionbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptionheader.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptionheader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptionmenuitem.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptionmenuitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptionslider.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptionslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptiontab.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptiontab.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptiontoolbox.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptiontoolbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/styleoptionviewitem.py` & `prettyqt-1.4.1/prettyqt/widgets/styleoptionviewitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/swipegesture.py` & `prettyqt-1.4.1/prettyqt/widgets/swipegesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/systemtrayicon.py` & `prettyqt-1.4.1/prettyqt/widgets/systemtrayicon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tabbar.py` & `prettyqt-1.4.1/prettyqt/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tableview.py` & `prettyqt-1.4.1/prettyqt/widgets/tableview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tablewidget.py` & `prettyqt-1.4.1/prettyqt/widgets/tablewidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tablewidgetitem.py` & `prettyqt-1.4.1/prettyqt/widgets/tablewidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tablewidgetselectionrange.py` & `prettyqt-1.4.1/prettyqt/widgets/tablewidgetselectionrange.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tabwidget.py` & `prettyqt-1.4.1/prettyqt/widgets/tabwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/textbrowser.py` & `prettyqt-1.4.1/prettyqt/widgets/textbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/textedit.py` & `prettyqt-1.4.1/prettyqt/widgets/textedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/timeedit.py` & `prettyqt-1.4.1/prettyqt/widgets/timeedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/toolbar.py` & `prettyqt-1.4.1/prettyqt/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/toolbox.py` & `prettyqt-1.4.1/prettyqt/widgets/toolbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/toolbutton.py` & `prettyqt-1.4.1/prettyqt/widgets/toolbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/tooltip.py` & `prettyqt-1.4.1/prettyqt/widgets/tooltip.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/treeview.py` & `prettyqt-1.4.1/prettyqt/widgets/treeview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/treewidget.py` & `prettyqt-1.4.1/prettyqt/widgets/treewidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/treewidgetitem.py` & `prettyqt-1.4.1/prettyqt/widgets/treewidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/treewidgetitemiterator.py` & `prettyqt-1.4.1/prettyqt/widgets/treewidgetitemiterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/undoview.py` & `prettyqt-1.4.1/prettyqt/widgets/undoview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/whatsthis.py` & `prettyqt-1.4.1/prettyqt/widgets/whatsthis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/widget.py` & `prettyqt-1.4.1/prettyqt/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/widgetaction.py` & `prettyqt-1.4.1/prettyqt/widgets/widgetaction.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/wizard.py` & `prettyqt-1.4.1/prettyqt/widgets/wizard.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/prettyqt/widgets/wizardpage.py` & `prettyqt-1.4.1/prettyqt/widgets/wizardpage.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.3.0/pyproject.toml` & `prettyqt-1.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PrettyQt"
-version = "1.3.0"
+version = "1.4.1"
 description = "A pythonic layer on top of PyQt6 / PySide6"
 readme = 'docs/index.md'
 repository = "https://github.com/phil65/prettyqt"
 homepage = "https://github.com/phil65/prettyqt"
 authors = ["phil65 <philipptemminghoff@googlemail.com>"]
 packages = [
     { include = "prettyqt" },
@@ -48,15 +48,14 @@
 pytest-qt = {version = "^4.1"}
 mypy = "^1"
 types-Deprecated = "^1.2"
 types-docutils = "^0"
 types-orjson = "^3.6"
 pylint = "^2.5"
 pytest-xvfb = {version = "^2", markers = "sys_platform == 'linux'"}
-codecov = "^2.1"
 coverage = "^7"
 mkdocs = "^1"
 mkdocs-material = "^9"
 mkdocstrings = {version = "^0", extras = ["python-legacy"]}
 
 pymdown-extensions = "^9"
 black = "^23"
@@ -177,15 +176,15 @@
   | build
   | dist
   | tests/.*/setup.py
 )/
 '''
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.3.0"
+version = "1.4.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_start_rev = "v0.100.0"
 changelog_file = "docs/changelog.md"
 version_files = [
     "prettyqt/__init__.py:__version__",
     "pyproject.toml:version",
```

### Comparing `prettyqt-1.3.0/PKG-INFO` & `prettyqt-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyqt
-Version: 1.3.0
+Version: 1.4.1
 Summary: A pythonic layer on top of PyQt6 / PySide6
 Home-page: https://github.com/phil65/prettyqt
 Author: phil65
 Author-email: philipptemminghoff@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -30,15 +30,14 @@
 Project-URL: Repository, https://github.com/phil65/prettyqt
 Description-Content-Type: text/markdown
 
 # prettyqt: Pythonic layer on top of PyQt5 / PyQt6 / PySide6
 [![PyPI Latest Release](https://img.shields.io/pypi/v/prettyqt.svg)](https://pypi.org/project/prettyqt/)
 [![Package Status](https://img.shields.io/pypi/status/prettyqt.svg)](https://pypi.org/project/prettyqt/)
 [![License](https://img.shields.io/pypi/l/prettyqt.svg)](https://github.com/phil65/PrettyQt/blob/master/LICENSE)
-[![Travis Build Status](https://travis-ci.org/phil65/prettyqt.svg?branch=master)](https://travis-ci.org/phil65/prettyqt)
 [![CodeCov](https://codecov.io/gh/phil65/PrettyQt/branch/master/graph/badge.svg)](https://codecov.io/gh/phil65/PrettyQt)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyUp](https://pyup.io/repos/github/phil65/PrettyQt/shield.svg)](https://pyup.io/repos/github/phil65/PrettyQt/)
 
 ## What is it?
 
 **PrettyQt** is a Python package that provides a pythonic layer on top of the GUI frameworks PyQt6 / PySide6.
```

