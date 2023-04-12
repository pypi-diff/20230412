# Comparing `tmp/RepRepBuild-0.5.1.tar.gz` & `tmp/RepRepBuild-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.5.1.tar", last modified: Tue Apr 11 13:57:27 2023, max compression
+gzip compressed data, was "RepRepBuild-0.6.0.tar", last modified: Wed Apr 12 08:22:49 2023, max compression
```

## Comparing `RepRepBuild-0.5.1.tar` & `RepRepBuild-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.689089 RepRepBuild-0.5.1/
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.5.1/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-11 13:57:27.688089 RepRepBuild-0.5.1/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.5.1/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1597 2023-04-11 13:56:44.000000 RepRepBuild-0.5.1/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-11 13:57:27.689089 RepRepBuild-0.5.1/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.673089 RepRepBuild-0.5.1/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.674089 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       28 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.688089 RepRepBuild-0.5.1/src/reprepbuild/
--rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.5.1/src/reprepbuild/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9811 2023-04-11 13:17:07.000000 RepRepBuild-0.5.1/src/reprepbuild/__main__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.5.1/src/reprepbuild/articlezip.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3109 2023-03-25 10:49:48.000000 RepRepBuild-0.5.1/src/reprepbuild/bibtex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.5.1/src/reprepbuild/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.5.1/src/reprepbuild/latexdep.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.5.1/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.5.1/src/reprepbuild/pythonscript.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.5.1/src/reprepbuild/repeat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.5.1/src/reprepbuild/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.5.1/src/reprepbuild/zip.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/
+-rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.6.0/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.6.0/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-12 08:21:27.000000 RepRepBuild-0.6.0/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.952363 RepRepBuild-0.6.0/src/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.953363 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/src/reprepbuild/
+-rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.6.0/src/reprepbuild/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     9841 2023-04-12 01:15:07.000000 RepRepBuild-0.6.0/src/reprepbuild/__main__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.6.0/src/reprepbuild/articlezip.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.6.0/src/reprepbuild/bibtex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.6.0/src/reprepbuild/latex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.6.0/src/reprepbuild/latexdep.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.6.0/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.6.0/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.6.0/src/reprepbuild/repeat.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.6.0/src/reprepbuild/utils.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.6.0/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.5.1/COPYING` & `RepRepBuild-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/PKG-INFO` & `RepRepBuild-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.5.1
+Version: 0.6.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.5.1/README.md` & `RepRepBuild-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/pyproject.toml` & `RepRepBuild-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepRepBuild"
-version = "0.5.1"
+version = "0.6.0"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Build tool for Reproducible Reporting"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.6"
@@ -28,14 +28,15 @@
     "Topic :: Text Processing :: Markup :: LaTeX",
 ]
 dependencies = [
     "ninja",
     "pymupdf",
     "tqdm",
     "watchdog",
+    "bibsane",
 ]
 
 [project.urls]
 Issues = "https://github.com/reproducible-reporting/reprepbuild/issues"
 Source = "https://github.com/reproducible-reporting/reprepbuild/"
 Changelog = "https://github.com/reproducible-reporting/reprepbuild/blob/main/CHANGELOG.md"
```

### Comparing `RepRepBuild-0.5.1/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.6.0/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.5.1
+Version: 0.6.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.5.1/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.6.0/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/__init__.py` & `RepRepBuild-0.6.0/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/__main__.py` & `RepRepBuild-0.6.0/src/reprepbuild/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 DEFAULT_RULES = {
     "latexdep": {"command": "rr-latexdep $in", "depfile": "$in.d"},
     "bibtex": {"command": "rr-bibtex $in", "depfile": "$in.d"},
     "latex": {"command": "rr-latex $in"},
     "copy": {"command": "cp $in $out"},
-    "latexdiff": {"command": "latexdiff $in > $out"},
+    "latexdiff": {"command": "latexdiff --append-context2cmd=abstract $in > $out"},
     "reprozip": {"command": "rr-zip $out $in"},
     "reproarticlezip": {"command": "rr-article-zip $out $in"},
     "svgtopdf": {
         "command": "inkscape $in --export-filename=$out --export-type=pdf; rr-normalize-pdf $out"
     },
     "pythonscript": {"command": "rr-python-script $in -- $args > $out", "depfile": "$in.d"},
 }
