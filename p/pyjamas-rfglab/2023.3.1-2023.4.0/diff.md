# Comparing `tmp/pyjamas_rfglab-2023.3.1-py3-none-any.whl.zip` & `tmp/pyjamas_rfglab-2023.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,76 +1,83 @@
-Zip file size: 529355 bytes, number of entries: 74
+Zip file size: 549307 bytes, number of entries: 81
 -rw-r--r--  2.0 unx    33144 b- defN 20-Feb-04 05:51 pyjamas/LICENSE
 -rw-r--r--  2.0 unx     1088 b- defN 20-Jan-17 04:15 pyjamas/__init__.py
 -rw-r--r--  2.0 unx     1793 b- defN 21-Aug-22 22:40 pyjamas/dragdropmainwindow.py
 -rw-r--r--  2.0 unx     4901 b- defN 23-Jan-22 21:23 pyjamas/orthogonalviewswindow.py
--rw-r--r--  2.0 unx    51991 b- defN 23-Mar-16 21:08 pyjamas/pjscore.py
--rw-r--r--  2.0 unx    32618 b- defN 23-Mar-14 22:07 pyjamas/pjseventfilter.py
+-rw-r--r--  2.0 unx    52550 b- defN 23-Apr-12 16:42 pyjamas/pjscore.py
+-rw-r--r--  2.0 unx    32616 b- defN 23-Apr-12 16:40 pyjamas/pjseventfilter.py
 -rw-r--r--  2.0 unx     2123 b- defN 20-Feb-19 06:14 pyjamas/pjsthreads.py
 -rw-r--r--  2.0 unx  2950623 b- defN 20-Jan-17 04:15 pyjamas/pyjamas.tif
 -rw-r--r--  2.0 unx    26659 b- defN 22-Nov-12 20:45 pyjamas/rutils.py
--rw-r--r--  2.0 unx     1586 b- defN 22-Apr-19 02:31 pyjamas/dialogs/__init__.py
+-rw-r--r--  2.0 unx     1645 b- defN 23-Apr-12 16:40 pyjamas/dialogs/__init__.py
 -rw-r--r--  2.0 unx    17513 b- defN 20-Jul-11 20:07 pyjamas/dialogs/adjustcontrast.py
 -rw-r--r--  2.0 unx    28797 b- defN 22-Oct-11 19:50 pyjamas/dialogs/batchanalysis.py
 -rw-r--r--  2.0 unx     5453 b- defN 23-Feb-19 02:47 pyjamas/dialogs/batchprojectconcat.py
+-rw-r--r--  2.0 unx     6858 b- defN 23-Apr-12 16:40 pyjamas/dialogs/batchresize.py
 -rw-r--r--  2.0 unx     2980 b- defN 21-Oct-30 00:59 pyjamas/dialogs/classifierdialogABC.py
+-rw-r--r--  2.0 unx     3143 b- defN 23-Apr-12 16:40 pyjamas/dialogs/classifiertype.py
 -rw-r--r--  2.0 unx     6381 b- defN 23-Feb-19 02:47 pyjamas/dialogs/expandnpropagateseeds.py
 -rw-r--r--  2.0 unx     5171 b- defN 21-Oct-31 01:33 pyjamas/dialogs/expandseeds.py
 -rw-r--r--  2.0 unx    12944 b- defN 22-Apr-23 19:28 pyjamas/dialogs/findseeds.py
 -rw-r--r--  2.0 unx    11319 b- defN 21-Oct-30 00:56 pyjamas/dialogs/logregression.py
 -rw-r--r--  2.0 unx     3432 b- defN 21-Oct-30 00:59 pyjamas/dialogs/matplotlibdialog.py
 -rw-r--r--  2.0 unx     8762 b- defN 21-Oct-31 01:33 pyjamas/dialogs/measurepoly.py
 -rw-r--r--  2.0 unx    13235 b- defN 23-Feb-19 02:47 pyjamas/dialogs/neuralnet.py
 -rw-r--r--  2.0 unx     8642 b- defN 23-Feb-19 02:47 pyjamas/dialogs/nonmax_suppr.py
 -rw-r--r--  2.0 unx     5477 b- defN 23-Feb-19 02:47 pyjamas/dialogs/propagateseeds.py
+-rw-r--r--  2.0 unx    14546 b- defN 23-Apr-12 16:40 pyjamas/dialogs/rescuneuralnet.py
 -rw-r--r--  2.0 unx    12468 b- defN 21-Oct-30 01:12 pyjamas/dialogs/svm.py
 -rw-r--r--  2.0 unx     2233 b- defN 20-May-13 06:00 pyjamas/dialogs/textdialog.py
 -rw-r--r--  2.0 unx     4026 b- defN 21-Oct-30 01:12 pyjamas/dialogs/timepoints.py
 -rw-r--r--  2.0 unx      899 b- defN 21-May-09 22:07 pyjamas/external/__init__.py
 -rw-r--r--  2.0 unx     6852 b- defN 20-Jul-11 20:09 pyjamas/external/pascal_voc_io.py
 -rw-r--r--  2.0 unx      924 b- defN 22-Jun-20 21:44 pyjamas/rannotations/__init__.py
 -rw-r--r--  2.0 unx      856 b- defN 20-Jan-17 04:15 pyjamas/rannotations/rannotation.py
 -rw-r--r--  2.0 unx    16818 b- defN 23-Jan-29 04:49 pyjamas/rannotations/rpolyline.py
 -rw-r--r--  2.0 unx     2288 b- defN 22-Aug-14 20:59 pyjamas/rannotations/rvector2d.py
 -rw-r--r--  2.0 unx     1257 b- defN 20-Jan-17 04:15 pyjamas/rcallbacks/__init__.py
 -rw-r--r--  2.0 unx     7696 b- defN 22-Nov-14 19:12 pyjamas/rcallbacks/rcallback.py
 -rw-r--r--  2.0 unx     1658 b- defN 23-Feb-07 15:13 pyjamas/rcallbacks/rcbabout.py
 -rw-r--r--  2.0 unx    13560 b- defN 23-Mar-16 20:28 pyjamas/rcallbacks/rcbannotations.py
--rw-r--r--  2.0 unx    66708 b- defN 22-Jun-19 20:11 pyjamas/rcallbacks/rcbbatchprocess.py
--rw-r--r--  2.0 unx    35409 b- defN 22-Mar-02 19:53 pyjamas/rcallbacks/rcbclassifiers.py
+-rw-r--r--  2.0 unx    70337 b- defN 23-Apr-12 16:40 pyjamas/rcallbacks/rcbbatchprocess.py
+-rw-r--r--  2.0 unx    66441 b- defN 23-Apr-12 16:40 pyjamas/rcallbacks/rcbclassifiers.py
 -rw-r--r--  2.0 unx    77409 b- defN 23-Feb-22 03:17 pyjamas/rcallbacks/rcbimage.py
--rw-r--r--  2.0 unx    49461 b- defN 23-Feb-20 21:31 pyjamas/rcallbacks/rcbio.py
+-rw-r--r--  2.0 unx    52706 b- defN 23-Apr-12 16:40 pyjamas/rcallbacks/rcbio.py
 -rw-r--r--  2.0 unx    11288 b- defN 22-Dec-29 14:40 pyjamas/rcallbacks/rcbmeasure.py
 -rw-r--r--  2.0 unx    12556 b- defN 23-Mar-16 20:12 pyjamas/rcallbacks/rcboptions.py
 -rw-r--r--  2.0 unx     3617 b- defN 22-Aug-11 04:10 pyjamas/rcallbacks/rcbplugins.py
 -rw-r--r--  2.0 unx      913 b- defN 20-May-28 03:02 pyjamas/rimage/__init__.py
 -rw-r--r--  2.0 unx     3091 b- defN 21-Aug-22 22:13 pyjamas/rimage/csgraph.py
 -rw-r--r--  2.0 unx     3799 b- defN 23-Mar-14 22:07 pyjamas/rimage/rimcore.py
 -rw-r--r--  2.0 unx    67158 b- defN 23-Mar-16 20:13 pyjamas/rimage/rimutils.py
 -rw-r--r--  2.0 unx     1484 b- defN 21-Feb-14 22:27 pyjamas/rimage/rimml/__init__.py
--rw-r--r--  2.0 unx     3224 b- defN 22-Oct-11 01:54 pyjamas/rimage/rimml/batchclassifier.py
--rw-r--r--  2.0 unx     1499 b- defN 21-Oct-30 01:41 pyjamas/rimage/rimml/batchml.py
--rw-r--r--  2.0 unx     2473 b- defN 21-Oct-27 19:58 pyjamas/rimage/rimml/batchneuralnet.py
+-rw-r--r--  2.0 unx     3557 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/batchclassifier.py
+-rw-r--r--  2.0 unx     1585 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/batchml.py
+-rw-r--r--  2.0 unx     2740 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/batchneuralnet.py
+-rw-r--r--  2.0 unx     7409 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/batchrecurrentneuralnet.py
+-rw-r--r--  2.0 unx      275 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/classifier_types.py
 -rw-r--r--  2.0 unx     1173 b- defN 20-Aug-28 21:52 pyjamas/rimage/rimml/featurecalculator.py
 -rw-r--r--  2.0 unx     1387 b- defN 20-Dec-27 23:49 pyjamas/rimage/rimml/featurecalculator_rawimage.py
 -rw-r--r--  2.0 unx     1289 b- defN 20-Dec-27 23:49 pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
 -rw-r--r--  2.0 unx     3196 b- defN 21-Oct-27 19:58 pyjamas/rimage/rimml/featurecalculator_sog.py
--rw-r--r--  2.0 unx    17286 b- defN 22-Oct-11 01:54 pyjamas/rimage/rimml/rimclassifier.py
--rw-r--r--  2.0 unx     1687 b- defN 21-Oct-27 20:01 pyjamas/rimage/rimml/rimlr.py
+-rw-r--r--  2.0 unx    17339 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/rimclassifier.py
+-rw-r--r--  2.0 unx     1824 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/rimlr.py
 -rw-r--r--  2.0 unx     1382 b- defN 21-Oct-27 20:01 pyjamas/rimage/rimml/rimml.py
 -rw-r--r--  2.0 unx     1857 b- defN 21-Oct-27 20:01 pyjamas/rimage/rimml/rimneuralnet.py
--rw-r--r--  2.0 unx     1944 b- defN 21-Oct-27 20:01 pyjamas/rimage/rimml/rimsvm.py
--rw-r--r--  2.0 unx    14859 b- defN 22-Mar-02 19:26 pyjamas/rimage/rimml/rimunet.py
+-rw-r--r--  2.0 unx     1960 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/rimrecurrentneuralnet.py
+-rw-r--r--  2.0 unx    20936 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/rimrescunet.py
+-rw-r--r--  2.0 unx     2084 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/rimsvm.py
+-rw-r--r--  2.0 unx    15137 b- defN 23-Apr-12 16:40 pyjamas/rimage/rimml/rimunet.py
 -rw-r--r--  2.0 unx      847 b- defN 20-Jan-17 04:15 pyjamas/rplugins/__init__.py
 -rw-r--r--  2.0 unx     1249 b- defN 23-Feb-19 02:47 pyjamas/rplugins/base.py
 -rw-r--r--  2.0 unx      796 b- defN 23-Jan-02 00:28 pyjamas/tests/__init__.py
 -rw-r--r--  2.0 unx      857 b- defN 23-Jan-19 20:27 pyjamas/tests/conftest.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-25 02:03 pyjamas/tests/unit/__init__.py
 -rw-r--r--  2.0 unx     5912 b- defN 23-Feb-20 22:03 pyjamas/tests/unit/pjsfixtures.py
 -rw-r--r--  2.0 unx    11195 b- defN 23-Feb-16 03:14 pyjamas/tests/unit/test_image.py
 -rw-r--r--  2.0 unx    17400 b- defN 23-Feb-10 03:43 pyjamas/tests/unit/test_io.py
--rw-r--r--  2.0 unx     8308 b- defN 23-Mar-16 21:09 pyjamas_rfglab-2023.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 21:09 pyjamas_rfglab-2023.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Mar-16 21:09 pyjamas_rfglab-2023.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-16 21:09 pyjamas_rfglab-2023.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6516 b- defN 23-Mar-16 21:09 pyjamas_rfglab-2023.3.1.dist-info/RECORD
-74 files, 3747546 bytes uncompressed, 519023 bytes compressed:  86.2%
+-rw-r--r--  2.0 unx     8308 b- defN 23-Apr-12 17:01 pyjamas_rfglab-2023.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 17:01 pyjamas_rfglab-2023.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Apr-12 17:01 pyjamas_rfglab-2023.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 17:01 pyjamas_rfglab-2023.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7179 b- defN 23-Apr-12 17:01 pyjamas_rfglab-2023.4.0.dist-info/RECORD
+81 files, 3843152 bytes uncompressed, 537917 bytes compressed:  86.0%
```

## zipnote {}

```diff
@@ -33,17 +33,23 @@
 
 Filename: pyjamas/dialogs/batchanalysis.py
 Comment: 
 
 Filename: pyjamas/dialogs/batchprojectconcat.py
 Comment: 
 
+Filename: pyjamas/dialogs/batchresize.py
+Comment: 
+
 Filename: pyjamas/dialogs/classifierdialogABC.py
 Comment: 
 
+Filename: pyjamas/dialogs/classifiertype.py
+Comment: 
+
 Filename: pyjamas/dialogs/expandnpropagateseeds.py
 Comment: 
 
 Filename: pyjamas/dialogs/expandseeds.py
 Comment: 
 
 Filename: pyjamas/dialogs/findseeds.py
