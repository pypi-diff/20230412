# Comparing `tmp/nvosscript-1.1.9.tar.gz` & `tmp/nvosscript-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.1.9.tar", last modified: Tue Apr 11 10:17:23 2023, max compression
+gzip compressed data, was "nvosscript-1.2.0.tar", last modified: Wed Apr 12 01:43:35 2023, max compression
```

## Comparing `nvosscript-1.1.9.tar` & `nvosscript-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,25 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.128851 nvosscript-1.1.9/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.1.9/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 10:17:23.128378 nvosscript-1.1.9/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.1.9/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.113011 nvosscript-1.1.9/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.1.9/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    12890 2023-04-11 09:49:24.000000 nvosscript-1.1.9/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.1.9/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     7331 2023-04-11 07:50:33.000000 nvosscript-1.1.9/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4376 2023-04-11 07:50:33.000000 nvosscript-1.1.9/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      812 2023-04-11 07:50:33.000000 nvosscript-1.1.9/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.116253 nvosscript-1.1.9/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 10:17:23.000000 nvosscript-1.1.9/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      682 2023-04-11 10:17:23.000000 nvosscript-1.1.9/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-04-11 10:17:23.000000 nvosscript-1.1.9/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-04-11 10:17:23.000000 nvosscript-1.1.9/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-04-11 10:17:23.000000 nvosscript-1.1.9/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       20 2023-04-11 10:17:23.000000 nvosscript-1.1.9/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-04-11 10:17:23.128909 nvosscript-1.1.9/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-04-11 10:17:19.000000 nvosscript-1.1.9/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.117155 nvosscript-1.1.9/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.1.9/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     3480 2023-04-11 10:17:19.000000 nvosscript-1.1.9/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.107586 nvosscript-1.1.9/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.127063 nvosscript-1.1.9/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-04-11 07:07:42.000000 nvosscript-1.1.9/venv/bin/activate_this.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-04-11 07:08:34.000000 nvosscript-1.1.9/venv/bin/jp.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      632 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2html.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      754 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2html4.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2html5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      831 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2latex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      654 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2man.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      820 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2odt.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1758 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      639 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      675 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2s5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      911 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2xetex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      640 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rst2xml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      708 2023-04-11 07:08:20.000000 nvosscript-1.1.9/venv/bin/rstpep2html.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 10:17:23.127782 nvosscript-1.1.9/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1283 2023-04-11 07:50:33.000000 nvosscript-1.1.9/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.589281 nvosscript-1.2.0/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.0/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 01:43:35.589147 nvosscript-1.2.0/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.0/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.587538 nvosscript-1.2.0/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.0/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    12912 2023-04-12 01:26:56.000000 nvosscript-1.2.0/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.2.0/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     7481 2023-04-11 11:20:46.000000 nvosscript-1.2.0/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4493 2023-04-12 01:35:00.000000 nvosscript-1.2.0/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      893 2023-04-12 01:33:59.000000 nvosscript-1.2.0/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.588431 nvosscript-1.2.0/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-12 01:43:35.589323 nvosscript-1.2.0/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-12 01:40:18.000000 nvosscript-1.2.0/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.588652 nvosscript-1.2.0/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.0/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3529 2023-04-12 01:40:27.000000 nvosscript-1.2.0/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.588869 nvosscript-1.2.0/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.2.0/win/win_auto_script.py
```

### Comparing `nvosscript-1.1.9/LICENSE` & `nvosscript-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.9/nvos/file.py` & `nvosscript-1.2.0/nvos/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 def sync_project_data(workspace_path):
     logger.info(f"start execute sync_project_data {workspace_path}")
     project_space_path = os.path.join(workspace_path, ".ndtc", "project_space")
     origin_project_space_list = []
     if os.path.exists(project_space_path):
         with open(project_space_path, 'r') as f:
             for line in f:
-                origin_project_space_list.append(json.loads(line.rstrip()))
+                origin_project_space_list.append(json.loads(line.strip()))
     project_space_list = []
     find_project_space(workspace_path, project_space_list)
     project_space_list = filter_project_space(workspace_path, project_space_list)
     sync_project_offset(workspace_path, project_space_list)
     if len(project_space_list) != len(origin_project_space_list):
         logger.info(
             f"projectSpace changed projectSpaceList: {project_space_list}          originProjectSpaceList:{origin_project_space_list}")
@@ -205,20 +205,20 @@
     return project_space_list
 
 
 def get_current_git_branch(workspace_path):
     git_path = os.path.join(workspace_path, ".git")
     if not os.path.exists(git_path):
         return ""
-    result = subprocess.run(['git', 'branch'], capture_output=True, text=True)
-    git_branch_val = result.stdout
+    completed_process = subprocess.run(['git', 'branch'], stdout=subprocess.PIPE)
+    git_branch_val = completed_process.stdout.decode().splitlines()
     if len(git_branch_val) == 0:
         return ""
     git_branch_data = ""
-    for line in git_branch_val.splitlines():
+    for line in git_branch_val:
         if "*" in line:
             git_branch_data = line.split("*")[1].strip()
     return git_branch_data
 
 
 # 获取项目的空间
 def find_project_space(workspace_path, result_list):
```

### Comparing `nvosscript-1.1.9/nvos/login.py` & `nvosscript-1.2.0/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.9/nvos/remote.py` & `nvosscript-1.2.0/nvos/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,24 @@
     "prod": "https://ndtc.nioint.com/#/nvosTool/spaceList",
     "stg": "https://ndtc-stg.nioint.com/#/nvosTool/spaceList",
     "dev": " https://soa-tools-dev.nioint.com/#/nvosTool/spaceList"
 }
 global_var = 0
 
 