```

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/articlezip.py` & `RepRepBuild-0.6.0/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/bibtex.py` & `RepRepBuild-0.6.0/src/reprepbuild/bibtex.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,83 +19,96 @@
 # --
 """Run BibTex on a LaTeX aux file."""
 
 
 import argparse
 import os
 import subprocess
+import sys
 
 from .utils import write_dep
 
 
 def main():
     """Main program."""
     args = parse_args()
     return run_bibtex(args.path_aux)
 
 
 def parse_args():
     """Parse command-line arguments."""
-    parser = argparse.ArgumentParser("rr-bibtex")
+    parser = argparse.ArgumentParser("rr-bibtex", description="Run bibtex and bibsane")
     parser.add_argument("path_aux", help="The top-level aux file.")
     return parser.parse_args()
 
 
 def run_bibtex(path_aux):
+    """Process the `.first.aux file`, run bibtex and bibsane."""
     if not path_aux.endswith(".first.aux"):
         print(f"BibTeX input must have a `.first.aux` extension. Got {path_aux}")
         return 2
     workdir, fn_aux = os.path.split(path_aux)
     prefix = fn_aux[:-10]
 
     args = ["bibtex", fn_aux]
-    result = 0
     path_blg = os.path.join(workdir, prefix + ".blg")
-    try:
-        subprocess.run(
-            args,
-            cwd=workdir,
-            check=True,
-            stdin=subprocess.DEVNULL,
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
-    except subprocess.CalledProcessError:
+    cp = subprocess.run(
+        args,
+        cwd=workdir,
+        stdin=subprocess.DEVNULL,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+    )
+    if cp.returncode != 0:
         print(f"    Error running `bibtex {fn_aux}` in `{workdir}`.")
         with open(path_blg) as f:
             for line in f:
                 print(line[:-1])
                 if line.startswith("You've used "):
                     break
-        sys.exit(1)
+        return 1
+
+    args = ["bibsane", fn_aux, "--config=../bibsane.yaml"]
+    cp = subprocess.run(
+        args,
+        cwd=workdir,
+        text=True,
+        stdin=subprocess.DEVNULL,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    )
+    if cp.returncode != 0:
+        print(f"    Error running `bibsane {fn_aux}` in `{workdir}`.")
+        sys.stdout.write(cp.stdout)
+        return 1
 
     # Rename files to those without the `first` interjection.
     for ext in "blg", "bbl":
         os.rename(
             os.path.join(workdir, f"{prefix}.first.{ext}"),
             os.path.join(workdir, f"{prefix}.{ext}"),
         )
 
-    # Parse the blg file to get a list of used bib files
+    # Parse the blg file to get a list of used bib files.
     paths_bib = set()
     with open(path_blg) as f:
         for line in f:
             if line.startswith("Database file #"):
                 paths_bib.add(os.path.join(workdir, line.split()[-1]))
 
-    # Discard the bib files that were generated by LaTeX
+    # Discard the bib files generated by LaTeX.
     path_fls = os.path.join(workdir, prefix + ".fls")
     with open(path_fls) as f:
         for line in f:
             if line.startswith("OUTPUT "):
                 paths_bib.discard(os.path.join(workdir, os.path.normpath(line[7:].strip())))
 
     # Store the input bib files for dependency tracking
     path_bbl = os.path.join(workdir, prefix + ".bbl")
     path_dep = path_aux + ".d"
     write_dep(path_dep, [path_bbl], paths_bib)
 
-    return result
+    return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/latex.py` & `RepRepBuild-0.6.0/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/latexdep.py` & `RepRepBuild-0.6.0/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.6.0/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.6.0/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/repeat.py` & `RepRepBuild-0.6.0/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/utils.py` & `RepRepBuild-0.6.0/src/reprepbuild/utils.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.1/src/reprepbuild/zip.py` & `RepRepBuild-0.6.0/src/reprepbuild/zip.py`

 * *Files identical despite different names*