@@ -63,14 +69,17 @@
 
 Filename: pyjamas/dialogs/nonmax_suppr.py
 Comment: 
 
 Filename: pyjamas/dialogs/propagateseeds.py
 Comment: 
 
+Filename: pyjamas/dialogs/rescuneuralnet.py
+Comment: 
+
 Filename: pyjamas/dialogs/svm.py
 Comment: 
 
 Filename: pyjamas/dialogs/textdialog.py
 Comment: 
 
 Filename: pyjamas/dialogs/timepoints.py
@@ -147,14 +156,20 @@
 
 Filename: pyjamas/rimage/rimml/batchml.py
 Comment: 
 
 Filename: pyjamas/rimage/rimml/batchneuralnet.py
 Comment: 
 
+Filename: pyjamas/rimage/rimml/batchrecurrentneuralnet.py
+Comment: 
+
+Filename: pyjamas/rimage/rimml/classifier_types.py
+Comment: 
+
 Filename: pyjamas/rimage/rimml/featurecalculator.py
 Comment: 
 
 Filename: pyjamas/rimage/rimml/featurecalculator_rawimage.py
 Comment: 
 
 Filename: pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
@@ -171,14 +186,20 @@
 
 Filename: pyjamas/rimage/rimml/rimml.py
 Comment: 
 
 Filename: pyjamas/rimage/rimml/rimneuralnet.py
 Comment: 
 
+Filename: pyjamas/rimage/rimml/rimrecurrentneuralnet.py
+Comment: 
+
+Filename: pyjamas/rimage/rimml/rimrescunet.py
+Comment: 
+
 Filename: pyjamas/rimage/rimml/rimsvm.py
 Comment: 
 
 Filename: pyjamas/rimage/rimml/rimunet.py
 Comment: 
 
 Filename: pyjamas/rplugins/__init__.py
@@ -201,23 +222,23 @@
 
 Filename: pyjamas/tests/unit/test_image.py
 Comment: 
 
 Filename: pyjamas/tests/unit/test_io.py
 Comment: 
 
-Filename: pyjamas_rfglab-2023.3.1.dist-info/METADATA
+Filename: pyjamas_rfglab-2023.4.0.dist-info/METADATA
 Comment: 
 
-Filename: pyjamas_rfglab-2023.3.1.dist-info/WHEEL
+Filename: pyjamas_rfglab-2023.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyjamas_rfglab-2023.3.1.dist-info/entry_points.txt
+Filename: pyjamas_rfglab-2023.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyjamas_rfglab-2023.3.1.dist-info/top_level.txt
+Filename: pyjamas_rfglab-2023.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyjamas_rfglab-2023.3.1.dist-info/RECORD
+Filename: pyjamas_rfglab-2023.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyjamas/pjscore.py

```diff
@@ -125,15 +125,15 @@
     livewire_margin: int = 5
     livewire_heuristic_weight: float = 0.  # defaults to Dijkstra.
     balloon_crop_size: int = 50  # crop size used to inflate balloons
 
     undo_stack_size: int = 500
 
     # Read version.
-    __version__: str = '2023.3.1'
+    __version__: str = '2023.4.0'
 
     def __init__(self):
         self.initData()  # Initialize object variables.
         self.setupUI()  # Build the GUI.
 
     def setupUI(self):
         self.app = QtWidgets.QApplication(sys.argv)
@@ -432,21 +432,26 @@
                          self.classifiers.cbCreateLR)
         self.addMenuItem(self.menuClassifiers, 'Create and train support vector machine ...', None,
                          self.classifiers.cbCreateSVM)
         # self.addMenuItem(self.menuClassifiers, 'Create and train convolutional neural network ...', None,
         #                 self.classifiers.cbCreateCNN)
         self.addMenuItem(self.menuClassifiers, 'Create and train UNet ...', None,
                          self.classifiers.cbCreateUNet)
+        self.addMenuItem(self.menuClassifiers, 'Create and train ReSCUNet ...', None,
+                         self.classifiers.cbCreateReSCUNet)
 
         # -- Decision Trees
 
         self.menuClassifiers.addSeparator()
 
         self.addMenuItem(self.menuClassifiers, 'Apply classifier ...', None, self.classifiers.cbApplyClassifier)
 
+        self.addMenuItem(self.menuClassifiers, 'Apply tracking classifier ...', None,
+                         self.classifiers.cbApplyTrackingClassifier)
+
         self.menuClassifiers.addSeparator()
 
         self.addMenuItem(self.menuClassifiers, 'Non-maximum suppression ...', None,
                          self.classifiers.cbNonMaxSuppression)
 
         self.addMenuItem(self.menuClassifiers, 'Segment detected objects ...', None,
                          self.image.cbSegmentDetectedObjects)
@@ -558,14 +563,17 @@
                                  projection_type=rcallbacks.rcbimage.projection_types.MAX))
 
         # Sum project and concatenate.
         self.addMenuItem(self.menuBatch, "Sum project and concatenate ...", None,
                          partial(self.batch.cbBatchProjectConcat,
                                  projection_type=rcallbacks.rcbimage.projection_types.SUM))
 
+        # Resize images.
+        self.addMenuItem(self.menuBatch, "Resize images ...", None, self.batch.cbBatchResize)
+
         self.menuBatch.addSeparator()
 
         # Measure.
         self.addMenuItem(self.menuBatch, "Measure ...", None,
                          self.batch.cbMeasureBatch)
 
         self.menubar.addMenu(self.menuBatch)
@@ -938,19 +946,23 @@
         apolygonf = QtGui.QPolygonF()
         apolygonf.append(QtCore.QPointF(aVector.origin[0], aVector.origin[1]))
         apolygonf.append(QtCore.QPointF(aVector.end[0], aVector.end[1]))
 
         aPath.addPolygon(apolygonf)
         return self.gScene.addPath(aPath, pen, PyJAMAS.polyline_brush_style)
 
-    def addPolyline(self, coordinates: list, z: int, paint: bool = True, pushundo=False) -> bool:
+    def addPolyline(self, coordinates: list, z: int, theid: int = None, paint: bool = True, pushundo=False) -> bool:
         thepolyline: QtGui.QPolygonF = RUtils.list2qpolygonf(coordinates)
 
         self.polylines[z].append(thepolyline)
-        polyline_id = max(self.polyline_ids[z]) + 1 if len(self.polyline_ids[z]) else 1
+        if theid is not None and type(theid) == int and theid > 0:
+            polyline_id = theid
+        else:
+            polyline_id = max(self.polyline_ids[z]) + 1 if len(self.polyline_ids[z]) else 1
+
         self.polyline_ids[z].append(polyline_id)
         if pushundo:
             self.undo_stack.push(
                 {'changetype': undo_modes.POLYLINE_ADDED, 'frame': z, 'index': len(self.polylines[z]) - 1,
                  'details': None})
 
         # Draw the polyline if it is being added to the right time point.
```

## pyjamas/pjseventfilter.py

```diff
@@ -168,15 +168,14 @@
                     if y0 > y1:
                         y1, y0 = y0, y1
 
                     self.pjs._poly_ = []
                     self.pjs.addPolyline([[x0, y0], [x0, y1], [x1, y1], [x1, y0], [x0, y0]], self.pjs.curslice,
                                          pushundo=True)
 
-
             elif self.pjs.annotation_mode == PyJAMAS.polyline_annotations:
                 if event.type() == QtCore.QEvent.MouseButtonPress:
                     # Store coordinate if left click ...
                     if event.buttons() == QtCore.Qt.LeftButton:
                         self.pjs._poly_.append([self.x, self.y])
 
                         if self.pjs._agraphicsitem_ and self.pjs._agraphicsitem_.scene():
@@ -415,15 +414,14 @@
 
                         self.pjs.repaint()
 
                 # Update polyline as mouse button is released.
                 #elif event.type() == QtCore.QEvent.MouseButtonRelease and self.pjs._poly_ != []:
                 #    self.pjs._poly_ = []
 
-
             elif self.pjs.annotation_mode == PyJAMAS.export_fiducial_polyline:
                 self.process_export_fiducial_polyline(event)
 
             elif event.type() == QtCore.QEvent.Resize:
                 self.pjs.timeSlider.setGeometry(
                     QtCore.QRect(0, self.pjs.MainWindow.height() - 43, self.pjs.MainWindow.width(), 22))
```

## pyjamas/dialogs/__init__.py

```diff
@@ -13,16 +13,17 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from . import measurepoly, propagateseeds, expandseeds, expandnpropagateseeds, batchprojectconcat, svm, nonmax_suppr, \
-    timepoints, textdialog, findseeds, matplotlibdialog, logregression, adjustcontrast, batchanalysis, neuralnet
+    timepoints, textdialog, findseeds, matplotlibdialog, logregression, adjustcontrast, batchanalysis, neuralnet, \
+    rescuneuralnet
 
 __all__ = [measurepoly.MeasurePolyDialog, propagateseeds.PropagateSeedsDialog, expandseeds.ExpandSeedsDialog,
            expandnpropagateseeds.ExpandNPropagateSeedsDialog, batchprojectconcat.BatchProjectConcatenateDialog,
            svm.SVMDialog, nonmax_suppr.NonMaxDialog, timepoints.TimePointsDialog, textdialog.TextDialog,
            findseeds.FindSeedsDialog,
            matplotlibdialog.MatplotlibDialog, logregression.LRDialog,
            adjustcontrast.AdjustContrastDialog, batchanalysis.BatchMeasureDialog,
-           neuralnet.NeuralNetDialog]
+           neuralnet.NeuralNetDialog, rescuneuralnet.ReSCUNeuralNetDialog]
```

## pyjamas/rcallbacks/rcbbatchprocess.py

```diff
@@ -27,16 +27,19 @@
 from nbformat.notebooknode import NotebookNode
 import numpy
 import pandas as pd
 # import pylustrator
 from PyQt5 import QtWidgets
 import seaborn as sns
 from scipy.optimize import leastsq
+import skimage.io as sio
+import skimage.transform as st
 
 from pyjamas.dialogs.batchanalysis import BatchMeasureDialog
+from pyjamas.dialogs.batchresize import BatchResizeDialog
 from pyjamas.dialogs.batchprojectconcat import BatchProjectConcatenateDialog
 from pyjamas.pjscore import PyJAMAS
 from pyjamas.pjsthreads import ThreadSignals
 from pyjamas.rcallbacks.rcallback import RCallback
 from pyjamas.rcallbacks.rcbimage import projection_types
 from pyjamas.rimage.rimutils import rimutils as rimutils
 from pyjamas.rutils import RUtils
@@ -162,14 +165,85 @@
             if return_value:
                 self.pjs.cwd = os.path.abspath(theparameters['input_folder'])
 
             return return_value
         else:
             return False
 
+    def cbBatchResize(self, parameters: Optional[dict] = None):
+        """
+        Resizes all images within a given folder or folder tree to a specified size and saves them to a new folder.
+
+        :param parameters: dictionary with parameters, a dialog will open if the value is none.
+
+            ``input_folder``: absolute path to the folder containing all images to be resized.
+            ``save_folder``: absolute path to the folder that resized images will be saved to.
+            ``im_size``: tuple containing the new image size in (rows, cols), eq. (height, width).
+            ``recurr``: When set to true, the folder tree will be searched recursively for images to be resized.
+
+        :return: True if resizing complete, False otherwise.
+        """
+        # Get folder name.
+        continue_flag: bool = True
+
+        if parameters is None or parameters is False:
+            dialog = QtWidgets.QDialog()
+            ui = BatchResizeDialog()
+            ui.setupUi(dialog)
+
+            dialog.exec_()
+            dialog.show()
+
+            continue_flag = dialog.result() == QtWidgets.QDialog.Accepted
+
+            if continue_flag:
+                parameters = ui.parameters()
+
+            dialog.close()
+
+        if continue_flag:
+            input_folder = parameters.get('input_folder')
+            save_folder = parameters.get('save_folder')
+            im_size = parameters.get('im_size')
+            recurr = parameters.get('recurr')
+            if save_folder == '':
+                save_folder = input_folder + f"_resized_{im_size[0]}x{im_size[1]}"
+            if not os.path.exists(save_folder):
+                os.mkdir(save_folder)
+            self.batch_resize_images(input_folder, save_folder, im_size, recurr)
+            self.pjs.statusbar.showMessage('Finished.')
+        else:
+            self.pjs.statusbar.showMessage('Error during resizing.')
+            return False
+
+    def batch_resize_images(self, input_folder: Optional[str] = None, save_folder: Optional[str] = None,
+                            im_size: Optional[tuple] = (512, 512), recurr: Optional[bool] = True):
+        for subfile in os.listdir(input_folder):
+            subfile_path = os.path.join(input_folder, subfile)
+            if os.path.isdir(subfile_path) and recurr:
+                if not os.path.exists(os.path.join(save_folder, subfile)):
+                    os.mkdir(os.path.join(save_folder, subfile))
+                self.batch_resize_images(subfile_path, os.path.join(save_folder, subfile), im_size, recurr)
+            elif os.path.splitext(subfile_path)[1] == '.tif':
+                img = sio.imread(subfile_path)
+                if img.ndim == 3:
+                    img = img[0, :, :]
+                img = numpy.expand_dims(
+                    st.resize(img, (im_size[0], im_size[1]), order=3, mode='constant', preserve_range=True), axis=-1)
+                if numpy.unique(img).size == 2:  # Binary image, need to correct for interpolation
+                    max_value = numpy.max(numpy.max(img))
+                    img = numpy.round(numpy.divide(img, numpy.full(img.shape, max_value)))
+                    img = numpy.multiply(img, numpy.full(img.shape, max_value))
+                    img = numpy.maximum(img, numpy.zeros((im_size[0], im_size[1], 1)))
+                sio.imsave(os.path.join(save_folder, subfile), img[:, :, 0], check_contrast=False)
+            else:  # Not an acceptable image type or sub-directory
+                continue
+
+        return True
+
     def cbMeasureBatch(self, parameters: Optional[dict] = None) -> bool:
         """
         Measures image data sets and produces plots and CSV files that combine all the data. A Python script to reproduce the analysis, and a Jupyter notebook to reproduce the analysis and generate the plots can also be generated.
 
         :param parameters: dictionary containing measurement parameters; a dialog will open if the value is set to None; dictionary keys are:
 
             ``folder1``:
@@ -863,15 +937,16 @@
 
         # Create filename.
         thenow = datetime.now()
         filename = thenow.strftime(
             f"{thenow.year:04}{thenow.month:02}{thenow.day:02}_{thenow.hour:02}{thenow.minute:02}{thenow.second:02}")
 
         # This ensures paths that work in both Unix and Windows.
-        filepath = self.results_folder + filename if self.results_folder.endswith('/') else self.results_folder + '/' + filename
+        filepath = self.results_folder + filename if self.results_folder.endswith(
+            '/') else self.results_folder + '/' + filename
 
         # Save DataFrame to folder.
         all_data.to_csv(RUtils.set_extension(filepath + self.analysis_filename_appendix, self.analysis_extension))
 
         # Save Python script to folder.
         with open(RUtils.set_extension(filepath + self.script_filename_appendix, RCBBatchProcess.SCRIPT_EXTENSION_BM),
                   "w") as f:
@@ -901,15 +976,15 @@
 
         return True
 
     def _save_notebook_setup(self, data_path: str, parameters: dict) -> NotebookNode:
         nb: NotebookNode = nbf.v4.new_notebook()
         nb['cells'] = []
 
-        text = f"""# PyJAMAS notebook {data_path[data_path.rfind(os.sep)+1:]}"""
+        text = f"""# PyJAMAS notebook {data_path[data_path.rfind(os.sep) + 1:]}"""
         nb['cells'].append(nbf.v4.new_markdown_cell(text))
 
         text = """We start by importing the packages necessary to run and plot the analysis:"""
         nb['cells'].append(nbf.v4.new_markdown_cell(text))
 
         code = f"import matplotlib\n" \
                f"import matplotlib.pyplot as plt\n" \
@@ -956,15 +1031,15 @@
 
         return nb
 
     def _save_widget_notebook_setup(self, data_path: str, parameters: dict) -> NotebookNode:
         nb: NotebookNode = nbf.v4.new_notebook()
         nb['cells'] = []
 
-        text = f"""# PyJAMAS notebook {data_path[data_path.rfind(os.sep)+1:]}"""
+        text = f"""# PyJAMAS notebook {data_path[data_path.rfind(os.sep) + 1:]}"""
         nb['cells'].append(nbf.v4.new_markdown_cell(text))
 
         text = """We start by importing the packages necessary to run and plot the analysis. We also create lists that define what we will be plotting."""
         nb['cells'].append(nbf.v4.new_markdown_cell(text))
 
         code = f"import ipywidgets as widgets\n" \
                f"import matplotlib\n" \
@@ -1171,8 +1246,8 @@
 
         code += f"    ax.legend(frameon=False)\n" \
                 f"    ax = sns.stripplot(x='experimental group', y=metric, data=thedata, color='k', alpha=0.75, size=6, dodge=False, jitter=0.05)\n" \
                 f"    sns.despine()\n" \
                 f"    return"
         nb['cells'].append(nbf.v4.new_code_cell(code))
 
-        return nb
+        return nb
```

