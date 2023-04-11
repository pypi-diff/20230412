# Comparing `tmp/cpggen-0.8.1.tar.gz` & `tmp/cpggen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.8.1.tar", max compression
+gzip compressed data, was "cpggen-0.9.0.tar", max compression
```

## Comparing `cpggen-0.8.1.tar` & `cpggen-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-11 06:29:33.544823 cpggen-0.8.1/LICENSE
--rw-r--r--   0        0        0     6570 2023-04-11 06:29:33.544823 cpggen-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/__init__.py
--rw-r--r--   0        0        0    12884 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/cli.py
--rw-r--r--   0        0        0    22431 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/logger.py
--rw-r--r--   0        0        0    10065 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-11 06:29:33.548823 cpggen-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7898 1970-01-01 00:00:00.000000 cpggen-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 23:10:54.522020 cpggen-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6746 2023-04-11 23:10:54.522020 cpggen-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 23:10:54.526020 cpggen-0.9.0/cpggen/__init__.py
+-rw-r--r--   0        0        0    12884 2023-04-11 23:10:54.526020 cpggen-0.9.0/cpggen/cli.py
+-rw-r--r--   0        0        0    23764 2023-04-11 23:10:54.526020 cpggen-0.9.0/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-11 23:10:54.526020 cpggen-0.9.0/cpggen/logger.py
+-rw-r--r--   0        0        0    10234 2023-04-11 23:10:54.526020 cpggen-0.9.0/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-11 23:10:54.526020 cpggen-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8074 1970-01-01 00:00:00.000000 cpggen-0.9.0/PKG-INFO
```

### Comparing `cpggen-0.8.1/LICENSE` & `cpggen-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.8.1/README.md` & `cpggen-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 ██║     ██╔═══╝ ██║   ██║
 ╚██████╗██║     ╚██████╔╝
  ╚═════╝╚═╝      ╚═════╝
 ```
 
 CPG Generator is a python cli tool to generate [Code Property Graph](https://cpg.joern.io) for multiple languages. The generated CPG can be directly imported to [Joern](https://joern.io) or uploaded to [Qwiet.AI](https://docs.shiftleft.io/home) for analysis.
 
+## Pre-requisites
+
+- JDK 11 or above
+- Python 3.10
+- Docker or podman (Windows, Linux or Mac) or
+- Joern [natively installed](https://docs.joern.io/installation) (Linux only)
+
 ## Installation
 
 cpggen is available as a [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
 
 ```
 pip install cpggen
 ```
@@ -38,23 +45,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - cpggen with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
```

### Comparing `cpggen-0.8.1/cpggen/cli.py` & `cpggen-0.9.0/cpggen/cli.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.8.1/cpggen/executor.py` & `cpggen-0.9.0/cpggen/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,50 +55,50 @@
     "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "python": "%(joern_home)spysrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-tests -l error",
     "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-tests -l error",
     "go": "%(joern_home)sgo2cpg generate -o %(cpg_out)s ./...",
-    "jar": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
-    "jar-with-blocklist": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
-    "scala": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
-    "jsp": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
-    "jsp-with-blocklist": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "cdxgen -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
     "export": "joern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
