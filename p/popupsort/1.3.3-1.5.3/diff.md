# Comparing `tmp/popupsort-1.3.3.tar.gz` & `tmp/popupsort-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popupsort-1.3.3.tar", last modified: Sun Apr  9 15:48:13 2023, max compression
+gzip compressed data, was "popupsort-1.5.3.tar", last modified: Wed Apr 12 15:22:34 2023, max compression
```

## Comparing `popupsort-1.3.3.tar` & `popupsort-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 15:48:13.678715 popupsort-1.3.3/
--rw-rw-rw-   0        0        0     1093 2023-03-18 09:14:08.000000 popupsort-1.3.3/LICENSE.md
--rw-rw-rw-   0        0        0     2552 2023-04-09 15:48:13.679725 popupsort-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1785 2023-04-09 15:41:22.000000 popupsort-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 15:48:13.663776 popupsort-1.3.3/popupsort/
--rw-rw-rw-   0        0        0       41 2023-03-18 09:14:08.000000 popupsort-1.3.3/popupsort/__init__.py
--rw-rw-rw-   0        0        0     9991 2023-04-09 15:47:57.000000 popupsort-1.3.3/popupsort/popupsort.py
-drwxrwxrwx   0        0        0        0 2023-04-09 15:48:13.677717 popupsort-1.3.3/popupsort.egg-info/
--rw-rw-rw-   0        0        0     2552 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 09:46:14.000000 popupsort-1.3.3/popupsort.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 15:48:13.680709 popupsort-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-04-09 15:48:06.000000 popupsort-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:22:34.349575 popupsort-1.5.3/
+-rw-rw-rw-   0        0        0     1093 2023-03-18 09:14:08.000000 popupsort-1.5.3/LICENSE.md
+-rw-rw-rw-   0        0        0     2552 2023-04-12 15:22:34.349575 popupsort-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1785 2023-04-09 15:41:22.000000 popupsort-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 15:22:34.330513 popupsort-1.5.3/popupsort/
+-rw-rw-rw-   0        0        0       74 2023-04-12 15:13:39.000000 popupsort-1.5.3/popupsort/__init__.py
+-rw-rw-rw-   0        0        0    15518 2023-04-12 15:22:19.000000 popupsort-1.5.3/popupsort/popupsort.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:22:34.347581 popupsort-1.5.3/popupsort.egg-info/
+-rw-rw-rw-   0        0        0     2552 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-18 09:46:14.000000 popupsort-1.5.3/popupsort.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:22:34.350573 popupsort-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      574 2023-04-12 15:22:28.000000 popupsort-1.5.3/setup.py
```

### Comparing `popupsort-1.3.3/LICENSE.md` & `popupsort-1.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `popupsort-1.3.3/PKG-INFO` & `popupsort-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popupsort
-Version: 1.3.3
+Version: 1.5.3
 Summary: A Python package for visualizing sorting algorithms
 Home-page: https://github.com/ZouheirN/PopUpSort
 Author: Zouheir Nakouzi
 Author-email: zouheir2002@gmail.com
 License: MIT
 Description: # PopUpSort
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: popupsort Version: 1.3.3 Summary: A Python package
+Metadata-Version: 2.1 Name: popupsort Version: 1.5.3 Summary: A Python package
 for visualizing sorting algorithms Home-page: https://github.com/ZouheirN/
 PopUpSort Author: Zouheir Nakouzi Author-email: zouheir2002@gmail.com License:
 MIT Description: # PopUpSort
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 With the assistance of ChatGPT-3.5, I was able to create this sorting
 visualizer. The PopUpSort package is a Python package that visualizes the
```

### Comparing `popupsort-1.3.3/README.md` & `popupsort-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `popupsort-1.3.3/popupsort/popupsort.py` & `popupsort-1.5.3/popupsort/popupsort.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 import random
+import re
 import time
 from tkinter import *
 
 
 class SortingVisualizer:
     def __init__(self, arr, speed):