## pyjamas/rcallbacks/rcbclassifiers.py

```diff
@@ -29,16 +29,17 @@
 from pyjamas.pjscore import PyJAMAS
 from pyjamas.pjsthreads import ThreadSignals
 from pyjamas.rcallbacks.rcallback import RCallback
 from pyjamas.rimage.rimml.rimclassifier import rimclassifier
 import pyjamas.rimage.rimml.rimlr as rimlr
 import pyjamas.rimage.rimml.rimsvm as rimsvm
 import pyjamas.rimage.rimml.rimunet as rimunet
+import pyjamas.rimage.rimml.rimrescunet as rimrescunet
 from pyjamas.rutils import RUtils
-
+from pyjamas.rimage.rimml.classifier_types import classifier_types
 
 
 class RCBClassifiers(RCallback):
     COLAB_NOTEBOOK_APPENDIX: str = '_colab_notebook'
 
     def cbCreateLR(self, parameters: Optional[dict] = None, wait_for_thread: bool = False) -> bool:
         """
@@ -133,34 +134,99 @@
         if continue_flag:
             self.pjs.batch_classifier.image_classifier = rimunet.UNet(parameters)
 
             if not parameters.get('generate_notebook'):
                 self.launch_thread(self.pjs.batch_classifier.fit, {'stop': True}, finished_fn=self.finished_fn,
                                    stop_fn=self.stop_fn, wait_for_thread=wait_for_thread)
             else:
-                self._generate_unet_notebook(parameters)
+                self._generate_neuralnet_notebook(parameters)
+
+            return True
+
+        else:
+            return False
+
+    def cbCreateReSCUNet(self, parameters: Optional[dict] = None, wait_for_thread: bool = False) -> bool:  # Handle IO errors.
+        """
+        Create a convolutional neural network with ReSCUNet architecture.
+
+        :param parameters: dictionary containing the parameters to create a ReSCUNet; a dialog opens if this parameter is set to None; keys are:
+
+            ``positive_training_folder``:
+                path to the folder containing positive training images, formatted as a string
+            ``train_image_size``:
+                the number of rows and columns in the network input (train images will be scaled to this size) formatted as a tuple of two integers, both of the integers must be divisible by 16.
+            ``step_sz``:
+                number of pixel rows and columns to divide test images into, each subimage will be scaled to the network input size and processed, formatted as a tuple of two integers
+            ``epochs``:
+                maximum number of iterations over the training data, as an int
+            ``learning_rate``:
+                step size when updating the weights, as a float
+            ``mini_batch_size``:
+                size of mini batches, as an int
+            ``erosion_width``:
+                width of the erosion kernel to apply to the labeled image produced by the UNet, to separate touching objects, as an int
+            ``concatenation_depth``:
+                number of encoder blocks before previous segmentation mask and current image frame input streams are combined in the network
+            ``generate_notebook``:
+                whether a Jupyter notebook to create and train the UNet (e.g. in Google Colab) should be generated, as a bool (if True, the UNet will NOT be created)
+            ``notebook_path``:
+                where to store the Jupyter notebook if it must be created
+            ``save_folder``:
+                where to store resized images and weight maps, if empty the resized images and weight maps will not be saved
+            ``resize_images_flag``:
+                whether or not to resize images, resized images and weight_maps will be loaded from positive_training_folder if False
+        :param wait_for_thread: True if PyJAMAS must wait for the thread running this operation to complete, False otherwise.
+        :return: True if the classifier was successfully created, False otherwise.
+        """
+        continue_flag = True
+
+        if parameters is None or parameters is False:
+            dialog = QtWidgets.QDialog()
+            ui = dialogs.rescuneuralnet.ReSCUNeuralNetDialog()
+            ui.setupUi(dialog)
+
+            dialog.exec_()
+            dialog.show()
+
+            continue_flag = dialog.result() == QtWidgets.QDialog.Accepted
+            parameters = ui.parameters()
+
+            dialog.close()
+
+        if continue_flag:
+            self.pjs.batch_classifier.image_classifier = rimrescunet.ReSCUNet(parameters)
+
+            if not parameters.get('generate_notebook'):
+                self.launch_thread(self.pjs.batch_classifier.fit, {'stop': True}, finished_fn=self.finished_fn,
+                                   stop_fn=self.stop_fn, wait_for_thread=wait_for_thread)
+            else:
+                self._generate_neuralnet_notebook(parameters)
 
             return True
 
         else:
             return False
 
-    def _generate_unet_notebook(self, parameters: dict) -> bool:
+    def _generate_neuralnet_notebook(self, parameters: dict, architecture: classifier_types) -> bool:
         # Follow scheme of path generation from measure notebook from rcbbatchprocess._save_notebook
         path = parameters.get('notebook_path')
 
         # Create filename
         thenow = datetime.now()
         filename = thenow.strftime(
             f"{thenow.year:04}{thenow.month:02}{thenow.day:02}_{thenow.hour:02}{thenow.minute:02}{thenow.second:02}")
         filepath = path + filename if path.endswith('/') else path + '/' + filename
 
         fname = RUtils.set_extension(filepath+RCBClassifiers.COLAB_NOTEBOOK_APPENDIX, PyJAMAS.notebook_extension)
 
-        nb: NotebookNode = self._save_unet_notebook(fname, parameters)
+        if architecture == classifier_types.RESCUNET.value:
+            nb: NotebookNode = self._save_rescunet_notebook(fname, parameters)
+        else:
+            nb: NotebookNode = self._save_unet_notebook(fname, parameters)
 
         nb['metadata'].update({'language_info': {'name': 'python'}})
 
         with open(fname, 'w', encoding="utf-8") as f:
             nbf.write(nb, f)
 
         return True
@@ -257,14 +323,15 @@
         nb['cells'].append(nbf.v4.new_code_cell(code))
 
         text = f"Set some parameters:"
         nb['cells'].append(nbf.v4.new_markdown_cell(text))
 
         rows, cols = parameters.get('train_image_size', rimunet.UNet.TRAIN_IMAGE_SIZE[0:2])
         code =  f"BATCH_SIZE = {parameters.get('mini_batch_size', rimunet.UNet.BATCH_SIZE)}\n" \
+                f"CLASSIFIER_TYPE = {classifier_types.UNET.value}\n" \
                 f"EPOCHS = {parameters.get('epochs', rimunet.UNet.EPOCHS)}\n" \
                 f"LEARNING_RATE = {parameters.get('learning_rate', rimunet.UNet.LEARNING_RATE)}\n" \
                 f"IMG_WIDTH = {cols}\n" \
                 f"IMG_HEIGHT = {rows}\n" \
                 f"IMG_CHANNELS = 1\n" \
                 f"TRAIN_PATH = '/content/train/'\n" \
                 f"TEST_PATH = '/content/test/'\n" \
@@ -498,14 +565,15 @@
                 f"plt.plot(history.history['loss'])"
         nb['cells'].append(nbf.v4.new_code_cell(code))
 
         text = """Save and download the model (can be loaded into PyJAMAS):"""
         nb['cells'].append(nbf.v4.new_markdown_cell(text))
 
         code = """theclassifier = {
+    'classifier_type': CLASSIFIER_TYPE,
     'positive_training_folder': TRAIN_PATH,
     'train_image_size': (IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS),
     'scaler': themax,
     'epochs': EPOCHS,
     'mini_batch_size': BATCH_SIZE,
     'learning_rate': LEARNING_RATE,
     'classifier': model.get_weights(),
@@ -547,14 +615,511 @@
                 f"ax2.imshow(np.squeeze(yhat), cmap=plt.cm.gray)\n" \
                 f"ax3.imshow(np.squeeze(testLabel), cmap=plt.cm.gray)\n" \
                 f"ax4.imshow(np.squeeze(weightImage), cmap=plt.cm.gray)"
         nb['cells'].append(nbf.v4.new_code_cell(code))
 
         return nb
 
+    def _save_rescunet_notebook(self, filepath: str, parameters: dict) -> NotebookNode:
+        nb: NotebookNode = nbf.v4.new_notebook()
+        nb['cells'] = []
+
+        filename = filepath[filepath.rfind(os.sep) + 1:]
+
+        text = f"""# PyJAMAS notebook for Google Colab {filename}"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        text = f"Use the following folder structure:\n" \
+               f"\n" \
+               f"train/\n" \
+               f"\n\ttrain_folder_name_1/\n" \
+               f"\t\timage/\n" \
+               f"\t\t\ttrain_image_name_1.tif\n" \
+               f"\t\tmask/\n" \
+               f"\t\t\ttrain_image_name_1.tif\n" \
+               f"\t\tprev_mask/\n" \
+               f"\t\t\ttrain_image_name_1.tif\n" \
+               f"\n" \
+               f"\t.\n" \
+               f"\t.\n" \
+               f"\t.\n" \
+               f"\n\ttrain_folder_name_n/\n" \
+               f"\t\timage/\n" \
+               f"\t\t\ttrain_image_name_n.tif\n" \
+               f"\t\tmask/\n" \
+               f"\t\t\ttrain_image_name_n.tif\n" \
+               f"\t\tprev_mask/\n" \
+               f"\t\t\ttrain_image_name_n.tif\n" \
+               f"\n" \
+               f"test/\n" \
+               f"\n\ttest_folder_name_1/\n" \
+               f"\t\timage/\n" \
+               f"\t\t\ttest_image_name_1.tif\n" \
+               f"\t\tmask/\n" \
+               f"\t\t\ttest_image_name_1.tif\n" \
+               f"\t\tprev_mask/\n" \
+               f"\t\t\ttest_image_name_1.tif\n" \
+               f"\n" \
+               f"\t.\n" \
+               f"\t.\n" \
+               f"\t.\n" \
+               f"\n\ttest_folder_name_m/\n" \
+               f"\t\timage/\n" \
+               f"\t\t\ttest_image_name_m.tif\n" \
+               f"\t\tmask/\n" \
+               f"\t\t\ttest_image_name_m.tif\n" \
+               f"\t\tprev_mask/\n" \
+               f"\t\t\ttest_image_name_m.tif\n" \
+               f"\n" \
+               f"Zip up the data into a file (e.g. testtrain.zip) and upload the file into /content in a google colab runtime.\n" \
+               f"Then change into the /content folder and unzip the data."
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = f"!cd /content"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        code = f"!unzip testtrain.zip"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """We import the packages necessary to run and plot the analysis:"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = f"import os\n" \
+               f"from typing import Optional, Tuple\n" \
+               f"import pickle\n" \
+               f"import gzip\n" \
+               f"from tqdm import tqdm\n" \
+               f"import numpy as np\n" \
+               f"import matplotlib.pyplot as plt\n" \
+               f"from skimage import draw\n" \
+               f"from skimage.io import imread, imshow, imread_collection, concatenate_images\n" \
+               f"from skimage.transform import resize\n" \
+               f"from skimage.morphology import label\n" \
+               f"from skimage.segmentation import find_boundaries\n" \
+               f"from joblib import Parallel, delayed\n" \
+               f"import matplotlib.pyplot as plt\n" \
+               f"%matplotlib inline\n" \
+               f"import sys\n" \
+               f"import random\n" \
+               f"import warnings\n" \
+               f"import pandas as pd\n" \
+               f"from itertools import chain\n" \
+               f"import tensorflow as tf\n" \
+               f"import tensorflow.keras.backend as kb" \
+               f"import tensorflow.keras.utils as ku\n" \
+               f"from tensorflow.keras.metrics import MeanIoU\n" \
+               f"from tensorflow.keras.models import Model, load_model\n" \
+               f"from tensorflow.keras.layers import Input\n" \
+               f"from tensorflow.keras.layers import Dropout, Lambda\n" \
+               f"from tensorflow.keras.layers import Conv2D, Conv2DTranspose\n" \
+               f"from tensorflow.keras.layers import MaxPooling2D\n" \
+               f"from tensorflow.keras.layers import Lambda\n" \
+               f"from tensorflow.keras.layers import concatenate\n" \
+               f"from tensorflow.keras.layers import multiply\n" \
+               f"from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint\n" \
+               f"from tensorflow.keras.optimizers import Adam\n" \
+               f"from tensorflow.keras.preprocessing import image\n" \
+               f"from tensorflow.keras import backend as K\n" \
+               f"from tensorflow.keras import layers as L"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = f"Set some parameters:"
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        rows, cols = parameters.get('train_image_size', rimrescunet.ReSCUNet.TRAIN_IMAGE_SIZE[0:2])
+        code =  f"BATCH_SIZE = {parameters.get('mini_batch_size', rimrescunet.ReSCUNet.BATCH_SIZE)}\n" \
+                f"EPOCHS = {parameters.get('epochs', rimrescunet.ReSCUNet.EPOCHS)}\n" \
+                f"LEARNING_RATE = {parameters.get('learning_rate', rimrescunet.ReSCUNet.LEARNING_RATE)}\n" \
+                f"CLASSIFIER_TYPE = {classifier_types.RESCUNET.value}\n" \
+                f"CONCATENATION_LEVEL = {parameters.get('concatenation_level', rimrescunet.ReSCUNet.CONCATENATION_LEVEL)}\n" \
+                f"IMG_WIDTH = {cols}\n" \
+                f"IMG_HEIGHT = {rows}\n" \
+                f"IMG_CHANNELS = 1\n" \
+                f"TRAIN_PATH = '/content/train/'\n" \
+                f"TEST_PATH = '/content/test/'\n" \
+                f"MODEL_FILE_NAME = '{RUtils.set_extension(filename, PyJAMAS.classifier_extension)}'\n" \
+                f"PICKLE_PROTOCOL = {RUtils.DEFAULT_PICKLE_PROTOCOL}\n" \
+                f"warnings.filterwarnings('ignore', category=UserWarning, module='skimage')\n" \
+                f"seed = 42\n" \
+                f"random.seed(seed)\n" \
+                f"np.random.seed(seed)"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = f"Define weight function:"
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = """def weight_map(binmasks, w0=10, sigma=5, show=False):
+    \"\"\"Compute the weight map for a given mask, as described in Ronneberger et al.
+    (https://arxiv.org/pdf/1505.04597.pdf)
+    \"\"\"
+
+    labmasks = label(binmasks)
+    n_objs = np.amax(labmasks)
+
+    nrows, ncols = labmasks.shape[:2]
+    masks = np.zeros((n_objs, nrows, ncols))
+    distMap = np.zeros((nrows * ncols, n_objs))
+    X1, Y1 = np.meshgrid(np.arange(nrows), np.arange(ncols))
+    X1, Y1 = np.c_[X1.ravel(), Y1.ravel()].T
+    for i in tqdm(range(n_objs)):
+        mask = np.squeeze(labmasks == i + 1)
+        bounds = find_boundaries(mask, mode='inner')
+        X2, Y2 = np.nonzero(bounds)
+        xSum = (X2.reshape(-1, 1) - X1.reshape(1, -1)) ** 2
+        ySum = (Y2.reshape(-1, 1) - Y1.reshape(1, -1)) ** 2
+        distMap[:, i] = np.sqrt(xSum + ySum).min(axis=0)
+        masks[i] = mask
+    ix = np.arange(distMap.shape[0])
+    if distMap.shape[1] == 1:
+        d1 = distMap.ravel()
+        border_loss_map = w0 * np.exp((-1 * (d1) ** 2) / (2 * (sigma ** 2)))
+    else:
+        if distMap.shape[1] == 2:
+            d1_ix, d2_ix = np.argpartition(distMap, 1, axis=1)[:, :2].T
+        else:
+            d1_ix, d2_ix = np.argpartition(distMap, 2, axis=1)[:, :2].T
+        d1 = distMap[ix, d1_ix]
+        d2 = distMap[ix, d2_ix]
+        border_loss_map = w0 * np.exp((-1 * (d1 + d2) ** 2) / (2 * (sigma ** 2)))
+    xBLoss = np.zeros((nrows, ncols))
+    xBLoss[X1, Y1] = border_loss_map
+    # class weight map
+    loss = np.zeros((nrows, ncols))
+    w_1 = 1 - masks.sum() / loss.size
+    w_0 = 1 - w_1
+    loss[masks.sum(0) == 1] = w_1
+    loss[masks.sum(0) == 0] = w_0
+    ZZ = xBLoss + loss
+    # ZZ = resize(ZZ, outsize, preserve_range=True)
+    if show:
+        plt.imshow(ZZ)
+        plt.colorbar()
+        plt.axis('off')
+    return ZZ"""
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """Resize images and normalize intensities:"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = """# Get train and test IDs
+train_ids = next(os.walk(TRAIN_PATH))[1]
+test_ids = next(os.walk(TEST_PATH))[1]
+
+X_train = np.zeros((len(train_ids), IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS), dtype=np.uint16)
+X_train_mask = np.zeros((len(train_ids), IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS), dtype=np.bool)
+Y_train = np.zeros((len(train_ids), IMG_HEIGHT, IMG_WIDTH, 1), dtype=bool)
+W_train = np.zeros((len(train_ids), IMG_HEIGHT, IMG_WIDTH, 1), dtype=float)
+print('Getting and resizing train images and masks ... ')
+sys.stdout.flush()
+for n, id_ in tqdm(enumerate(train_ids), total=len(train_ids)):
+    path = TRAIN_PATH + id_
+    im_file = path+"/image/"+os.listdir(path+"/image/")[0]
+    img = imread(im_file)
+    if img.ndim == 3:
+        img = img[0,:,:]
+    img = np.expand_dims(resize(img, (IMG_HEIGHT, IMG_WIDTH), mode='constant', preserve_range=True),axis=-1)
+    X_train[n] = img
+    prev_msk_file = path+"/prev_mask/"+os.listdir(path+"/prev_mask/")[0]
+    prev_mask = np.zeros((IMG_HEIGHT, IMG_WIDTH, 1), dtype=bool)
+    prev_mask_ = imread(prev_msk_file)
+    prev_mask_ = np.expand_dims(resize(prev_mask_, (IMG_HEIGHT, IMG_WIDTH), mode='constant', 
+                                      preserve_range=True), axis=-1)
+    max_value = np.max(np.max(prev_mask_))
+    prev_mask_ = np.round(np.divide(prev_mask_, np.full(prev_mask_.shape, max_value)))
+    prev_mask_ = np.multiply(prev_mask_, np.full(prev_mask_.shape, max_value))
+    prev_mask = np.maximum(prev_mask, prev_mask_)
+    X_train_mask[n] = prev_mask
+    
+    msk_file = path+"/mask/"+os.listdir(path+"/mask/")[0]
+    mask = np.zeros((IMG_HEIGHT, IMG_WIDTH, 1), dtype=bool)
+    mask_ = imread(msk_file)
+    mask_ = np.expand_dims(resize(mask_, (IMG_HEIGHT, IMG_WIDTH), mode='constant', 
+                                      preserve_range=True), axis=-1)
+    max_value = np.max(np.max(mask_))
+    mask_ = np.round(np.divide(mask_, np.full(mask_.shape, max_value)))
+    mask_ = np.multiply(mask_, np.full(mask_.shape, max_value))
+    mask = np.maximum(mask, mask_)
+    weights = weight_map(mask)
+    Y_train[n] = mask
+    W_train[n, :, :, 0] = weights
+
+# Get and resize test images
+X_test = np.zeros((len(test_ids), IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS), dtype=np.uint16)
+X_test_mask = np.zeros((len(test_ids), IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS), dtype=np.bool)
+Y_test = np.zeros((len(test_ids), IMG_HEIGHT, IMG_WIDTH, 1), dtype=bool)
+print('Getting and resizing test images ... ')
+sys.stdout.flush()
+for n, id_ in tqdm(enumerate(test_ids), total=len(test_ids)):
+    path = TEST_PATH + id_
+    im_file = path+"/image/"+os.listdir(path+"/image/")[0]
+    img = imread(im_file)
+    if img.ndim == 3:
+        img = img[0,:,:]
+    img = np.expand_dims(resize(img, (IMG_HEIGHT, IMG_WIDTH), mode='constant', preserve_range=True),axis=-1)
+    X_test[n] = img
+    prev_msk_file = path+"/prev_mask/"+os.listdir(path+"/prev_mask/")[0]
+    prev_mask = np.zeros((IMG_HEIGHT, IMG_WIDTH, 1), dtype=bool)
+    prev_mask_ = imread(prev_msk_file)
+    prev_mask_ = np.expand_dims(resize(prev_mask_, (IMG_HEIGHT, IMG_WIDTH), mode='constant', 
+                                      preserve_range=True), axis=-1)
+    max_value = np.max(np.max(prev_mask_))
+    prev_mask_ = np.round(np.divide(prev_mask_, np.full(prev_mask_.shape, max_value)))
+    prev_mask_ = np.multiply(prev_mask_, np.full(prev_mask_.shape, max_value))
+    prev_mask = np.maximum(prev_mask, prev_mask_)
+    X_test_mask[n] = prev_mask
+    
+    msk_file = path+"/mask/"+os.listdir(path+"/mask/")[0]
+    mask = np.zeros((IMG_HEIGHT, IMG_WIDTH, 1), dtype=bool)
+    mask_ = imread(msk_file)
+    mask_ = np.expand_dims(resize(mask_, (IMG_HEIGHT, IMG_WIDTH), mode='constant', 
+                                      preserve_range=True), axis=-1)
+            max_value = np.max(np.max(mask_))
+    mask_ = np.round(np.divide(mask_, np.full(mask_.shape, max_value)))
+    mask_ = np.multiply(mask_, np.full(mask_.shape, max_value))
+    mask = np.maximum(mask, mask_)
+    Y_test[n] = mask
+
+# Normalize intensities.
+themax = np.amax(np.concatenate((X_train, X_test)))
+X_train = X_train/themax
+X_test = X_test/themax"""
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        code = """# Tensors for the model to work with
+ycat = tf.keras.utils.to_categorical(Y_train)
+wmap = np.zeros((X_train.shape[0], IMG_HEIGHT, IMG_WIDTH, 2), dtype=np.float32)
+wmap[..., 0] = W_train.squeeze()
+wmap[..., 1] = W_train.squeeze()"""
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """Define loss function and build UNet:"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = """_epsilon = tf.convert_to_tensor(K.epsilon(), np.float32)
+
+def my_loss(target, output):
+    \"\"\"
+    A custom function defined to simply sum the pixelwise loss.
+    This function doesn't compute the crossentropy loss, since that is made a
+    part of the model's computational graph itself.
+    Parameters
+    ----------
+    target : tf.tensor
+        A tensor corresponding to the true labels of an image.
+    output : tf.tensor
+        Model output
+    Returns
+    -------
+    tf.tensor
+        A tensor holding the aggregated loss.
+    \"\"\"
+    return - tf.reduce_sum(target * output,
+                           len(output.get_shape()) - 1)
+
+
+def make_weighted_loss_rescunet(input_shape, n_classes, concatenation_level):
+    # two inputs, one for the image and one for the weight maps
+    ip = tf.keras.Input(shape=input_shape, name="image_input")
+    
+    # the shape of the weight maps has to be such that it can be element-wise
+    # multiplied to the softmax output.
+    weight_ip = tf.keras.Input(shape=input_shape[:2] + (n_classes,))
+    mask_ip = tf.keras.Input(shape=input_shape[:2] + (n_classes,))
+
+    if concatenation_level < 0 or concatenation_level > 4:
+        print("Invalid concatenation level, setting concatenation level to 0.")
+        concatenation_level = 0
+
+    curr_level = 0
+    if concatenation_level == curr_level:
+        in1 = [kl.Concatenate()([ip, mask_ip])
+    else:
+        in1 = [ip]
+        
+    # adding the layers
+    conv1 = L.Conv2D(64, 3, activation='relu', padding='same', kernel_initializer='he_normal')(in1[0])
+    conv1 = L.Conv2D(64, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv1)
+    conv1 = L.Dropout(0.1)(conv1)
+    mpool1 = L.MaxPool2D()(conv1)
+    
+    if concatenation_level > curr_level:
+        # mask convolutions
+        convm1 = kl.Conv2D(64, 3, activation='relu', padding='same', kernel_initializer='he_normal')(mask_ip)
+        convm1 = kl.Conv2D(64, 3, activation='relu', padding='same', kernel_initializer='he_normal')(convm1)
+        convm1 = kl.Dropout(0.1)(convm1)
+        mpoolm1 = kl.MaxPool2D()(convm1)
+
+    curr_level += 1
+    if concatenation_level == curr_level:
+        in2 = [kl.Concatenate()([mpool1, mpoolm1])]
+    else:
+        in2 = [mpool1]
+
+    conv2 = L.Conv2D(128, 3, activation='relu', padding='same', kernel_initializer='he_normal')(in2[0])
+    conv2 = L.Conv2D(128, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv2)
+    conv2 = L.Dropout(0.2)(conv2)
+    mpool2 = L.MaxPool2D()(conv2)
+    
+    if concatenation_level > curr_level:
+        # mask convolutions
+        convm2 = kl.Conv2D(128, 3, activation='relu', padding='same', kernel_initializer='he_normal')(mpoolm1)
+        convm2 = kl.Conv2D(128, 3, activation='relu', padding='same', kernel_initializer='he_normal')(convm2)
+        convm2 = kl.Dropout(0.2)(convm2)
+        mpoolm2 = kl.MaxPool2D()(convm2)
+
+    curr_level += 1
+    if concatenation_level == curr_level:
+        in3 = [kl.Concatenate()([mpool2, mpoolm2])]
+    else:
+        in3 = [mpool2]
+
+    conv3 = L.Conv2D(256, 3, activation='relu', padding='same', kernel_initializer='he_normal')(in3[0])
+    conv3 = L.Conv2D(256, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv3)
+    conv3 = L.Dropout(0.3)(conv3)
+    mpool3 = L.MaxPool2D()(conv3)
+    
+    if concatenation_level > curr_level:
+        # mask convolutions
+        convm3 = kl.Conv2D(256, 3, activation='relu', padding='same', kernel_initializer='he_normal')(mpoolm2)
+        convm3 = kl.Conv2D(256, 3, activation='relu', padding='same', kernel_initializer='he_normal')(convm3)
+        convm3 = kl.Dropout(0.3)(convm3)
+        mpoolm3 = kl.MaxPool2D()(convm3)
+
+    curr_level += 1
+    if concatenation_level == curr_level:
+        in4 = [kl.Concatenate()([mpool3, mpoolm3])]
+    else:
+        in4 = [mpool3]
+
+    conv4 = L.Conv2D(512, 3, activation='relu', padding='same', kernel_initializer='he_normal')(in4[0])
+    conv4 = L.Conv2D(512, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv4)
+    conv4 = L.Dropout(0.4)(conv4)
+    mpool4 = L.MaxPool2D()(conv4)
+    
+    if concatenation_level > curr_level:
+        convm4 = kl.Conv2D(512, 3, activation='relu', padding='same', kernel_initializer='he_normal')(mpoolm3)
+        convm4 = kl.Conv2D(512, 3, activation='relu', padding='same', kernel_initializer='he_normal')(convm4)
+        convm4 = kl.Dropout(0.4)(convm4)
+        mpoolm4 = kl.MaxPool2D()(convm4)
+
+    curr_level += 1
+    if concatenation_level == curr_level:
+        in5 = [kl.Concatenate()([mpool4, mpoolm4])]
+    else:
+        in5 = [mpool4]
+
+    conv5 = L.Conv2D(1024, 3, activation='relu', padding='same', kernel_initializer='he_normal')(in5[0])
+    conv5 = L.Conv2D(1024, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv5)
+    conv5 = L.Dropout(0.5)(conv5)
+
+    up6 = L.Conv2DTranspose(512, 2, strides=2, kernel_initializer='he_normal', padding='same')(conv5)
+    conv6 = L.Concatenate()([up6, conv4])
+    conv6 = L.Conv2D(512, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv6)
+    conv6 = L.Conv2D(512, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv6)
+    conv6 = L.Dropout(0.4)(conv6)
+
+    up7 = L.Conv2DTranspose(256, 2, strides=2, kernel_initializer='he_normal', padding='same')(conv6)
+    conv7 = L.Concatenate()([up7, conv3])
+    conv7 = L.Conv2D(256, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv7)
+    conv7 = L.Conv2D(256, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv7)
+    conv7 = L.Dropout(0.3)(conv7)
+
+    up8 = L.Conv2DTranspose(128, 2, strides=2, kernel_initializer='he_normal', padding='same')(conv7)
+    conv8 = L.Concatenate()([up8, conv2])
+    conv8 = L.Conv2D(128, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv8)
+    conv8 = L.Conv2D(128, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv8)
+    conv8 = L.Dropout(0.2)(conv8)
+
+    up9 = L.Conv2DTranspose(64, 2, strides=2, kernel_initializer='he_normal', padding='same')(conv8)
+    conv9 = L.Concatenate()([up9, conv1])
+    conv9 = L.Conv2D(64, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv9)
+    conv9 = L.Conv2D(64, 3, activation='relu', padding='same', kernel_initializer='he_normal')(conv9)
+    conv9 = L.Dropout(0.1)(conv9)
+
+    c10 = L.Conv2D(n_classes, 1, activation='softmax', kernel_initializer='he_normal', name="unet-activation")(conv9)
+
+    # Add a few non trainable layers to mimic the computation of the crossentropy
+    # loss, so that the actual loss function just has to peform the
+    # aggregation.
+    c11 = L.Lambda(lambda x: x / tf.reduce_sum(x, len(x.get_shape()) - 1, True))(c10)
+    c11 = L.Lambda(lambda x: tf.clip_by_value(x, _epsilon, 1. - _epsilon))(c11)
+    c11 = L.Lambda(lambda x: K.log(x))(c11)
+    weighted_sm = L.multiply([c11, weight_ip])
+
+    model = Model(inputs=[ip, weight_ip, mask_ip], outputs=[weighted_sm])
+    return model"""
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """Create and train ReSCUNet:"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = f"model = make_weighted_loss_rescunet((IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS), 2, CONCATENATION_LEVEL)\n" \
+               f"adam = tf.keras.optimizers.Adam(learning_rate=LEARNING_RATE)\n" \
+               f"model.compile(adam, loss=my_loss)\n" \
+               f"history = model.fit([X_train, wmap, X_train_mask], ycat, batch_size=BATCH_SIZE, epochs=EPOCHS)\n" \
+               f"plt.plot(history.history['loss'])"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """Save and download the model (can be loaded into PyJAMAS):"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = """theclassifier = {
+        
+    'classifier_type': CLASSIFIER_TYPE,
+    'positive_training_folder': TRAIN_PATH,
+    'train_image_size': (IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS),
+    'scaler': themax,
+    'epochs': EPOCHS,
+    'mini_batch_size': BATCH_SIZE,
+    'learning_rate': LEARNING_RATE,
+    'classifier': model.get_weights(),
+}
+
+try:
+    fh = gzip.open('/content/'+MODEL_FILE_NAME, "wb")
+    pickle.dump(theclassifier, fh, PICKLE_PROTOCOL)
+
+except (IOError, OSError) as ex:
+    if fh is not None:
+        fh.close()
+
+fh.close()
+
+from google.colab import files
+files.download('/content/'+MODEL_FILE_NAME)"""
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """Grab output layers for testing here in the notebook:"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = f"image_input = model.get_layer('image_input').input\n" \
+               f"softmax_output = model.get_layer('unet-activation').output\n" \
+               f"predictor = K.function([image_input], [softmax_output])"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        text = """Sample test for the first image in the test set (set ind=i for the (i+1)th image):"""
+        nb['cells'].append(nbf.v4.new_markdown_cell(text))
+
+        code = f"ind = 0\n" \
+               f"testImage = X_test[ind]\n" \
+               f"testPrevMask = X_test_mask[ind]\n" \
+               f"yhat = predictor([testImage.reshape((1, IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS)), testPrevMask.reshape((1, IMG_HEIGHT, IMG_WIDTH, IMG_CHANNELS))])[0]\n" \
+               f"yhat = np.argmax(yhat[0], axis=-1)\n" \
+               f"testLabel = Y_test[ind]\n" \
+               f"weightImage = weight_map(testLabel)\n" \
+               f"fig, (ax1, ax2, ax3, ax4, ax5) = plt.subplots(nrows=1, ncols=5, figsize=(50, 500))\n" \
+               f"ax1.imshow(np.squeeze(testImage), cmap=plt.cm.gray)\n" \
+               f"ax2.imshow(np.squeeze(testPrevMask), cmap=plt.cm.gray)\n" \
+               f"ax3.imshow(np.squeeze(yhat), cmap=plt.cm.gray)\n" \
+               f"ax4.imshow(np.squeeze(testLabel), cmap=plt.cm.gray)\n" \
+               f"ax5.imshow(np.squeeze(weightImage), cmap=plt.cm.gray)"
+        nb['cells'].append(nbf.v4.new_code_cell(code))
+
+        return nb
+
     def cbCreateSVM(self, parameters: Optional[dict] = None, wait_for_thread: bool = False) -> bool:  # Handle IO errors.
         """
         Create a support vector machine classifier.
 
         :param parameters: dictionary containing the parameters to create a logistic regression classifier; a dialog opens if this parameter is set to None; keys are:
 
             ``positive_training_folder``:
@@ -640,46 +1205,122 @@
                                finished_fn=self.finished_fn,  progress_fn=self.progress_fn, stop_fn=self.stop_fn,
                                wait_for_thread=wait_for_thread)
 
             return True
         else:
             return False
 
-    def apply_classifier(self, theslices: numpy.ndarray, progress_signal: ThreadSignals, stop_signal: ThreadSignals) -> bool:
+    def apply_classifier(self, theslices: numpy.ndarray, progress_signal: ThreadSignals,
+                         stop_signal: ThreadSignals) -> bool:
         # Make sure that the slices are in a 1D numpy array.
         theslices = numpy.atleast_1d(theslices)
-        num_slices = theslices.size
 
         if stop_signal is not None:
             stop_signal.emit("Applying classifier ...")
 
-        self.pjs.batch_classifier.predict(self.pjs.slices, theslices, progress_signal)
-
+        if type(self.pjs.batch_classifier.image_classifier) is rimrescunet.ReSCUNet:
+            self.pjs.batch_classifier.predict(self.pjs.slices, theslices, progress_signal, self.pjs.polylines)
+        else:
+            self.pjs.batch_classifier.predict(self.pjs.slices, theslices, progress_signal)
         # For every slice ...
         for index in theslices:
             if type(self.pjs.batch_classifier.image_classifier) in [rimlr.lr, rimsvm.svm]:
                 self.add_classifier_boxes(self.pjs.batch_classifier.box_arrays[index], index, False)
+            elif type(self.pjs.batch_classifier.image_classifier) is rimrescunet.ReSCUNet:
+                self.add_neuralnet_polylines(self.pjs.batch_classifier.object_arrays[index],
+                                             self.pjs.batch_classifier.object_ids[index], index, False)
             elif type(self.pjs.batch_classifier.image_classifier) is rimunet.UNet:
-                self.add_neuralnet_polylines(self.pjs.batch_classifier.object_arrays[index], index, False)
+                self.add_neuralnet_polylines(self.pjs.batch_classifier.object_arrays[index], slice_index=index,
+                                             paint=False)
             else:
                 self.pjs.statusbar.showMessage(f"Wrong classifier type.")
                 return False
 
         return True
 
-    def add_neuralnet_polylines(self, polylines: Optional[numpy.ndarray] = None, slice_index: Optional[int] = None,
-                                paint: bool = True) -> bool:  # The first slice_index should be 0.
+    def cbApplyTrackingClassifier(self, firstSlice: Optional[int] = None, lastSlice: Optional[int] = None,
+                                  wait_for_thread: bool = False) -> bool:    # Handle IO errors.
+        """
+        Apply the current classifier to detect and track objects in the open image. Currently only compatible with
+        ReSCU-Nets, this option will give each polyline mask to the network as individual inputs, rather than the
+        mask including all of the polylines, allowing the network to produce outputs that correspond to each object.
+
+        :param firstSlice: slice number for the first slice to use (minimum is 1); a dialog will open if this parameter is None.
+        :param lastSlice: slice number for the last slice to use; a dialog will open if this parameter is None.
+        :param wait_for_thread: True if PyJAMAS must wait for the thread running this operation to complete, False otherwise.
+        :return: True if the classifier is applied, False if the process is cancelled.
+        """
+        if (firstSlice is False or firstSlice is None or lastSlice is False or lastSlice is None) and self.pjs is not None:
+            dialog = QtWidgets.QDialog()
+            ui = dialogs.timepoints.TimePointsDialog()
+
+            lastSlice = 1 if self.pjs.n_frames == 1 else self.pjs.slices.shape[0]
+            ui.setupUi(dialog, firstslice=self.pjs.curslice + 1, lastslice=lastSlice)
+
+            dialog.exec_()
+            dialog.show()
+            # If the dialog was closed by pressing OK, then run the measurements.
+            continue_flag = dialog.result() == QtWidgets.QDialog.Accepted
+            firstSlice, lastSlice = ui.parameters()
+
+            dialog.close()
+        else:
+            continue_flag = True
+
+        if continue_flag:
+            if firstSlice <= lastSlice:
+                theslicenumbers = numpy.arange(firstSlice - 1, lastSlice, dtype=int)
+            else:
+                theslicenumbers = numpy.arange(lastSlice - 1, firstSlice, dtype=int)
+            print("Launching thread ...")
+            self.launch_thread(self.apply_tracking_classifier,
+                               {'theslices': theslicenumbers, 'progress': True, 'stop': True},
+                               finished_fn=self.finished_fn, progress_fn=self.progress_fn, stop_fn=self.stop_fn,
+                               wait_for_thread=wait_for_thread)
+
+            return True
+        else:
+            return False
+
+    def apply_tracking_classifier(self, theslices: numpy.ndarray, progress_signal: ThreadSignals,
+                                  stop_signal: ThreadSignals) -> bool:
+        # TO DO: test tracking classifier
+        # Make sure that the slices are in a 1D numpy array.
+        theslices = numpy.atleast_1d(theslices)
+
+        if stop_signal is not None:
+            stop_signal.emit("Applying classifier ...")
+        if type(self.pjs.batch_classifier.image_classifier) is rimrescunet.ReSCUNet:
+            print("Applying classifier ...")
+            self.pjs.batch_classifier.predict(self.pjs.slices, theslices, progress_signal, self.pjs.polylines,
+                                              self.pjs.polyline_ids, max(max(self.pjs.polyline_ids)), track=True)
+        else:
+            self.pjs.statusbar.showMessage(f"Wrong classifier type.")
+            return False
+
+        # For every slice ...
+        for index in theslices:
+            self.add_neuralnet_polylines(self.pjs.batch_classifier.object_arrays[index],
+                                         self.pjs.batch_classifier.object_ids[index], index, False)
+
+        return True
+
+    def add_neuralnet_polylines(self, polylines: Optional[numpy.ndarray] = None, ids: Optional[numpy.ndarray] = None,
+                                slice_index: Optional[int] = None, paint: bool = True) -> bool:
         if polylines is None or polylines is False or polylines == []:
             return False
 
         if slice_index is None or slice_index is False:
             slice_index = self.pjs.curslice
 
-        for aPoly in polylines:
-            self.pjs.addPolyline(aPoly, slice_index, paint=paint)
+        for p, aPoly in enumerate(polylines):
+            if ids is None:
+                self.pjs.addPolyline(aPoly, slice_index, paint=paint)
+            else:
+                self.pjs.addPolyline(aPoly, slice_index, theid=ids[p], paint=paint)
 
         return True
 
     def add_classifier_boxes(self, boxes: Optional[numpy.ndarray] = None, slice_index: Optional[int] = None,
                              paint: bool = True) -> bool:  # The first slice_index should be 0.
         if boxes is None or boxes is False or boxes == []:
             return False
```