-def upload_client_script():
+def upload_client_script(file_path):
     get_current_env()
     s3_secret = get_s3_secret()
     bucket_name = s3_secret["bucket"]
     aws_ak = s3_secret["ak"]
     aws_sk = s3_secret["sk"]
     aws_region = s3_secret["regionId"]
     s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
                         aws_secret_access_key=aws_sk)
     bucket = s3.Bucket(bucket_name)
-    file_path = "/Users/andre.zhao/PycharmProjects/nvos-script/dist/nvosscript.zip"
     file_name = "/nvos-script/nvosscript.zip"
     bucket.upload_file(file_path, file_name)
 
 def upload_file(file_path_list, project_space_list):
     s3_secret = get_s3_secret()
     bucket_name = s3_secret["bucket"]
     aws_ak = s3_secret["ak"]
@@ -182,19 +181,25 @@
     return {}
 
 
 def switch_env(env):
     val = daemon_network_mapping.get(env)
     if len(val) == 0:
         return
-    with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'w') as f:
-        f.writelines(val)
     tip = daemon_network_front_mapping.get(env)
+    result = {"cloud":val,"tip":tip,"env":env}
+    with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'w') as f:
+        f.writelines(json.dumps(result))
     print(f"this script current env:{env} and cloud linked:{tip}")
 
 
 def get_current_env():
     global daemon_network
+    result = {}
     if os.path.exists(os.path.expanduser(os.path.join('~', 'nvos_env'))):
         with open(os.path.expanduser(os.path.join('~', 'nvos_env')), 'r')as f:
-            daemon_network = f.readline()
-    logger.info(f"get_current_env this env:{daemon_network}")
+            result = json.loads(f.readline().strip())
+    daemon_network = result["cloud"]
+    tip = result["tip"]
+    env = result["env"]
+    logger.info(f"current env:{env} this cloud linked:{tip} daemon_network:{daemon_network}")
+    return result
```

### Comparing `nvosscript-1.1.9/nvos/run.py` & `nvosscript-1.2.0/nvos/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 
 def command_init():
     status = login.check_login_status()
     if not status:
         print("Please login first. you could use login command to login this script")
         return
     workspace_path, success = utils.check_workspace_exist(os.getcwd())
-    init_path = os.path.join(workspace_path, ".ndtc", "init")
 
-    flag = utils.check_subdirectory_workspace_exist(os.getcwd())
+    sub_workspace_path, flag = utils.check_subdirectory_workspace_exist(os.getcwd())
     if flag:
-        print("The subdirectory has already bean initialized, don't repeat execute init command")
+        print(f"The subdirectory has already bean initialized, don't repeat execute init command, this subdirectory:{sub_workspace_path}")
         try:
             shutil.rmtree(os.path.join(os.getcwd(), ".ndtc"))
         except OSError as e:
             print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
         return
 
     print("please wait one minute.........")
@@ -109,21 +108,26 @@
     status = login.check_login_status()
     if not status:
         print("Please login first. you could use login command to login this script")
         return workspace_path, False
     return workspace_path, True
 
 
-def command_env(env):
+def command_env(env=None):
+    if env is None:
+        result = remote.get_current_env()
+        print(f"current env:{result['env']} this cloud linked:{result['tip']}")
+        return
+
     remote.switch_env(env)
     workspace_env = []
     with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'r') as f:
         for line in f:
             workspace_env.append(line.strip())
     for item in workspace_env:
         try:
             os.remove(os.path.join(item, ".ndtc", 'offset'))
             os.remove(os.path.join(item, ".ndtc", 'project_space'))
             os.remove(os.path.join(item, ".ndtc", 'config'))
-        except OSError as e:
-            print(f"Error: {os.path.join(item, '.ndtc', 'offset')} : {e.strerror}")
+        except OSError:
+            logger.exception("command_env")
```

### Comparing `nvosscript-1.1.9/nvos/utils.py` & `nvosscript-1.2.0/nvos/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             return current_path, True
     return check_workspace_exist(os.path.dirname(current_path))
 
 
 def check_subdirectory_workspace_exist(current_path, index=0):
     for file_name in os.listdir(current_path):
         if ".ndtc" == file_name and index >= 1:
-            return True
+            return os.path.join(current_path,file_name) ,True
     for file_name in os.listdir(current_path):
         if os.path.isdir(os.path.join(current_path, file_name)):
             index = index + 1
             result = check_subdirectory_workspace_exist(os.path.join(current_path, file_name), index)
             if result:
-                return result
-    return False
+                return os.path.join(current_path, file_name), result
+    return "", False
```

### Comparing `nvosscript-1.1.9/setup.py` & `nvosscript-1.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.1.9',
+    version='1.2.0',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.1.9/start/main.py` & `nvosscript-1.2.0/start/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.1.9")
+        print("1.2.0")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
@@ -63,10 +63,10 @@
         print(
             "\n\t if you still have many things you don't understand,you can take a look as https://nio.feishu.cn/wiki/wikcn9L7Di4ILQKaNmDDTrmpLqg ")
 
 
 if __name__ == '__main__':
     multiprocessing.freeze_support()
     main()
-    # remote.upload_client_script()
+    # remote.upload_client_script("/Users/andre.zhao/Documents/test/nvosscript.zip")
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `nvosscript-1.1.9/win/win_auto_script.py` & `nvosscript-1.2.0/win/win_auto_script.py`

 * *Files identical despite different names*