+
         if not isinstance(arr, list):
             raise TypeError("Input array must be a list")
 
         if speed < 0:
             raise ValueError("Speed must be a non-negative value")
 
         self.arr = arr
         self.n = len(arr)
         self.window = Tk()
         self.window.title("PopUpSort")
-        self.window.geometry("600x450")
+        # self.window.geometry("620x480")
         self.window.resizable(False, False)  # disables resizing in both directions
 
+        window_width = 620
+        window_height = 480
+        x = int(int(self.window.winfo_screenwidth() / 2) - int(window_width / 2))
+        y = int(int(self.window.winfo_screenheight() / 2) - int(window_height / 2))
+        self.window.geometry(f"{window_width}x{window_height}+{x}+{y}")
+
+        self.label = Label(self.window, text="", font=("Helvetica", 16))
+        self.label.pack()
+
         self.canvas = Canvas(self.window, width=600, height=400)
         self.canvas.pack()
 
+        self.total_time = None
+
         self.time_label = Label(self.window, text="Elapsed Time: 0.000s", fg="black", font=("Helvetica", 16))
         self.time_label.pack(side=BOTTOM)
 
         if self.n == 0:
             raise ValueError("Cannot visualize an empty array")
 
         self.draw_array(self.arr, color='blue')
@@ -35,14 +48,17 @@
         self.update_timer()
 
     def update_timer(self):
         self.elapsed_time = time.time() - self.start_time
 
         if self.timer_stopped:
             self.time_label.config(fg='green2')
+            text = self.time_label.cget("text")
+            match = re.search(r'\d+\.\d+', text)
+            self.total_time = float(match.group())
             return
         else:
             self.time_label.config(text="Elapsed Time: {:.3f}s".format(self.elapsed_time))
             self.window.after(10, self.update_timer)
 
     def draw_array(self, arr, color, highlight=None):
         if highlight is None:
@@ -70,18 +86,19 @@
 
             self.canvas.create_rectangle(x0, y0, x1, y1, fill=current_color)
 
             # draw the label under the rectangle with the adjusted font size
             label_x = (x0 + x1) / 2
             label_y = y1 + 25 if i % 2 else y1 + 15
 
-            self.canvas.create_text(label_x, label_y, text=str(self.arr[i]), font=("Arial", font_size))
+            self.canvas.create_text(label_x, label_y, text=str(self.arr[i]), font=("Helvetica", font_size))
 
             # draw a line pointing to the rectangle