## pyjamas/rcallbacks/rcbio.py

```diff
@@ -12,40 +12,42 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from copy import deepcopy
 import gzip
 import os
 import pickle
 from typing import List, Optional, Tuple
 
 import cv2
 import numpy
 from PyQt5 import QtWidgets, QtGui, QtCore
 import scipy.io
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
-from tensorflow.keras.models import Model
 
 from pyjamas.external import pascal_voc_io
 from pyjamas.pjscore import PyJAMAS
 from pyjamas.pjscore import undo_modes
 from pyjamas.rcallbacks.rcallback import RCallback
 from pyjamas.rimage.rimml.batchclassifier import BatchClassifier
 from pyjamas.rimage.rimml.batchneuralnet import BatchNeuralNet
 from pyjamas.rimage.rimml.rimclassifier import rimclassifier
 from pyjamas.rimage.rimutils import rimutils
 from pyjamas.rimage.rimml.rimlr import lr
 from pyjamas.rimage.rimml.rimsvm import svm
 from pyjamas.rimage.rimml.rimunet import UNet
 from pyjamas.rutils import RUtils
+from pyjamas.rimage.rimml.classifier_types import classifier_types
+from pyjamas.dialogs.classifiertype import ClassifierTypeDialog
+from pyjamas.rimage.rimml.batchrecurrentneuralnet import BatchRecurrentNeuralNet
+from pyjamas.rimage.rimml.rimrescunet import ReSCUNet
 
 
 class RCBIO(RCallback):
     FILENAME_BASE: str = "cell_"
     FILENAME_FIDUCIAL_LENGTH: int = 5
     DEFAULT_PICKLE_PROTOCOL: int = RUtils.DEFAULT_PICKLE_PROTOCOL
 
@@ -85,14 +87,17 @@
         # Store current working directory.
         self.pjs.cwd = os.path.dirname(filename)  # Path of loaded image.
         self.pjs.filename = filename
 
         # Initialize image and display.
         self.pjs.initImage()
 
+        # Clear and reset classifier object arrays so that the classifier can be applied without reloading from file
+        self.pjs.batch_classifier.reset_objects(self.pjs.n_frames)
+
         return True
 
     def cbLoadArray(self, image: numpy.ndarray) -> bool:
         """
         Load a numpy matrix as an image.
 
         :param image: the array to open.
@@ -103,15 +108,16 @@
 
         self.pjs.slices = image
 
         self.pjs.filename = 'animage'
 
         self.pjs.initImage()
 
-        return True
+        # Clear and reset classifier object arrays so that the classifier can be applied without reloading from file
+        self.pjs.batch_classifier.reset_objects(self.pjs.n_frames)
 
     def cbLoadAnnotations(self, filenames: Optional[List[str]] = None, image_file: Optional[str] = None,
                           replace: bool = True, message: str = "Load annotations ...") -> bool:  # Handle IO errors
         """
         Loads PyJAMAS annotation files.
 
         :param filenames: paths to the files containing the annotations.
@@ -195,15 +201,15 @@
 
             for i in range(len(allpolylines)):
                 allpolylines[i].extend([apolylinelist for apolylinelist in curpolylines[i]])
                 allpolyline_ids[i].extend((numpy.asarray(curpolyline_ids[i]) + maxid).tolist())
 
             max_id_list = [max(slice_ids) for slice_ids in curpolyline_ids if slice_ids]
 
-            # this takes care of the scenario with no polylines defined on any slice.
+            # this takes care of the scenario with no polylines defined on any slice
             if max_id_list:
                 themaxid = max(max_id_list)
                 maxid = max(maxid, themaxid)
 
         if image_file == '':  # Create a blank image.
             # Find maxx, maxy, and maxz, and create a numpy.ndarray with those dimensions + 1.
             maxz = len(allfiducials)
@@ -505,15 +511,15 @@
         :param fiducials: list of fiducials to save (one slice per time point, one row with [x, y] coordinates per fiducial (int)).
         :param pickle_protocol: integer indicating the pickle protocol to use for saving (defaults to RCBIO.DEFAULT_PICKLE_PROTOCOL).
         :param message: string to display as the dialog box title.
         :return: True if the annotations were saved, False otherwise.
         """
 
         # Get file name.
-        if filename is None or filename is False: # When the menu option is clicked on, for some reason that I do not understand, the function is called with filename = False, which causes a bunch of problems.
+        if filename is None or filename is False or filename == '': # When the menu option is clicked on, for some reason that I do not understand, the function is called with filename = False, which causes a bunch of problems.
             fname = QtWidgets.QFileDialog.getSaveFileName(None, message, self.pjs.cwd,
                                                           filter='PyJAMAS data (*' + PyJAMAS.data_extension + ')')  # fname[0] is the full filename, fname[1] is the filter used.
 
             # If cancel ...
             filename = fname[0]
             if filename == '':
                 return False
@@ -690,15 +696,15 @@
         if theclassifier is None or theclassifier is False:
             if self.pjs.batch_classifier.image_classifier is None:
                 return False
             else:
                 theclassifier = self.pjs.batch_classifier.image_classifier
 
         # Get file name.
-        if filename is None or filename is False: # When the menu option is clicked on, for some reason that I do not understand, the function is called with filename = False, which causes a bunch of problems.
+        if filename is None or filename is False:  # When the menu option is clicked on, for some reason that I do not understand, the function is called with filename = False, which causes a bunch of problems.
             fname = QtWidgets.QFileDialog.getSaveFileName(None, message, self.pjs.cwd,
                                                           filter='PyJAMAS classifier (*' + PyJAMAS.classifier_extension + ')')  # fname[0] is the full filename, fname[1] is the filter used.
 
             # If cancel ...
             filename = fname[0]
             if filename == '':
                 return False
@@ -714,30 +720,44 @@
 
         theclassifier.save(filename)
 
         self.pjs.statusbar.showMessage(f'Saved classifier {filename}.')
 
         return True
 
-    def cbLoadClassifier(self, filename: Optional[str] = None, message: str = "Load classifier ...") -> bool:  # Handle IO errors
+    def cbLoadClassifier(self, filename: Optional[str] = None,
+                         message: str = "Load classifier ...") -> bool:  # Handle IO errors
         """
         Load a classifier from disk.
 
         :param filename: name of the file containing a pickled classifier to be loaded.
         :param message: string to display as the dialog box title.
         :return: True if the classifier was loaded, False otherwise.
         """
 
+        filename = self.load_classifier(filename, message)
+
+        if filename is None:
+            return False
+
+        # Modify current path.
+        self.pjs.cwd = os.path.dirname(filename)
+
+        self.pjs.statusbar.showMessage(f"Classifier {filename} loaded.")
+
+        return True
+
+    def load_classifier(self, filename: Optional[str] = None, message: str = "Load classifier ...") -> str:
         # Get file name.
-        if filename is None or filename is False: # When the menu option is clicked on, for some reason that I do not understand, the function is called with filename = False, which causes a bunch of problems.
+        if filename is None or filename is False:
             fname = QtWidgets.QFileDialog.getOpenFileName(None, message, self.pjs.cwd,
                                                           filter='PyJAMAS classifier (*' + PyJAMAS.classifier_extension + ')')  # fname[0] is the full filename, fname[1] is the filter used.
             filename = fname[0]
             if filename == '':
-                return False
+                return None
 
         # Open file name and read classifier.
         fh = None
         theparameters: dict = None
 
         try:
             fh = gzip.open(filename, "rb")
@@ -745,34 +765,67 @@
             fh.close()
 
         except (IOError, OSError) as ex:
             if fh is not None:
                 fh.close()
 
             print(ex)
-            return False
+            return None
 
-        theclassifier = theparameters.get('classifier', None)
-
-        if type(theclassifier) is SVC:
-            self.pjs.batch_classifier = BatchClassifier(self.pjs.n_frames, svm(theparameters))
-        elif type(theclassifier) is LogisticRegression:
-            self.pjs.batch_classifier = BatchClassifier(self.pjs.n_frames, lr(theparameters))
-        elif type(theclassifier) in [list, Model]:
-            self.pjs.batch_classifier = BatchNeuralNet(self.pjs.n_frames, UNet(theparameters))
-        else:
-            self.pjs.statusbar.showMessage(f"Wrong classifier type.")
-            return False
+        if theparameters is None:
+            return None
 
-        # Modify current path.
-        self.pjs.cwd = os.path.dirname(filename)
+        theclassifier = theparameters.get('classifier', None)
+        classifier_type = theparameters.get('classifier_type', None)
 
-        self.pjs.statusbar.showMessage(f"Classifier {filename} loaded.")
+        classifier_identities = set(thetype.value for thetype in classifier_types)
+        loading = True
+        while loading:  # Ask for classifier type until successfully built or cancelled
+            try:
+                if classifier_type == classifier_types.SUPPORT_VECTOR_MACHINE.value and type(theclassifier) == svm:
+                    self.pjs.batch_classifier = BatchClassifier(self.pjs.n_frames, svm(theparameters))
+                elif classifier_type == classifier_types.LOGISTIC_REGRESSION.value and type(theclassifier) == lr:
+                    self.pjs.batch_classifier = BatchClassifier(self.pjs.n_frames, lr(theparameters))
+                elif classifier_type == classifier_types.UNET.value and type(theclassifier) == list:
+                    self.pjs.batch_classifier = BatchNeuralNet(self.pjs.n_frames, UNet(theparameters))
+                elif classifier_type == classifier_types.RESCUNET.value and type(theclassifier) == list:
+                    concatenation_level = theparameters.get('concatenation_level', None)
+                    if concatenation_level is None:  # compatibility with older classifiers without concatenation_level
+                        build_success = False  # Iterate over possible values to find proper construction
+                        concatenation_level = 0
+                        while not build_success and concatenation_level <= 4:
+                            try:
+                                theparameters['concatenation_level'] = concatenation_level
+                                self.pjs.batch_classifier = BatchRecurrentNeuralNet(self.pjs.n_frames, ReSCUNet(theparameters))
+                                build_success = True
+                            except:
+                                concatenation_level += 1
+                        if not build_success:
+                            raise TypeError("Wrong classifier type.")
+                    else:
+                        self.pjs.batch_classifier = BatchRecurrentNeuralNet(self.pjs.n_frames, ReSCUNet(theparameters))
+                else:
+                    raise TypeError("Wrong classifier type.")
+                loading = False  # Passed through if/else's without error so the classifier was loaded, exit the loop
+
+            except:  # Classifier type non-existent, unknown, or incorrect
+                dialog = QtWidgets.QDialog()
+                ui = ClassifierTypeDialog()
+                ui.setupUi(dialog, classifier_type=classifier_types.UNKNOWN.value)
+                dialog.exec_()
+                dialog.show()
+                continue_flag = dialog.result() == QtWidgets.QDialog.Accepted
+                classifier_type = ui.parameters()
+                dialog.close()
+                if not continue_flag:
+                    self.pjs.statusbar.showMessage("Unknown classifier type.")
+                    loading = False  # User cancelled loading, exit loop and return None as filename
+                    filename = None
 
-        return True
+        return filename
 
     def cbExportPolylineAnnotations(self, folder_name: Optional[str] = None) -> bool:
         """
         Set PyJAMAS' annotation mode such that when a fiducial is clicked on, its containing polyline -over time- is stored in a new PyJAMAS annotation file (pickled).
 
         :param folder_name: folder where annotation files will be stored.
         :return: True if the annotation mode was changed, False otherwise.
```

