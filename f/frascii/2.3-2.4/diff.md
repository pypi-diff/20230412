# Comparing `tmp/frascii-2.3.tar.gz` & `tmp/frascii-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-2.3.tar", last modified: Tue Apr 11 13:54:48 2023, max compression
+gzip compressed data, was "frascii-2.4.tar", last modified: Wed Apr 12 12:35:18 2023, max compression
```

## Comparing `frascii-2.3.tar` & `frascii-2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.322233 frascii-2.3/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-11 13:54:48.322233 frascii-2.3/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12240 2023-04-07 11:54:45.000000 frascii-2.3/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.318233 frascii-2.3/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1533 2023-04-11 13:54:36.000000 frascii-2.3/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     6323 2023-03-07 12:42:34.000000 frascii-2.3/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.322233 frascii-2.3/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.3/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.3/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.3/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.3/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.3/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      744 2023-02-28 13:56:01.000000 frascii-2.3/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.3/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2562 2023-04-11 13:53:30.000000 frascii-2.3/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      609 2023-02-24 15:05:19.000000 frascii-2.3/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.3/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.3/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.3/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.3/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.318233 frascii-2.3/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-11 13:54:48.322233 frascii-2.3/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.3/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.960043 frascii-2.4/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-12 12:35:18.960043 frascii-2.4/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12240 2023-04-07 11:54:45.000000 frascii-2.4/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.956043 frascii-2.4/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1533 2023-04-12 12:35:12.000000 frascii-2.4/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     6323 2023-03-07 12:42:34.000000 frascii-2.4/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.960043 frascii-2.4/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.4/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.4/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.4/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.4/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.4/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      744 2023-02-28 13:56:01.000000 frascii-2.4/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.4/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.4/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      609 2023-02-24 15:05:19.000000 frascii-2.4/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.4/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.4/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.4/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.4/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.956043 frascii-2.4/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-12 12:35:18.960043 frascii-2.4/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.4/setup.py
```

### Comparing `frascii-2.3/README.md` & `frascii-2.4/README.md`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/__init__.py` & `frascii-2.4/frascii/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '2.3'
+__version__ = '2.4'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter):
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter):
 	return julia_string(f, x, y, x_radius, y_radius, stepsize, max_iter)
```

### Comparing `frascii-2.3/frascii/commands.py` & `frascii-2.4/frascii/commands.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/dragon_curve.py` & `frascii-2.4/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/fibonacci.py` & `frascii-2.4/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/hilbert_curve.py` & `frascii-2.4/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/julia.py` & `frascii-2.4/frascii/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/koch.py` & `frascii-2.4/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/l_system.py` & `frascii-2.4/frascii/fractals/l_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 def l_system(start, rules, n):
 	letters = start
 	rules = rules.replace("(", "").replace(")", "").replace(" ", "").split(",")
 	rules = dict(rule.split("->") for rule in rules)
 	for i in range(n):
 		letters = "".join(rules[l] if l in rules else l for l in letters)
-	return "".join(l for l in letters if l in "+-Ff")
+	return "".join(l for l in letters if l in "+-Ff[]")
 	
 
 def cleanup(arr):
 	if all(seg == "  " for seg in arr[0]):
 		arr = arr[1:]
 	if all(seg == "  " for seg in arr[-1]):
 		arr = arr[:-1]
@@ -18,14 +18,15 @@
 		arr = [row[:-1] for row in arr]
 	return arr
 
 def l_system_string(start, rules, n, start_dir="U"):
 	letters = l_system(start, rules, n)
 	out = [["URDL"]]
 	pos = [0, 0]  #y, x
+	pos_stack = []
 	comp = "URDL"
 	if start_dir not in "URDL":
 		raise ValueError(f"start_dir must be U,R,D or L but was {start_dir}")
 	while comp[0] != start_dir:
 		comp = comp[1:] + comp[0]
 	prev_comp = comp
 	buff = ""
@@ -36,17 +37,19 @@
 		if pos[0] == len(out) - 1:
 			out.append(["URDL" for i in range(len(out[0]))])
 		if pos[1] == len(out[0]) - 1:
 			out = [row + ["URDL"] for row in out]
 		if pos[0] == 0:
 			out.insert(0, ["URDL" for i in range(len(out[0]))])
 			pos[0] = 1
+			pos_stack = [[[p[0][0]+1, p[0][1]], p[1]] for p in pos_stack]
 		if pos[1] == 0:
 			out = [["URDL"] + row for row in out]
-			pos[1] = 1	
+			pos[1] = 1
+			pos_stack = [[[p[0][0], p[0][1]+1], p[1]] for p in pos_stack]
 
 		curr = out[pos[0]][pos[1]]
 		if turn == "-":
 			comp = comp[1:] + comp[0]
 
 		elif turn == "+":
 			comp = comp[-1] + comp[:-1]
@@ -62,28 +65,37 @@
 			elif comp[0] == "D":
 				pos[0] += 1
 			elif comp[0] == "L":
 				pos[1] -= 1
 			if turn == "F":
 				out[pos[0]][pos[1]] = out[pos[0]][pos[1]].replace(comp[2], "")
 
+		elif turn == "[":
+			pos_stack.append([[pos[0], pos[1]], comp])
+
+		elif turn == "]":
+			pos, comp = pos_stack.pop()
+
+
 	# Enlarge grid
 	if pos[0] == len(out) - 1:
 		out.append(["URDL" for i in range(len(out[0]))])
 	if pos[1] == len(out[0]) - 1:
 		out = [row + ["URDL"] for row in out]
 	if pos[0] == 0:
 		out.insert(0, ["URDL" for i in range(len(out[0]))])
 		pos[0] = 1
+		pos_stack = [[[p[0][0]+1, p[0][1]], p[1]] for p in pos_stack]
 	if pos[1] == 0:
 		out = [["URDL"] + row for row in out]
 		pos[1] = 1	
+		pos_stack = [[[p[0][0], p[0][1]+1], p[1]] for p in pos_stack]
 
 	trans = {"URDL": "  ", "URD": "╴ ", "URL": "╷ ", "UDL": "╶─",
 			 "RDL": "╵ ", "RL": "│ ", "UD": "──", "UR": "┐ ",
 			 "UL": "┌─", "RD": "┘ ", "DL": "└─", "U": "┬─",
 			 "R": "┤ ", "D": "┴─", "L": "├─", "": "┼─"}
 	return "\n".join("".join(trans[c] for c in row) for row in cleanup(out))
 
 
 if __name__ == '__main__':
-	print(l_system_string("A", "(A->+Bf-AFA-FB+), (B->-AF+BFB+FA-)", 3, "R"))
+	print(l_system_string("F", "(F->F[-F][+F])", 5, "U"))
```

### Comparing `frascii-2.3/frascii/fractals/mandelbrot.py` & `frascii-2.4/frascii/fractals/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/peano_curve.py` & `frascii-2.4/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii/fractals/sierpinski_carpet.py` & `frascii-2.4/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-2.3/frascii.egg-info/SOURCES.txt` & `frascii-2.4/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