-            self.canvas.create_line(label_x, -5 + label_y - font_size // 2, label_x, y0 + (y1 - y0) + font_size // 2, width=1)
+            self.canvas.create_line(label_x, -5 + label_y - font_size // 2, label_x, y0 + (y1 - y0) + font_size // 2,
+                                    width=1)
 
         self.window.update()
 
     def bubble_sort(self):
         for i in range(self.n):
             for j in range(0, self.n - i - 1):
                 if self.arr[j] > self.arr[j + 1]:
@@ -248,45 +265,177 @@
         self.window.mainloop()
 
 
 def sort(arr, algorithm, speed=0.01):
     sv = SortingVisualizer(arr, speed)
 
     if algorithm.lower() == 'bubble sort' or algorithm.lower() == 'b':
+        sv.label.config(text="Bubble Sort")
         sv.bubble_sort()
     elif algorithm.lower() == 'selection sort' or algorithm.lower() == 's':
+        sv.label.config(text="Selection Sort")
         sv.selection_sort()
     elif algorithm.lower() == 'insertion sort' or algorithm.lower() == 'i':
+        sv.label.config(text="Insertion Sort")
         sv.insertion_sort()
     elif algorithm.lower() == 'quick sort' or algorithm.lower() == 'q':
+        sv.label.config(text="Quick Sort")
         sv.quick_sort()
     elif algorithm.lower() == 'merge sort' or algorithm.lower() == 'm':
+        sv.label.config(text="Merge Sort")
         sv.merge_sort()
     elif algorithm.lower() == 'heap sort' or algorithm.lower() == 'h':
+        sv.label.config(text="Heap Sort")
         sv.heap_sort(arr)
         sv.completed()
     elif algorithm.lower() == 'shell sort' or algorithm.lower() == 'sh':
+        sv.label.config(text="Shell Sort")
         sv.shell_sort()
 
+    return '%.3f' % sv.total_time + 's'
+
 
 def sort_rand(size, min, max, algorithm, speed=0.01):
     arr = []
     for i in range(size):
         arr.append(random.randint(min, max))
 
     sv = SortingVisualizer(arr, speed)
 
     if algorithm.lower() == 'bubble sort' or algorithm.lower() == 'b':
+        sv.label.config(text="Bubble Sort")
         sv.bubble_sort()
     elif algorithm.lower() == 'selection sort' or algorithm.lower() == 's':
+        sv.label.config(text="Selection Sort")
         sv.selection_sort()
     elif algorithm.lower() == 'insertion sort' or algorithm.lower() == 'i':
+        sv.label.config(text="Insertion Sort")
         sv.insertion_sort()
     elif algorithm.lower() == 'quick sort' or algorithm.lower() == 'q':
+        sv.label.config(text="Quick Sort")
         sv.quick_sort()
     elif algorithm.lower() == 'merge sort' or algorithm.lower() == 'm':
+        sv.label.config(text="Merge Sort")
         sv.merge_sort()
     elif algorithm.lower() == 'heap sort' or algorithm.lower() == 'h':
+        sv.label.config(text="Heap Sort")
         sv.heap_sort(arr)
         sv.completed()
     elif algorithm.lower() == 'shell sort' or algorithm.lower() == 'sh':
-        sv.shell_sort()
+        sv.label.config(text="Shell Sort")
+        sv.shell_sort()
+
+    return '%.3f' % sv.total_time + 's'
+
+
+def sort_compare(arr, algorithms, speed=0.01):
+    arr_copy = []
+
+    for i in range(len(algorithms)):
+        arr_copy.append(arr.copy())
+
+    sv = []
+
+    for i in range(len(algorithms)):
+        sv.append(sort(arr_copy[i], algorithms[i], speed))
+
+    for i in range(len(algorithms)):
+        if algorithms[i].lower() == 'insertion sort' or algorithms[i].lower() == 'i':
+            algorithms[i] = 'Insertion Sort'
+        elif algorithms[i].lower() == 'bubble sort' or algorithms[i].lower() == 'b':
+            algorithms[i] = 'Bubble Sort'
+        elif algorithms[i].lower() == 'selection sort' or algorithms[i].lower() == 's':
+            algorithms[i] = 'Selection Sort'
+        elif algorithms[i].lower() == 'merge sort' or algorithms[i].lower() == 'm':
+            algorithms[i] = 'Merge Sort'
+        elif algorithms[i].lower() == 'heap sort' or algorithms[i].lower() == 'h':
+            algorithms[i] = 'Heap Sort'
+        elif algorithms[i].lower() == 'quick sort' or algorithms[i].lower() == 'q':
+            algorithms[i] = 'Quick Sort'
+        elif algorithms[i].lower() == 'shell sort' or algorithms[i].lower() == 'sh':
+            algorithms[i] = 'Shell Sort'
+
+    window = Tk()
+
+    window.title("PopUpSort - Comparison Results")
+
+    window_width = 130 * len(sv)
+    window_height = 100
+    x = int(int(window.winfo_screenwidth() / 2) - int(window_width / 2))
+    y = int(int(window.winfo_screenheight() / 2) - int(window_height / 2))
+    window.geometry(f"{window_width}x{window_height}+{x}+{y}")
+
+    window.resizable(False, False)
+
+    for i in range(len(algorithms)):
+        frame = Frame(window)
+        frame.pack(side="left", padx=15, pady=20)
+
+        label = Label(frame, text=algorithms[i], font=("Helvetica", 12))
+        label.pack(side="top")
+
+        text = Label(frame, text=sv[i], font=("Helvetica", 12))
+        text.pack(side="bottom")
+
+        frame2 = Frame(frame, width=100, height=100)
+        frame2.pack()
+
+    window.mainloop()
+
+
+def sort_compare_rand(size, min, max, algorithms, speed=0.01):
+    arr = []
+    for i in range(size):
+        arr.append(random.randint(min, max))
+
+    arr_copy = []
+
+    for i in range(len(algorithms)):
+        arr_copy.append(arr.copy())
+
+    sv = []
+
+    for i in range(len(algorithms)):
+        sv.append(sort(arr_copy[i], algorithms[i], speed))
+
+    for i in range(len(algorithms)):
+        if algorithms[i].lower() == 'insertion sort' or algorithms[i].lower() == 'i':
+            algorithms[i] = 'Insertion Sort'
+        elif algorithms[i].lower() == 'bubble sort' or algorithms[i].lower() == 'b':
+            algorithms[i] = 'Bubble Sort'
+        elif algorithms[i].lower() == 'selection sort' or algorithms[i].lower() == 's':
+            algorithms[i] = 'Selection Sort'
+        elif algorithms[i].lower() == 'merge sort' or algorithms[i].lower() == 'm':
+            algorithms[i] = 'Merge Sort'
+        elif algorithms[i].lower() == 'heap sort' or algorithms[i].lower() == 'h':
+            algorithms[i] = 'Heap Sort'
+        elif algorithms[i].lower() == 'quick sort' or algorithms[i].lower() == 'q':
+            algorithms[i] = 'Quick Sort'
+        elif algorithms[i].lower() == 'shell sort' or algorithms[i].lower() == 'sh':
+            algorithms[i] = 'Shell Sort'
+
+    window = Tk()
+
+    window.title("PopUpSort - Comparison Results")
+
+    window_width = 130 * len(sv)
+    window_height = 100
+    x = int(int(window.winfo_screenwidth() / 2) - int(window_width / 2))
+    y = int(int(window.winfo_screenheight() / 2) - int(window_height / 2))
+    window.geometry(f"{window_width}x{window_height}+{x}+{y}")
+
+    window.resizable(False, False)
+
+    for i in range(len(algorithms)):
+        frame = Frame(window)
+        frame.pack(side="left", padx=15, pady=20)
+
+        label = Label(frame, text=algorithms[i], font=("Helvetica", 12))
+        label.pack(side="top")
+
+        text = Label(frame, text=sv[i], font=("Helvetica", 12))
+        text.pack(side="bottom")
+
+        frame2 = Frame(frame, width=100, height=100)
+        frame2.pack()
+
+    window.mainloop()
```

### Comparing `popupsort-1.3.3/popupsort.egg-info/PKG-INFO` & `popupsort-1.5.3/popupsort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popupsort
-Version: 1.3.3
+Version: 1.5.3
 Summary: A Python package for visualizing sorting algorithms
 Home-page: https://github.com/ZouheirN/PopUpSort
 Author: Zouheir Nakouzi
 Author-email: zouheir2002@gmail.com
 License: MIT
 Description: # PopUpSort
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: popupsort Version: 1.3.3 Summary: A Python package
+Metadata-Version: 2.1 Name: popupsort Version: 1.5.3 Summary: A Python package
 for visualizing sorting algorithms Home-page: https://github.com/ZouheirN/
 PopUpSort Author: Zouheir Nakouzi Author-email: zouheir2002@gmail.com License:
 MIT Description: # PopUpSort
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 With the assistance of ChatGPT-3.5, I was able to create this sorting
 visualizer. The PopUpSort package is a Python package that visualizes the
```

### Comparing `popupsort-1.3.3/setup.py` & `popupsort-1.5.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='popupsort',
-    version='1.3.3',
+    version='1.5.3',
     description='A Python package for visualizing sorting algorithms',
     long_description = README,
     long_description_content_type="text/markdown",
     author='Zouheir Nakouzi',
     author_email='zouheir2002@gmail.com',
     url='https://github.com/ZouheirN/PopUpSort',
     packages=['popupsort'],
```