## pyjamas/rimage/rimml/batchclassifier.py

```diff
@@ -79,7 +79,15 @@
                 self.prob_arrays[index],
                 prob_threshold,
                 iou_threshold,
                 max_num_objects
             )
 
         return True
+
+    def reset_objects(self, n_frames: int) -> bool:
+        self.n_frames = n_frames
+        self.prob_arrays = [numpy.empty((1, 0)) for i in range(self.n_frames)]
+        self.box_arrays = [numpy.empty((1, 0)) for i in range(self.n_frames)]
+        self.good_box_indices = [None for i in range(self.n_frames)]
+
+        return True
```

## pyjamas/rimage/rimml/batchml.py

```diff
@@ -37,7 +37,11 @@
     @abstractmethod
     def fit(self, stop_signal: Optional[ThreadSignals] = None) -> bool:
         pass
 
     @abstractmethod
     def predict(self, slices: numpy.ndarray, indices: numpy.ndarray, progress_signal: Optional[ThreadSignals] = None) -> bool:
         pass
+
+    @abstractmethod
+    def reset_objects(self, n_frames: int) -> bool:
+        pass
```

## pyjamas/rimage/rimml/batchneuralnet.py

```diff
@@ -35,15 +35,14 @@
     def fit(self, stop_signal: Optional[ThreadSignals] = None) -> bool:
         if self.image_classifier is None:
             return False
 
         if stop_signal is not None:
             stop_signal.emit('Launching classifier training ...')
 
-
         self.image_classifier.fit()
 
         if stop_signal is not None:
             stop_signal.emit('Classifier training completed.')
         return True
 
     def predict(self, slices: numpy.ndarray, indices: numpy.ndarray, progress_signal: Optional[ThreadSignals] = None) -> bool:
@@ -59,8 +58,15 @@
                 theimage = slices.copy()
 
             self.object_arrays[index], self.prob_arrays[index] = self.image_classifier.predict(theimage)
 
             if progress_signal is not None:
                 progress_signal.emit(int((100 * (i + 1)) / num_slices))
 
-        return True
+        return True
+
+    def reset_objects(self, n_frames: int) -> bool:
+        self.n_frames = n_frames
+        self.object_arrays = [numpy.empty((1, 0)) for i in range(self.n_frames)]
+        self.prob_arrays = [numpy.empty((1, 0)) for i in range(self.n_frames)]
+
+        return True
```