-    "qwiet": "sl analyze --tag app.group=%(group)s --app %(app)s-%(language)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
+    "qwiet": "sl analyze --tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "java": {
         "maven": [
-            get("MVN_CMD", "mvn"),
+            get("MVN_CMD", "%(maven_cmd)s"),
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
         "gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "build"],
         "sbt": ["sbt", "compile"],
     },
     "jar": {
         "maven": [
-            get("MVN_CMD", "mvn"),
+            get("MVN_CMD", "%(maven_cmd)s"),
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
         "gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "jar"],
         "sbt": ["sbt", "stage"],
     },
     "android": {"gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "compileDebugSources"]},
     "kotlin": {
         "maven": [
-            get("MVN_CMD", "mvn"),
+            get("MVN_CMD", "%(maven_cmd)s"),
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
         "gradle": [get("GRADLE_CMD", "gradle"), "build"],
     },
     "scala": ["sbt", "stage"],
@@ -156,22 +156,32 @@
         else:
             build_args = build_sets
         for afile in v:
             base_dir = os.path.dirname(afile)
             build_args_str = " ".join(build_args)
             if "%(" in build_args_str:
                 gradle_cmd = "gradle"
+                maven_cmd = "mvn"
                 if os.path.exists(os.path.join(base_dir, "gradlew")):
                     gradle_cmd = "gradlew"
                     try:
                         os.chmod(os.path.join(base_dir, "gradlew"), 0o755)
                     except Exception:
                         # Ignore errors
                         pass
-                build_args_str = build_args_str % dict(gradle_cmd=gradle_cmd)
+                if os.path.exists(os.path.join(base_dir, "mvnw")):
+                    maven_cmd = "mvnw"
+                    try:
+                        os.chmod(os.path.join(base_dir, "mvnw"), 0o755)
+                    except Exception:
+                        # Ignore errors
+                        pass
+                build_args_str = build_args_str % dict(
+                    gradle_cmd=gradle_cmd, maven_cmd=maven_cmd
+                )
             try:
                 LOG.debug(
                     f"Executing {build_args_str} in {base_dir}. To speed up this step, cache your project's dependencies using the CI build cache."
                 )
                 cp = subprocess.run(
                     build_args_str.split(" "),
                     stdout=subprocess.PIPE,
@@ -255,29 +265,31 @@
                 "[green]" + tool_verb,
                 total=100,
                 start=False,
             )
             cmd_with_args = cpg_tools_map.get(tool_lang)
             if not cmd_with_args:
                 return
+            # Perform build first
+            if auto_build:
+                LOG.info(f"Auto build {src} for {tool_lang}")
+                do_build(tool_lang, src, cwd, env)
             uber_jar = ""
             csharp_artifacts = ""
             # For languages like scala, jsp or jar we need to create a uber jar containing all jar, war files from the source directory
             if "uber_jar" in cmd_with_args:
                 stdout = subprocess.PIPE
                 java_artifacts = find_java_artifacts(src)
                 if len(java_artifacts):
                     uber_jar = java_artifacts[0]
             if "csharp_artifacts" in cmd_with_args:
                 stdout = subprocess.PIPE
                 csharp_artifacts = find_csharp_artifacts(src)
                 if len(csharp_artifacts):
                     csharp_artifacts = csharp_artifacts[0]
-            if auto_build:
-                do_build(tool_lang, src, cwd, env)
             modules = [src]
             # For go, the modules are based on the presence of go.mod files
             if tool_lang == "go":
                 go_mods = find_go_mods(src)
                 if go_mods:
                     modules = [os.path.dirname(gmod) for gmod in go_mods]
             for amodule in modules:
@@ -326,16 +338,19 @@
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
                     **extra_args,
                 )
+                sbom_lang = tool_lang
+                if tool_lang in ("jar", "scala"):
+                    sbom_lang = "java"
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
-                    src=amodule, tool_lang=tool_lang, sbom_out=sbom_out, **extra_args
+                    src=src, tool_lang=sbom_lang, sbom_out=sbom_out, **extra_args
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
                 if not check_command(lang_cmd):
                     if not use_container:
                         LOG.warn(
@@ -386,15 +401,15 @@
                                 LOG.warn(
                                     f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually using the command {' '.join(cmd_list_with_args)}"
                                 )
                     except Exception:
                         LOG.warn(f"Unable to export {src} to {cpg_out_dir}")
                     progress.update(task, completed=100, total=100)
                     continue
-                LOG.debug(
+                LOG.info(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
                         tool_lang,
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
                     )
                 )
                 cwd = amodule
@@ -404,26 +419,35 @@
                 try:
                     progress.update(
                         task,
                         description="Generating SBoM using cdxgen",
                         completed=10,
                         total=100,
                     )
-                    subprocess.run(
+                    # Enable debug for sbom tool
+                    if LOG.isEnabledFor(DEBUG):
+                        env["SCAN_DEBUG_MODE"] = "debug"
+                    LOG.debug(f"Executing {' '.join(sbom_cmd_list_with_args)}")
+                    cp = subprocess.run(
                         sbom_cmd_list_with_args,
                         stdout=stdout,
                         stderr=stderr,
                         cwd=cwd,
                         env=env,
                         check=False,
                         shell=False,
                         encoding="utf-8",
                     )
+                    if cp and LOG.isEnabledFor(DEBUG):
+                        if cp.stdout:
+                            LOG.debug(cp.stdout)
+                        if cp.stderr:
+                            LOG.debug(cp.stderr)
                 except Exception:
-                    # Ignore sbom generation errors
+                    # Ignore SBoM errors
                     pass
                 progress.update(
                     task, description="Generating CPG", completed=20, total=100
                 )
                 cp = subprocess.run(
                     cmd_list_with_args,
                     stdout=stdout,
```

### Comparing `cpggen-0.8.1/cpggen/logger.py` & `cpggen-0.9.0/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.8.1/cpggen/utils.py` & `cpggen-0.9.0/cpggen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,29 +167,31 @@
 
 def find_java_artifacts(search_dir):
     """
     Method to find java artifacts in the given directory
     :param src: Directory to search
     :return: List of war or ear or jar files
     """
-    is_empty = True
+    jlist = []
     with tempfile.NamedTemporaryFile(
         mode="w", suffix=".jar", encoding="utf-8", delete=False
     ) as zfile:
         with zipfile.ZipFile(zfile.name, "w") as zf:
             for dirname, subdirs, files in os.walk(search_dir):
-                is_empty = False
-                for filename in files:
-                    if (
-                        filename.endswith(".jar")
-                        or filename.endswith(".war")
-                        or filename.endswith(".ear")
-                    ):
-                        zf.write(os.path.join(dirname, filename), filename)
-    return [] if is_empty else [zfile.name]
+                filter_ignored_dirs(subdirs)
+                if not is_ignored_dir(search_dir, dirname):
+                    for filename in files:
+                        if (
+                            filename.endswith(".jar")
+                            or filename.endswith(".war")
+                            or filename.endswith(".ear")
+                        ):
+                            jlist.append(os.path.join(dirname, filename))
+                            zf.write(os.path.join(dirname, filename))
+    return jlist if len(jlist) == 1 else [zfile.name]
 
 
 def find_csharp_artifacts(search_dir):
     """
     Method to find .Net solution and csproj files in the given directory
     :param src: Directory to search
     :return: List of war or ear or jar files
```

### Comparing `cpggen-0.8.1/pyproject.toml` & `cpggen-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.8.1"
+version = "0.9.0"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.8.1/PKG-INFO` & `cpggen-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.8.1
+Version: 0.9.0
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -39,14 +39,21 @@
 ██║     ██╔═══╝ ██║   ██║
 ╚██████╗██║     ╚██████╔╝
  ╚═════╝╚═╝      ╚═════╝
 ```
 
 CPG Generator is a python cli tool to generate [Code Property Graph](https://cpg.joern.io) for multiple languages. The generated CPG can be directly imported to [Joern](https://joern.io) or uploaded to [Qwiet.AI](https://docs.shiftleft.io/home) for analysis.
 
+## Pre-requisites
+
+- JDK 11 or above
+- Python 3.10
+- Docker or podman (Windows, Linux or Mac) or
+- Joern [natively installed](https://docs.joern.io/installation) (Linux only)
+
 ## Installation
 
 cpggen is available as a [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
 
 ```
 pip install cpggen
 ```
@@ -70,23 +77,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - cpggen with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
```

