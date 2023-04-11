# Comparing `tmp/yeagerai-agent-0.0.37.tar.gz` & `tmp/yeagerai-agent-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeagerai-agent-0.0.37.tar", last modified: Mon Apr 10 15:39:48 2023, max compression
+gzip compressed data, was "yeagerai-agent-0.0.38.tar", last modified: Tue Apr 11 22:58:28 2023, max compression
```

## Comparing `yeagerai-agent-0.0.37.tar` & `yeagerai-agent-0.0.38.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-09 11:08:36.000000 yeagerai-agent-0.0.37/LICENSE
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2731 2023-04-10 01:09:09.000000 yeagerai-agent-0.0.37/README.md
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/setup.cfg
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-10 15:39:25.000000 yeagerai-agent-0.0.37/setup.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 13:23:58.000000 yeagerai-agent-0.0.37/yeagerai/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/agent/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-10 14:29:05.000000 yeagerai-agent-0.0.37/yeagerai/agent/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1161 2023-04-09 18:33:12.000000 yeagerai-agent-0.0.37/yeagerai/agent/master_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/agent/output_parser.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/agent/prompt_template.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4221 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.37/yeagerai/agent/yeagerai_agent.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/interfaces/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-06 00:28:34.000000 yeagerai-agent-0.0.37/yeagerai/interfaces/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/interfaces/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.37/yeagerai/interfaces/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/interfaces/callbacks/local_file_system_n_git.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3553 2023-04-10 15:38:11.000000 yeagerai-agent-0.0.37/yeagerai/interfaces/cli.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/memory/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-10 14:29:33.000000 yeagerai-agent-0.0.37/yeagerai/memory/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/memory/callbacks/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-10 14:29:46.000000 yeagerai-agent-0.0.37/yeagerai/memory/callbacks/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/memory/callbacks/session_memory_handler.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/memory/yeagerai_context.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/toolkit/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      541 2023-04-10 14:28:39.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/__init__.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_mocked_tests/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:37:27.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_mocked_tests/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4106 2023-04-10 14:30:31.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2628 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_source/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-09 16:52:27.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_source/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1725 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4952 2023-04-10 14:31:34.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_source/create_tool_source.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai/toolkit/design_solution_sketch/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 14:37:07.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/design_solution_sketch/__init__.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2842 2023-04-10 14:32:50.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3263 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-09 13:24:39.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/yeagerai_tool.py
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      589 2023-04-09 21:17:55.000000 yeagerai-agent-0.0.37/yeagerai/toolkit/yeagerai_toolkit.py
-drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-10 15:39:48.144104 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-10 15:39:48.000000 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/PKG-INFO
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1426 2023-04-10 15:39:48.000000 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-10 15:39:48.000000 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-10 15:39:48.000000 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/entry_points.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-10 15:39:48.000000 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/requires.txt
--rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-10 15:39:48.000000 yeagerai-agent-0.0.37/yeagerai_agent.egg-info/top_level.txt
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.391225 yeagerai-agent-0.0.38/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1067 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/LICENSE
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-11 22:58:28.391225 yeagerai-agent-0.0.38/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2937 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/README.md
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       38 2023-04-11 22:58:28.391225 yeagerai-agent-0.0.38/setup.cfg
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1199 2023-04-11 22:57:42.000000 yeagerai-agent-0.0.38/setup.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/agent/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       56 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/agent/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1203 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/agent/master_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1057 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/agent/output_parser.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1608 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/agent/prompt_template.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2917 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/agent/yeagerai_agent.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/interfaces/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/interfaces/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/interfaces/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      103 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/interfaces/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4873 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/interfaces/callbacks/local_file_system_n_git.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5719 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/interfaces/cli.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/memory/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       61 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/memory/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/memory/callbacks/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       80 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/memory/callbacks/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2689 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/memory/callbacks/session_memory_handler.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1677 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/memory/yeagerai_context.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/toolkit/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      670 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/__init__.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_mocked_tests/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_mocked_tests/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4123 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5114 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_source/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_source/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2574 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     4913 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_source/create_tool_source.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/toolkit/design_solution_sketch/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/design_solution_sketch/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     2855 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3508 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai/toolkit/load_n_fix_new_tool/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/load_n_fix_new_tool/__init__.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     5663 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     3221 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool_master_prompt.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       98 2023-04-11 09:44:18.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/yeagerai_tool.py
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      617 2023-04-11 22:55:42.000000 yeagerai-agent-0.0.38/yeagerai/toolkit/yeagerai_toolkit.py
+drwxrwxr-x   0 jmlago    (1000) jmlago    (1000)        0 2023-04-11 22:58:28.387225 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)      853 2023-04-11 22:58:28.000000 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)     1609 2023-04-11 22:58:28.000000 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        1 2023-04-11 22:58:28.000000 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       64 2023-04-11 22:58:28.000000 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)       47 2023-04-11 22:58:28.000000 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/requires.txt
+-rw-rw-r--   0 jmlago    (1000) jmlago    (1000)        9 2023-04-11 22:58:28.000000 yeagerai-agent-0.0.38/yeagerai_agent.egg-info/top_level.txt
```

### Comparing `yeagerai-agent-0.0.37/LICENSE` & `yeagerai-agent-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.37/PKG-INFO` & `yeagerai-agent-0.0.38/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.37
+Version: 0.0.38
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.37/README.md` & `yeagerai-agent-0.0.38/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [ WARNING: super-beta ]
 
 [![](https://dcbadge.vercel.app/api/server/VpfmXEMN66?compact=true&style=flat)](https://discord.gg/VpfmXEMN66) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/yeagerai.svg?style=social&label=Follow%20%40YeagerAI)](https://twitter.com/yeagerai) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
 Yeager.ai Agent is the first Langchain Agent creator designed to help you build, prototype, and deploy AI-powered agents with ease. With an emphasis on flexibility, interactivity, and seamless integration, Yeager.ai Agent is the perfect tool for developers, researchers, and AI enthusiasts alike.
 
 ## Quick install
-`pip install yeagerai`
+`pip install yeagerai-agent`
 
 ## Key Features
 - 🚀 **Create and Test Agents and Tools On-The-Fly:** With this feature, you can quickly prototype and experiment with agents and tools without the need for a lengthy setup process. Great for fast-paced development and testing!
 
 - 👩‍💻 **Interactive CLI:** Enjoy a user-friendly, interactive command line interface that makes it easy to navigate, manage, and execute commands with real-time feedback. It's like having a conversation with your code!
 
 - 💾 **Session Persistent Memory:** No more lost data between sessions! Our session persistent memory ensures that your work is preserved across multiple sessions, making it easy to pick up right where you left off.
@@ -18,26 +18,29 @@
 - 🌐 **Fully Integrated with the Langchain Ecosystem:** Seamlessly interact with other tools and resources in the Langchain ecosystem, allowing for efficient collaboration, sharing, and integration of your projects.
 
 
 ## Getting Started
 To call the yeagerai Agent from the terminal, just type:
 
 ```
-yeagerai
+yeagerai-agent
 ```
 
 And start building your agents on-the-fly!
 
-### ⚠️ Warning! GPT-4 API Access Required
+### ⚠️ Warnings! 
 
+#### GPT-4 API Access Required
 If you don't have access to GPT-4 API, don't worry! You can still take advantage of Yeager.ai Agent's features through our Discord bot. 🤖
 
 [Join our Discord server](https://discord.gg/VpfmXEMN66) to get started and interact with the Yeager.ai Agent using the GPT-4-powered bot. Our friendly community is also there to assist you, answer questions, and share their experiences.
 
+#### Not tested for windows
+But if you want to contribute PRs al welcome! Just contact @jmlago#0277 on [our Discord server](https://discord.gg/VpfmXEMN66)
 ## Documentation
-For detailed information on use cases, tools, agents, toolkits, and agent executors, please visit the [Yeager.ai Agent docs]().
+For detailed information on use cases, tools, agents, toolkits, and agent executors, please visit the [Yeager.ai Agent docs](https://yeagerai.gitbook.io/docs).
 
 ## Contributing
 We encourage contributions to help expand and improve the Yeager.ai Agent! Please read our [CONTRIBUTING]() for guidelines on how to submit your contributions.
 
 ## License
 Yeager.ai Agent is released under the MIT License. Please see the [LICENSE file](https://github.com/yeagerai/yeagerai-agent/blob/main/LICENSE) for more information.
```

### Comparing `yeagerai-agent-0.0.37/setup.py` & `yeagerai-agent-0.0.38/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="yeagerai-agent",
-    version="0.0.37",
+    version="0.0.38",
     description="The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.",
     author="YeagerAI LLC",
     author_email="jm@yeager.ai",
     packages=find_packages(),
     install_requires=[
         "langchain",
         "openai",
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/agent/master_template.py` & `yeagerai-agent-0.0.38/yeagerai/agent/master_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MASTER_TEMPLATE = """
 
-You are an AI agent named @yeager.ai developed by the company YeagerAI, and you are in a conversation with a human. 
+You are an AI agent named @yeager.ai developed by the company YeagerAI, and you are in a conversation with a human. There is nothing beyond your capabilities.
 Your duty is to help humans in the creation of LangChain agents and tools. To do that you use a test driven development approach.
 So usually it starts by designing a solution sketch, then the tests, and finally the code.
 
 Here are the previous messages of the conversation that you are having:
 
 {chat_history}
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/agent/output_parser.py` & `yeagerai-agent-0.0.38/yeagerai/agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.37/yeagerai/agent/prompt_template.py` & `yeagerai-agent-0.0.38/yeagerai/agent/prompt_template.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.37/yeagerai/interfaces/callbacks/local_file_system_n_git.py` & `yeagerai-agent-0.0.38/yeagerai/interfaces/callbacks/local_file_system_n_git.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.37/yeagerai/memory/callbacks/session_memory_handler.py` & `yeagerai-agent-0.0.38/yeagerai/memory/callbacks/session_memory_handler.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.37/yeagerai/memory/yeagerai_context.py` & `yeagerai-agent-0.0.38/yeagerai/memory/yeagerai_context.py`

 * *Files identical despite different names*

### Comparing `yeagerai-agent-0.0.37/yeagerai/toolkit/__init__.py` & `yeagerai-agent-0.0.38/yeagerai/toolkit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,7 +9,12 @@
     DesignSolutionSketchAPIWrapper,
     DesignSolutionSketchRun,
 )
 from yeagerai.toolkit.create_tool_mocked_tests.create_tool_mocked_tests import (
     CreateToolMockedTestsAPIWrapper,
     CreateToolMockedTestsRun,
 )
+
+from yeagerai.toolkit.load_n_fix_new_tool.load_n_fix_new_tool import (
+    LoadNFixNewToolAPIWrapper,
+    LoadNFixNewToolRun,
+)
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py` & `yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         chain = LLMChain(llm=chat, prompt=chat_prompt)
         out = chain.run(solution_sketch)
 
         # Extract the name of the class from the code block
         quick_llm = OpenAI(temperature=0)
         class_name = quick_llm(
             f"Which is the name of the class that is being tested here? Return only the class_name value like a python string, without any other explanation \n {out}"
-        )
+        ).replace("\n", "")
 
         # Parse the Python block inside the output, handling different code block formats
         code_block_pattern = re.compile(r"(```.*?```)", re.DOTALL)
         code_block = re.search(code_block_pattern, out)
         if code_block:
             code = code_block.group(1).strip()
 
@@ -79,19 +79,19 @@
         return "Error: No code block found or class name could not be extracted."
 
 
 class CreateToolMockedTestsRun(YeagerAITool):
     """Tool that adds the capability of creating the source code of other Tools on-the-fly and writing it into cwd."""
 
     name = "Create Tool Tests Source"
-    description = """Useful for when you need to create the unit tests for a LangChain Tool. 
-        Input should be a string that represents the solution sketch of the functionality wanted in the Tool,
+    description = """Useful for when you need to create the unit tests for a YeagerAI Tool. 
+        Input should be a string that represents the solution sketch of the functionality wanted in the YeagerAI Tool,
         It should be defined earlier in the conversation.
         """
-    final_answer_format = "Final answer: just return the output code block that contains the code of the Tool's unit tests and a success message"
+    final_answer_format = "Final answer: just return a success message saying that the file has been written successfully and the path."
     api_wrapper: CreateToolMockedTestsAPIWrapper
 
     def _run(self, solution_sketch: str) -> str:
         """Use the tool."""
         return self.api_wrapper.run(solution_sketch=solution_sketch)
 
     async def _arun(self, query: str) -> str:
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/toolkit/create_tool_source/create_tool_source.py` & `yeagerai-agent-0.0.38/yeagerai/toolkit/create_tool_source/create_tool_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,38 +72,38 @@
                 code = code[:-3]
 
             # Extract the name of the class from the code block
             class_name_pattern = re.compile(r"class (\w+)\(BaseModel\):")
             class_name_match = re.search(class_name_pattern, code)
             if class_name_match:
                 class_name = class_name_match.group(1)
+                class_name = class_name.replace("APIWrapper", "")
 
-                # Write the {class_name}.py file inside the user-defined session_path
                 output_file = f"{class_name}.py"
                 with open(os.path.join(self.session_path, output_file), "w") as f:
                     f.write(code)
                     f.close()
 
                 return f"The file {class_name}.py has been written in the {self.session_path} successfully!\nHere is the source code of the {class_name} LangChain tool based on given requirements:\n{code}"
 
         return "Error: No code block found or class name could not be extracted."
 
 
 class CreateToolSourceRun(YeagerAITool):
     """Tool that adds the capability of creating the source code of other Tools on-the-fly and writing it into cwd."""
 
     name = "Create Tool Source"
-    description = """Useful for when you need to create the source code of a LangChain Tool. 
+    description = """Useful for when you need to create the source code of a YeagerAITool. 
         Input MUST BE a string made of two substrings separated by a this token '######SPLIT_TOKEN########'.
         That is substring1+'######SPLIT_TOKEN########'+substring2: 
         - where substring1 represents the first string represents the solution sketch of the functionality wanted in the Tool.
         - and substring 2 is code block that contains the tool_tests. That is the unit tests already created for testing the tool. 
         Both of them should be defined earlier in the conversation.
         """
-    final_answer_format = "Final answer: just return the output code block that contains the code of the Tool and a success message"
+    final_answer_format = "Final answer: just return a success message saying the path where the class was written"
     api_wrapper: CreateToolSourceAPIWrapper
 
     def _run(self, solution_sketch_n_tool_tests: str) -> str:
         """Use the tool."""
         return self.api_wrapper.run(
             solution_sketch_n_tool_tests=solution_sketch_n_tool_tests
         )
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py` & `yeagerai-agent-0.0.38/yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,27 +42,27 @@
         human_message_prompt = HumanMessagePromptTemplate(prompt=y_tool_master_prompt)
         chat_prompt = ChatPromptTemplate.from_messages([human_message_prompt])
 
         # Create an LLMChain instance and run the command
         chain = LLMChain(llm=chat, prompt=chat_prompt)
         out = chain.run(tool_description_prompt)
 
-        return f"Here is the solution sketch of the LangChain tool that you described based on your requirements:\n{out}"
+        return f"Here is the solution sketch of the YeagerAI tool that you described based on your requirements:\n{out}"
 
 
 class DesignSolutionSketchRun(YeagerAITool):
     """Tool that adds the capability of creating the source code of other Tools on-the-fly and writing it into cwd."""
 
     name = "Design Tool Solution Sketch"
-    description = """Useful for when you need to create the solution sketch of a LangChain Tool. 
+    description = """Useful for when you need to create the solution sketch of a YeagerAITool. 
         Input should be one string, that contains a brief description of the functionality wanted in the Tool.
         The goal of this tool is augment this brief description converting it into a solution sketch.
         """
     final_answer_format = (
-        "Final answer: just return the solution sketch that you have designed."
+        "Final answer: just return a message just saying that the solution sketch was created."
     )
     api_wrapper: DesignSolutionSketchAPIWrapper
 
     def _run(self, tool_description_prompt: str) -> str:
         """Use the tool."""
         return self.api_wrapper.run(tool_description_prompt=tool_description_prompt)
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py` & `yeagerai-agent-0.0.38/yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,74 @@
-DESIGN_SOLUTION_SKETCH_MASTER_PROMPT = """You are a world class expert in designing Tools based on simple descriptions. You don't type python code, but give all the required specifications 
-so others can later implement the Tools.
+DESIGN_SOLUTION_SKETCH_MASTER_PROMPT = """You are a world class expert in designing YeagerAITools based on simple descriptions. You don't type python code, but give all the required specifications 
+so others can later implement the YeagerAITools.
 
-Here is how a template of a Tool looks like:
+Here is how a template of a YeagerAITool looks like:
 
 ```python
 # Import necessary libraries and modules
 import ...
 from pydantic import BaseModel
+from yeagerai.toolkit.yeagerai_tool import YeagerAITool
 # Define the base class (if not already defined in a separate file)
 
 # Define the tool class
 class MyToolAPIWrapper(BaseModel):
     def __init__(self, ...):
         # Initialize attributes
         ...
 
-    def run(self, ...):
+    def run(self, query: str) -> str:
         # Main method for running the tool
         # Validate input
         # Call APIs or perform main functionality
         # Handle errors and edge cases
         # Return the output
         ...
 
-    async def _arun(self, ...):
-        # Asynchronous main method (if applicable)
-        ...
-
     def _helper_function(self, ...):
         # Utility methods or helper functions (if required)
         ...
 
-class MyToolRun(YeagerTool):
+class MyToolRun(YeagerAITool):
     \"\"\"Explain what the tool does\"\"\"
 
+    api_wrapper: MyToolAPIWrapper # IMPORTANT: note that the api_wrapper must be defined with a colon, not an equal sign
     name = "My Tool's Name"
     description = (
         \"\"\"Describe when it is useful to use the tool.
         And an example of its inputs explained\"\"\"
     )
     final_answer_format = "Final answer: describe which is the output message of the tool"
-    api_wrapper: MyToolAPIWrapper
 
     def _run(self, query: str) -> str:
         \"\"\"Use the tool.\"\"\"
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         \"\"\"Use the tool asynchronously.\"\"\"
         raise NotImplementedError("GoogleSearchRun does not support async")
 
 ```
+IMPORTANT: 
+- There must be two classes, the (class_name)Run and the (class_name)APIWrapper. The (class_name)Run class must inherit from YeagerAITool, and the (class_name)APIWrapper class must inherit from BaseModel.
+- You can only return one python block of code that contains the code of the YeagerAITool based on the following solution sketch, and the tests that it must pass:
+- The run method of the (class_name)APIWrapper and the _run method of the (class_name)Run MUST HAVE ONLY ONE ARGUMENT, which is the query and is a string, and ONLY ONE output that is a string.
+- api_wrapper, name, description, and final_answer_format are class attributes.
+- Both classes must not have an __init__ method. And api_wrapper must not be instantiated, just typed. That is because the YeagerAITool class inherits from BaseModel. So basically api_wrapper just needs the type, no instantiation.
 
-And the design that you provide, will be used to create a Tool.
-
-Here is the methodology that you have to follow to create the design of the Tool:
+And the design that you provide, will be used to create a YeagerAITool.
 
-1. Define the tool's specifications:
-- Clearly state the main goal of the tool.
-- Break down the main goal into smaller tasks or steps, considering potential API calls if needed.
-- Describe the required inputs and expected outputs.
-- Identify any external APIs the tool will interact with and list their authentication and authorization requirements.
-- Understand the specific API endpoints and their expected inputs and outputs.
-- Outline any specific instructions or constraints, including handling potential API errors or rate-limiting issues.
-
-2. Create a solution sketch:
+Solution Sketch:
+- Name of the tool
 - Describe the main goal of the tool.
 - Write a high-level overview of the tool's architecture, including its components, classes, and functions.
 - Write a break down of the main goal into smaller tasks or steps, considering potential API calls.
 - Describe the required inputs and expected outputs.
 - Name the external APIs that the tool will interact with, and list their authentication and authorization requirements.
 - Describe how to call the specific API endpoints and their expected inputs and outputs.
-- Outline any specific instructions or constraints, including handling potential API errors or rate-limiting issues.
-- Describe a set of tests that the tool should pass in order to have all the functionalities
-- Write a set of input and output data examples for the above tests
 
-Create a solution sketch of a Tool given this description: 
+While creating the solution sketch, you have to be very precise, with short and understandable descriptions.
+
+Create a Solution Sketch (basically a text, DO NOT RETURN A BLOCK OF CODE) of a YeagerAITool given this description: 
 
 {tool_description_prompt}
 """
```

### Comparing `yeagerai-agent-0.0.37/yeagerai/toolkit/yeagerai_toolkit.py` & `yeagerai-agent-0.0.38/yeagerai/toolkit/yeagerai_toolkit.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 from typing import List
 
 from langchain.agents.agent_toolkits.base import BaseToolkit
 from langchain.tools import BaseTool
 
 
-class YeagerAIToolkit(BaseToolkit):
+class YeagerAIToolkit:
     """Toolkit for interacting with a JSON spec."""
 
-    tools_list: List[BaseTool] = []
+    def __init__(self) -> None:
+        self.tools_list: List[BaseTool] = []
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools_list
 
     def register_tool(self, tool: BaseTool):
         """Register a tool to the toolkit."""
```

### Comparing `yeagerai-agent-0.0.37/yeagerai_agent.egg-info/PKG-INFO` & `yeagerai-agent-0.0.38/yeagerai_agent.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeagerai-agent
-Version: 0.0.37
+Version: 0.0.38
 Summary: The @yeagerai Agent is used to create your custom LangChain Agents on-the-fly.
 Author: YeagerAI LLC
 Author-email: jm@yeager.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yeagerai-agent-0.0.37/yeagerai_agent.egg-info/SOURCES.txt` & `yeagerai-agent-0.0.38/yeagerai_agent.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,13 +23,16 @@
 yeagerai/toolkit/create_tool_mocked_tests/create_tool_mocked_tests_master_prompt.py
 yeagerai/toolkit/create_tool_source/__init__.py
 yeagerai/toolkit/create_tool_source/create_tool_master_prompt.py
 yeagerai/toolkit/create_tool_source/create_tool_source.py
 yeagerai/toolkit/design_solution_sketch/__init__.py
 yeagerai/toolkit/design_solution_sketch/design_solution_sketch.py
 yeagerai/toolkit/design_solution_sketch/design_solution_sketch_master_prompt.py
+yeagerai/toolkit/load_n_fix_new_tool/__init__.py
+yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool.py
+yeagerai/toolkit/load_n_fix_new_tool/load_n_fix_new_tool_master_prompt.py
 yeagerai_agent.egg-info/PKG-INFO
 yeagerai_agent.egg-info/SOURCES.txt
 yeagerai_agent.egg-info/dependency_links.txt
 yeagerai_agent.egg-info/entry_points.txt
 yeagerai_agent.egg-info/requires.txt
 yeagerai_agent.egg-info/top_level.txt
```