## pyjamas/rimage/rimml/rimclassifier.py

```diff
@@ -78,14 +78,15 @@
         self.object_positions: list = None
         self.object_map: numpy.ndarray = None
         self.box_array: numpy.ndarray = None
         self.prob_array: numpy.ndarray = None
 
     def save(self, filename: str) -> bool:
         theclassifier = {
+            'classifier_type': self.CLASSIFIER_TYPE,
             'positive_training_folder': self.positive_training_folder,
             'negative_training_folder': self.negative_training_folder,
             'hard_negative_training_folder': self.hard_negative_training_folder,
             'train_image_size': self.train_image_size,
             'scaler': self.scaler,
             'fc': self.fc,
             'step_sz': self.step_sz,
```

## pyjamas/rimage/rimml/rimlr.py

```diff
@@ -17,20 +17,22 @@
 """
 
 from typing import Optional
 
 from sklearn.linear_model import LogisticRegression
 
 from pyjamas.rimage.rimml.rimclassifier import rimclassifier
+from pyjamas.rimage.rimml.classifier_types import classifier_types
 
 
 class lr(rimclassifier):
     # Missed class penalty: small values (0.05) result in some additional nuclei detected and others
     # not. Large values (100) do not seem to change the result with respect to 1.0.
     DEFAULT_C: float = 1.0
+    CLASSIFIER_TYPE: str = classifier_types.LOGISTIC_REGRESSION.value
 
     def __init__(self, parameters: Optional[dict] = None):
         super().__init__(parameters)
 
         # LR-specific parameters.
         misclass_penalty_C: float = parameters.get('C', lr.DEFAULT_C)
         self.classifier = parameters.get('classifier', LogisticRegression(C=misclass_penalty_C,
```

## pyjamas/rimage/rimml/rimsvm.py

```diff
@@ -17,18 +17,20 @@
 """
 
 from typing import Optional
 
 from sklearn.svm import SVC
 
 from pyjamas.rimage.rimml.rimclassifier import rimclassifier
+from pyjamas.rimage.rimml.classifier_types import classifier_types
 
 
 class svm(rimclassifier):
     KERNEL_TYPES = ('linear', 'rbf')
+    CLASSIFIER_TYPE: str = classifier_types.SUPPORT_VECTOR_MACHINE.value
 
     DEFAULT_KERNEL_TYPE: int = 1
 
     # Missed class penalty: small values (0.05) result in some additional nuclei detected and others
     # not. Large values (100) do not seem to change the result with respect to 1.0.
     DEFAULT_C: float = 1.0
```

## pyjamas/rimage/rimml/rimunet.py

```diff
@@ -32,19 +32,22 @@
 import tensorflow.keras.utils as ku
 import numpy
 
 import pyjamas.pjscore
 from pyjamas.rimage.rimutils import rimutils
 from pyjamas.rimage.rimml.rimneuralnet import rimneuralnet
 from pyjamas.rutils import RUtils
+from pyjamas.rimage.rimml.classifier_types import classifier_types
 
 
 class UNet(rimneuralnet):
 
     EROSION_WIDTH: int = 7
+    CLASSIFIER_TYPE: str = classifier_types.UNET.value
+    VALIDATION_SPLIT: float = 0.1
 
     def __init__(self, parameters: Optional[dict] = None):
         super().__init__(parameters)
 
         self.W_train: numpy.ndarray = None
 
         output_classes: int = parameters.get('output_classes', UNet.OUTPUT_CLASSES)
@@ -68,15 +71,14 @@
         self.classifier.compile(adam, loss=self.pixelwise_loss)
 
         if type(classifier_representation) is list:
             self.classifier.set_weights(classifier_representation)
 
         self.step_sz = parameters.get('step_sz', UNet.STEP_SIZE)
 
-
     def make_weighted_loss_unet(self, input_shape: Tuple, n_classes: int) -> km.Model:
         _epsilon = tf.convert_to_tensor(kb.epsilon(), numpy.float32)
 
         # two inputs, one for the image and one for the weight maps
         ip = tf.keras.Input(shape=input_shape, name="image_input")
         # the shape of the weight maps has to be such that it can be element-wise
         # multiplied to the softmax output.
@@ -168,15 +170,16 @@
 
         ycat = ku.to_categorical(self.Y_train)
         wmap = numpy.zeros((self.X_train.shape[0], self.train_image_size[0], self.train_image_size[1], 2),
                            dtype=numpy.float32)
         wmap[..., 0] = self.W_train.squeeze()
         wmap[..., 1] = self.W_train.squeeze()
 
-        self.classifier.fit([self.X_train, wmap], ycat, batch_size=self.mini_batch_size, epochs=self.epochs)
+        self.classifier.fit([self.X_train, wmap], ycat, batch_size=self.mini_batch_size, epochs=self.epochs,
+                            validation_split=self.VALIDATION_SPLIT)
 
         return True
 
     @classmethod
     def weight_map(cls, binmasks: numpy.ndarray, w0: float = 10., sigma: float = 5., show: bool = False):
         """Compute the weight map for a given mask, as described in Ronneberger et al.
         (https://arxiv.org/pdf/1505.04597.pdf)
@@ -291,28 +294,29 @@
             (thecol - half_width):(thecol + half_width)] = numpy.logical_or(
                 testLabel[(therow - half_height):(therow + half_height), (thecol - half_width):(thecol + half_width)],
                 yhat)
             testProb[(therow - half_height):(therow + half_height),
             (thecol - half_width):(thecol + half_width)] = p  # This is not really correct: one should select the probability that makes the pixel get its final value (or an average of those).
 
         self.object_array = numpy.asarray(rimutils.extract_contours(
-            sm.dilation(sm.label(sm.binary_erosion(testLabel, sm.square(UNet.EROSION_WIDTH)), connectivity=1),
-                        sm.square(UNet.EROSION_WIDTH))), dtype=object)
+            sm.dilation(sm.label(sm.binary_erosion(testLabel, sm.square(self.EROSION_WIDTH)), connectivity=1),
+                        sm.square(self.EROSION_WIDTH))), dtype=object)
         self.prob_array = testProb
 
         return self.object_array.copy(), self.prob_array.copy()
 
     def save(self, filename: str) -> bool:
         classifier = self.classifier.get_weights() if self.classifier.weights else self.classifier
 
         theclassifier = {
+            'classifier_type': self.CLASSIFIER_TYPE,
             'positive_training_folder': self.positive_training_folder,
             'train_image_size': self.train_image_size,
             'scaler': self.scaler,
             'epochs': self.epochs,
             'mini_batch_size': self.mini_batch_size,
             'learning_rate': kb.eval(self.classifier.optimizer.lr),
             'classifier': self.classifier.get_weights(),
-            'step_sz': self.step_sz
+            'step_sz': self.step_sz,
         }
 
-        return RUtils.pickle_this(theclassifier, RUtils.set_extension(filename, pyjamas.pjscore.PyJAMAS.classifier_extension))
+        return RUtils.pickle_this(theclassifier, RUtils.set_extension(filename, pyjamas.pjscore.PyJAMAS.classifier_extension))
```

## Comparing `pyjamas_rfglab-2023.3.1.dist-info/METADATA` & `pyjamas_rfglab-2023.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjamas-rfglab
-Version: 2023.3.1
+Version: 2023.4.0
 Summary: PyJAMAS is Just A More Awesome SIESTA
 Home-page: https://bitbucket.org/rfg_lab/pyjamas
 Author: Rodrigo Fernandez-Gonzalez
 Author-email: rodrigo.fernandez.gonzalez@utoronto.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `pyjamas_rfglab-2023.3.1.dist-info/RECORD` & `pyjamas_rfglab-2023.4.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 pyjamas/LICENSE,sha256=5lnHvn0CrsS-hm-OcAcksF8MfQhsoOrEfjL3ki8kO3o,33144
 pyjamas/__init__.py,sha256=lip4G10pedUVHvwJHJKaJtz2c9c1gE-Jr72BTgtOCEU,1088
 pyjamas/dragdropmainwindow.py,sha256=aMT3m8HCOGQrvhv1bE0RqAeLT1DOeukzzHrWgjwPgZ8,1793
 pyjamas/orthogonalviewswindow.py,sha256=kr2ieb2mAncVgXDbHfZNclXb_AeDUvAVxUbROG7ttKQ,4901
-pyjamas/pjscore.py,sha256=1xBBPUonGGMl0_vVCBQ9sC8uVaEdA-6YOKYvA3m2hiY,51991
-pyjamas/pjseventfilter.py,sha256=-xQqJFjv4MPzYNwHaOWCiVj8aLdcqZpk5WKBLv65ObQ,32618
+pyjamas/pjscore.py,sha256=UzUnqvNnp1z61UMDfgAtDU7FLiY4LxZwJPaIaD9v74I,52550
+pyjamas/pjseventfilter.py,sha256=EKkqnokHkE3uaN71A1-SQnRgjd46eUwcJNlftBw8T3g,32616
 pyjamas/pjsthreads.py,sha256=9Y-1o6eXH5arV9hVAz6oOzUhqowtE084xtQ2cnle8qk,2123
 pyjamas/pyjamas.tif,sha256=y6WIzNc0BmoETvj1Bm3nk7RT2j-v-DAZyjIzd_V9OJs,2950623
 pyjamas/rutils.py,sha256=gtLoa3ViUkDx_Ba-l0l6bCMDu0zrQjQSRFmByQUxoaE,26659
-pyjamas/dialogs/__init__.py,sha256=9kuh7TuItHyUXTIfCum3Q14fE0awcF7ed6-nI5sMdhg,1586
+pyjamas/dialogs/__init__.py,sha256=O3kC1DwPHthI3izurSb-nCQh1aFY0bdQ9I-CD9iLiuY,1645
 pyjamas/dialogs/adjustcontrast.py,sha256=bCwwQ7uZ4eLoCLFu0Gb5s2EWfVceHBQ0lYcEkpMsAis,17513
 pyjamas/dialogs/batchanalysis.py,sha256=DDBeqnDGy4RKxerE7p2jfRH67n85eOz2rjIfouDG3TY,28797
 pyjamas/dialogs/batchprojectconcat.py,sha256=sCi3Ej2uQJ7KbHfg9I3Z5BQyhUIxwW6kLOhsRkV9z10,5453
+pyjamas/dialogs/batchresize.py,sha256=EysyuYkVsw8EnM2rqPH5iHIkABauCCtg_Qzgzpmvk_E,6858
 pyjamas/dialogs/classifierdialogABC.py,sha256=bHWPznIUqGTSZRWzyjIL3cTaPA6c6JwxKtBv3T0GI9U,2980
+pyjamas/dialogs/classifiertype.py,sha256=6Dt_cngt3c8jmQ-uvfhrA0FJp_s5cTkqkSvCm2TWMtU,3143
 pyjamas/dialogs/expandnpropagateseeds.py,sha256=b8oX0UoW6mGTDuS7djW1UAh9Gw6lpmPhUF3pLw-mTbg,6381
 pyjamas/dialogs/expandseeds.py,sha256=nujXPWg7yQaPmmJD2J2GusVaNNscewizJg2kIAq0v_Q,5171
 pyjamas/dialogs/findseeds.py,sha256=SrLy2ojhgnheAyx8amqpc9tDGjpNM_Hxk8D3qQ5J_TU,12944
 pyjamas/dialogs/logregression.py,sha256=NTHt4d3jy8IeXYbT0lgv2H0VFnZwwtbsNPjKWOA71lE,11319
 pyjamas/dialogs/matplotlibdialog.py,sha256=99nA4yBNQuFovDkvd5z6hz0UCIwo59vnQ_FGpplRmA0,3432
 pyjamas/dialogs/measurepoly.py,sha256=cAeUy_1_HFmJR-BmHoAZpnsUQZtkYjzQtNqhnNHQYa0,8762
 pyjamas/dialogs/neuralnet.py,sha256=1CsVozq1Xf0UJl3oPXnnfXuXUp6ROGpqteg10hRL46M,13235
 pyjamas/dialogs/nonmax_suppr.py,sha256=uAbINvqyzm3NNlL6ysd_tCAjfOqsXPUuroD9BVBE58k,8642
 pyjamas/dialogs/propagateseeds.py,sha256=DIhLIxVDK46n7Fv2Sv4o-vrdaMtmMmyG7pe5uGG4j1k,5477
+pyjamas/dialogs/rescuneuralnet.py,sha256=aIEplv-0h4WEiQ1z2BmQtjfbuzLB2l0Cg_EGL61GcV8,14546
 pyjamas/dialogs/svm.py,sha256=qUMG_aWrJySDksvzXiKF_r-I5duEHzEHFh01c28WlD0,12468
 pyjamas/dialogs/textdialog.py,sha256=MGR-V5aFS3MKz7-n7pyiUkh_8Q5uJ3nSts23J6_cO6Q,2233
 pyjamas/dialogs/timepoints.py,sha256=_Q7OaF_Lqc7v5aN6JL2tzsYUB5c2yAnRx_xn7ubD7SM,4026
 pyjamas/external/__init__.py,sha256=xea2DthoFUDPUqKhn58L_CWoe41alW-b4ncFlZJPnzI,899
 pyjamas/external/pascal_voc_io.py,sha256=a49bKjPyy-HblefUD03MrZrHBgb2FEsGz7TJKjdsBLA,6852
 pyjamas/rannotations/__init__.py,sha256=-CjMXJjy6NfvL87_xr4E6Vo4_XcWROXLk8gbqz2jtZw,924
 pyjamas/rannotations/rannotation.py,sha256=1seVrj5Eg3qoKaIqgYf52iaC1-oIhy7crVbvvxaTZrs,856
 pyjamas/rannotations/rpolyline.py,sha256=eywU1IKuKz_WyS-JlFokuAJGsiB6vfo47gSYqMaKfL0,16818
 pyjamas/rannotations/rvector2d.py,sha256=xxiMcZJoOcWYSqStXMGSmZ-8w6dJ5sLFvGOXhzV3v7s,2288
 pyjamas/rcallbacks/__init__.py,sha256=nDUzAAJB-nFcJcZtjvPAJWyMUMsVZ87wgrrf3OPAaOw,1257
 pyjamas/rcallbacks/rcallback.py,sha256=Sh4JHfVH8uYc4b9552hr3ME3MXkukk9mmvDc5MaXP2M,7696
 pyjamas/rcallbacks/rcbabout.py,sha256=XJa5jfvUqcbad12kcGrTl7GHBNRD8T007YAY5TYOt0U,1658
 pyjamas/rcallbacks/rcbannotations.py,sha256=XnhydIBklWTZMLTF3xjGgchkigmasAL0-Wm9p6aolLQ,13560
-pyjamas/rcallbacks/rcbbatchprocess.py,sha256=GP-svvROOTJ-lQIuIt3U0NMZZfk9ItcKyuaBgP5q1Y8,66708
-pyjamas/rcallbacks/rcbclassifiers.py,sha256=mWLr-ies32AU0R2BNTubn6RDb2alCAHbIwgvvp8Fsyw,35409
+pyjamas/rcallbacks/rcbbatchprocess.py,sha256=6-5HpTi2WBW9LFxsjf5WtOz3SNqq7E4Dm3vFykey6oA,70337
+pyjamas/rcallbacks/rcbclassifiers.py,sha256=slLc9aSxGKtGtYtp5foK87QG7kqYRZRSPczXKbp0Hw8,66441
 pyjamas/rcallbacks/rcbimage.py,sha256=RqYe1yAPKhrHhbHazftNc5YQ4WjqB8192s9XYLFWO1g,77409
-pyjamas/rcallbacks/rcbio.py,sha256=B97kq58XPoXiWQrZ7fTOjnRhXzddlT5FnaObt2Mqg_c,49461
+pyjamas/rcallbacks/rcbio.py,sha256=y_CJUPB1L3sjPnAii0Z-VALoiT97d2b28opBr2v11YY,52706
 pyjamas/rcallbacks/rcbmeasure.py,sha256=tEODUbQjwMaK9bTYxgqzvwYGSuNF1H9CqfcCpSxEopw,11288
 pyjamas/rcallbacks/rcboptions.py,sha256=J_-0EodMho_FyFMeG_BFMReClEm42ulis_lb9pLblfs,12556
 pyjamas/rcallbacks/rcbplugins.py,sha256=bRbOJ7zMPCTzjKJk3jnYTEEJrCIYP3geh_iWfrIA_Hk,3617
 pyjamas/rimage/__init__.py,sha256=BiL1mv2uql78UIxsar5UzSQMDFRy0JQskioHL4kW-a4,913
 pyjamas/rimage/csgraph.py,sha256=rMu8OgTx-uvIaRM78KGug7T_KEVLE4xWSkTo4CxFQQo,3091
 pyjamas/rimage/rimcore.py,sha256=50mFbTaUxQMiORfds4VPRudZF5RRUD-8COtlVFzmlkw,3799
 pyjamas/rimage/rimutils.py,sha256=gchln7rOvOyQloroWEN8IexcApa4WcCUNkgRR5Fto3o,67158
 pyjamas/rimage/rimml/__init__.py,sha256=O5rqK4O5d96Y61cB_6PbmmvG2HQuUcHO4xpALn-z3fE,1484
-pyjamas/rimage/rimml/batchclassifier.py,sha256=oPB2qoTygrpSbtuk2fgT1qUwdbmx6__wJOdKJdeOMbQ,3224
-pyjamas/rimage/rimml/batchml.py,sha256=rC1HLq_z9s5Sbup-SAVwJYgpOvLPS2mWR4rjr5VctBY,1499
-pyjamas/rimage/rimml/batchneuralnet.py,sha256=v83wVFo8mU36sO8yqEDA7S6z3mhiHIvrpvB-kSJdXhs,2473
+pyjamas/rimage/rimml/batchclassifier.py,sha256=WwjxeNy2uTF5sKhrific48uMAN64QzOLFiVlNhXy-5g,3557
+pyjamas/rimage/rimml/batchml.py,sha256=3cdNyWRtJ8FjB3yi9jjoY_kgN89e_lh32aAep1GhYjk,1585
+pyjamas/rimage/rimml/batchneuralnet.py,sha256=HCnm71qYfUZQlQhAyrmTZdW7IuQT2PShYxEheHktCjU,2740
+pyjamas/rimage/rimml/batchrecurrentneuralnet.py,sha256=ZEqDYU_1M4vbACOnUWKLRBkg6ULftzk-DWy0ILYMF78,7409
+pyjamas/rimage/rimml/classifier_types.py,sha256=SbDTTr5jh4In_pnHthUs0MCSJQvWc6E_dl3HVc7FLEQ,275
 pyjamas/rimage/rimml/featurecalculator.py,sha256=y8N9ug8RtvhEuJYDvVRGYVpC-yoSkiQDxFm9zTkIpAw,1173
 pyjamas/rimage/rimml/featurecalculator_rawimage.py,sha256=AS6NlAH9XINAR1rx7aeC2gOrlkVW1rQZlnK8w9EoF70,1387
 pyjamas/rimage/rimml/featurecalculator_rowofpixels.py,sha256=JNfu-6UYGpQo2KQrfqwP2kHN4XwkKvUoTpkOpMdJDek,1289
 pyjamas/rimage/rimml/featurecalculator_sog.py,sha256=j_VTupYS9DQz7hBXAIioCRli5mZ01Nr3Qb7-BaqSN00,3196
-pyjamas/rimage/rimml/rimclassifier.py,sha256=Zmm_nEGCLCrVsZz731zaV5PzbSOm1V-dPY5dMJcaVdA,17286
-pyjamas/rimage/rimml/rimlr.py,sha256=p2-mk6lN2gnIpMgEUGUwKuEH2mu1mHjxO_g7TScKweQ,1687
+pyjamas/rimage/rimml/rimclassifier.py,sha256=Kw56mewnfaRWtBJGK0q9mZpi7Sgnzl7-2iUYP8O5CJc,17339
+pyjamas/rimage/rimml/rimlr.py,sha256=-M6mrwJn9zwbbZ9J9ceCsv0d2Au4KUPA_-hRyCCXAok,1824
 pyjamas/rimage/rimml/rimml.py,sha256=9wm8gufvWLuszQpbEEBQJSP6Rzwex2owaZbwUYjj3-I,1382
 pyjamas/rimage/rimml/rimneuralnet.py,sha256=k6BrG7gcsgG08GTKs8FfZ37JUGqOLSaMxI7vOH9umAk,1857
-pyjamas/rimage/rimml/rimsvm.py,sha256=BWzFeAVlkp-RNVO-EVSgvPqysfDmO2sgP8FpSBAb_Ow,1944
-pyjamas/rimage/rimml/rimunet.py,sha256=Ihw9YPAX_FphTjFf-nEz_MToACgVrJ0X6CvIOoTc3Ko,14859
+pyjamas/rimage/rimml/rimrecurrentneuralnet.py,sha256=MIM6IgqC-lbXiYcLjJEWPNRqYUu7Cv8nmsuZh2Zc4Xo,1960
+pyjamas/rimage/rimml/rimrescunet.py,sha256=xv0BDhFwfKl-EQl6lC0nQkVrLHLmYr-3cVfGdy6u_9c,20936
+pyjamas/rimage/rimml/rimsvm.py,sha256=ZXYAwbWL2I39nDmXXqntbXRX0AwCBu8uda-XRiODtKk,2084
+pyjamas/rimage/rimml/rimunet.py,sha256=K-feheZFy9IEf3TnIpyzkc5OunID0lqsxjfbndmCqyQ,15137
 pyjamas/rplugins/__init__.py,sha256=aHh9B0OVLt-7rJyyoXV0t7NMoziJODn279yaHZrF5h4,847
 pyjamas/rplugins/base.py,sha256=d1zP7iq85pkTgAQMnF39XILFJ2xE7Thdr0qlLEUQ0zU,1249
 pyjamas/tests/__init__.py,sha256=8l38RxqL4YvU35uHcp58t2qPDGy7nUgHz8sXpVr_X3A,796
 pyjamas/tests/conftest.py,sha256=Mi4BlSPuKkO4QBPpE6fh8K8jSrPq6Vr4TgqricNrnJo,857
 pyjamas/tests/unit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyjamas/tests/unit/pjsfixtures.py,sha256=lP0BFH_xPQiBO7ykUTYhUsx7SpXtLVGfCsLWwMy2E5g,5912
 pyjamas/tests/unit/test_image.py,sha256=rwx2XM8dPDIMoN_3PMAadC51Qh-llFDVoCAKodt-a38,11195
 pyjamas/tests/unit/test_io.py,sha256=u3v_uKXuCAPKpj9S8GvwERGFkq916m02RNEcsFVxs_U,17400
-pyjamas_rfglab-2023.3.1.dist-info/METADATA,sha256=bALvOdjUy7WB0fSarS0h9MRzDSKqr-lDxu75Sz7RJBk,8308
-pyjamas_rfglab-2023.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyjamas_rfglab-2023.3.1.dist-info/entry_points.txt,sha256=Kz2XxZBSSzrf8qtxDZPgWAw2aV48mIiIL1tLbMpFfV0,50
-pyjamas_rfglab-2023.3.1.dist-info/top_level.txt,sha256=1JrBnRcgMVjhVrxaCoReIJTpPg7PPqhjjzehykIDu_A,8
-pyjamas_rfglab-2023.3.1.dist-info/RECORD,,
+pyjamas_rfglab-2023.4.0.dist-info/METADATA,sha256=s3jFmeqJAI6NFSWrltIPLKH3XFgT1532QQuXjFNvaW0,8308
+pyjamas_rfglab-2023.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyjamas_rfglab-2023.4.0.dist-info/entry_points.txt,sha256=Kz2XxZBSSzrf8qtxDZPgWAw2aV48mIiIL1tLbMpFfV0,50
+pyjamas_rfglab-2023.4.0.dist-info/top_level.txt,sha256=1JrBnRcgMVjhVrxaCoReIJTpPg7PPqhjjzehykIDu_A,8
+pyjamas_rfglab-2023.4.0.dist-info/RECORD,,
```

