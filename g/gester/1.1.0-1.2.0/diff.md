# Comparing `tmp/gester-1.1.0.tar.gz` & `tmp/gester-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\dev\projects\gest\dist\.tmp-_fotl_yn\gester-1.1.0.tar", last modified: Sun Apr  9 09:41:33 2023, max compression
+gzip compressed data, was "E:\dev\projects\gest\dist\.tmp-ok2izjpp\gester-1.2.0.tar", last modified: Wed Apr 12 06:27:12 2023, max compression
```

## Comparing `gester-1.1.0.tar` & `gester-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:41:33.602823 gester-1.1.0/
--rw-rw-rw-   0        0        0     1361 2023-04-08 06:55:38.000000 gester-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2808 2023-04-09 09:41:33.602823 gester-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-04-09 07:55:46.000000 gester-1.1.0/README.md
--rw-rw-rw-   0        0        0     1211 2023-04-09 09:06:50.000000 gester-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 09:41:33.602823 gester-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-09 09:41:33.509223 gester-1.1.0/src/
--rw-rw-rw-   0        0        0       23 2023-04-09 07:22:30.000000 gester-1.1.0/src/__init__.py
--rw-rw-rw-   0        0        0     6407 2023-04-09 09:31:16.000000 gester-1.1.0/src/gest.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:41:33.571623 gester-1.1.0/src/gester.egg-info/
--rw-rw-rw-   0        0        0     2808 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 06:27:12.909800 gester-1.2.0/
+-rw-rw-rw-   0        0        0     1361 2023-04-08 06:55:38.000000 gester-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3716 2023-04-12 06:27:12.909800 gester-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      965 2023-04-09 12:07:01.000000 gester-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1211 2023-04-12 06:22:58.000000 gester-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 06:27:12.909800 gester-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 06:27:12.847400 gester-1.2.0/src/
+-rw-rw-rw-   0        0        0       23 2023-04-12 06:22:21.000000 gester-1.2.0/src/__init__.py
+-rw-rw-rw-   0        0        0     7286 2023-04-12 06:02:48.000000 gester-1.2.0/src/gest.py
+drwxrwxrwx   0        0        0        0 2023-04-12 06:27:12.878600 gester-1.2.0/src/gester.egg-info/
+-rw-rw-rw-   0        0        0     3716 2023-04-12 06:27:12.000000 gester-1.2.0/src/gester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-12 06:27:12.000000 gester-1.2.0/src/gester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 06:27:12.000000 gester-1.2.0/src/gester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-12 06:27:12.000000 gester-1.2.0/src/gester.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 06:27:12.000000 gester-1.2.0/src/gester.egg-info/top_level.txt
```

### Comparing `gester-1.1.0/LICENSE` & `gester-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gester-1.1.0/pyproject.toml` & `gester-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gester"
-version = "1.1.0"
+version = "1.2.0"
 description = "A game engine for console based text game"
 readme = "README.md"
 keywords = ["games", "game development", "game engine", "console"]
 license = {file = "LICENSE"}
 authors = [
     {name = "etcetra7n", email = "greeknio@gmail.com"}
 ]
```

### Comparing `gester-1.1.0/src/gest.py` & `gester-1.2.0/src/gest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from sys import argv, stdout, exit
 from time import sleep
 from os.path import isfile, abspath
 import re
 #from keyboard import is_pressed
 import pickle
-import colorama
 from colorama import Fore
 
 def init_in_game_vars(gest_file):
     in_game_vars['gest_file'] = abspath(gest_file)
     in_game_vars['line_index'] = 0
     gsav_file = re.search(r'^(.+?)\.gest$', abspath(gest_file))
     in_game_vars['gsav_file'] = gsav_file.group(1) + '.gsav'
+    in_game_vars['_scene_return'] = []
     return
 
 def save():
     gsav_file.seek(0)
     pickle.dump(in_game_vars, gsav_file)
 
 def trim(str):
@@ -27,24 +27,35 @@
             break
     for i, c in enumerate(reversed(str)):
         if(c != ' '):
             end = len(str)-i
             break
     return str[begin:end]
 
+def block(str, lines):
+    jump_index = 0
+    for i in range(in_game_vars['line_index']+1, len(lines)):
+        if re.match(r' *\[ *'+str+r' *\]', lines[i]):
+            jump_index = i+1
+            break
+    else:
+        print(Fore.RED + "\nnScript Error: " + Fore.RESET +"["+ str +"] not found")
+        exit()
+    return jump_index
+
 def txtout(txt):
 
     '''
     EMBEDDED VARIBLE
     Syntax:
         some text {var} some text...
     for example:
         My name is {name}
     '''
-    embedded_var = re.findall(r'\{[ ]*(.+?)[ ]*\}', txt)
+    embedded_var = re.findall(r'\{ *(.+?) *\}', txt)
     for var in embedded_var:
         txt = re.sub(r'(\{.+?\})', in_game_vars[var], txt, count = 1)
 
     for char in txt:
         print(char, end='')
         stdout.flush()
         sleep(0.02)
@@ -72,15 +83,15 @@
             '''
             COMMAND WITH VARIABLE
             Syntax:
                 [command: var] text
             for example:
                 [input: name] Enter your name:
             '''
-            com = re.search(r'\[[ ]*(.+?)[ ]*:[ ]*(.+?)[ ]*\][ ]*(.+?)$', line)
+            com = re.search(r'\[ *(.+?) *: *(.+?) *\] *(.+?)?$', line)
             if com:
                 command = com.group(1)
                 var = com.group(2)
                 prompt = com.group(3)
                 if(command == 'input'):
                     '''
                     INPUT COMMAND
@@ -111,19 +122,32 @@
                     txtout(prompt + ' (y/n): ')
                     inp = input()
                     if inp == 'y':
                         in_game_vars[var] = 'yes'
                     elif inp == 'n':
                         in_game_vars[var] = 'no'
                     else:
-                        txtout(Fore.YELLOW + "\nInvalid input:"+ Fore.RESET +" Try again\n\n"+ Fore.RESET)
+                        txtout(Fore.YELLOW + "\nInvalid input:"+ Fore.RESET +" Try again\n\n")
                         continue
                     line_index += 1
                     continue
 
+            play_scene = re.search(r'\[ *play *: *(.+?) *\]', line)
+            if play_scene:
+                in_game_vars['_scene_return'].append(line_index+1)
+                scene_name = play_scene.group(1)
+                for l in range(len(lines)):
+                    if re.match(r' *\[ *scene *: *'+ scene_name + r' *\]', lines[l]):
+                        line_index = l+1
+                        break
+                else:
+                    print(Fore.RED+"\nScript Error:"+Fore.RESET+" Scene `"+scene_name+"` is not defined")
+                    exit()
+                continue
+
             '''
             VARIABLE EQUALITY CONDITION
             Syntax:
                 [{var} value]
                 ...
                 [endblock]
 
@@ -135,36 +159,35 @@
 
                     (OR)
 
                 [{var} 'value']
                 ...
                 [endblock]
             '''
-            con = re.search(r'\[[ ]*\{(.+?)\}[ ]+[\'"]?(.+?)[\'"]?[ ]*\]', line)
+            con = re.search(r'\[ *\{(.+?)\} +[\'"]?(.+?)[\'"]? *\]', line)
             if con:
                 if in_game_vars[con.group(1)] == con.group(2):
                     line_index += 1
                     continue
 
                 else:
-                    jump_to = line_index
-                    for i in range(line_index+1, len(lines)):
-                        if re.match(r'\[[ ]*endblock[ ]*\]', lines[i]):
-                            jump_to = i+1
-                            break
-                    else:
-                        print(Fore.RED + "\nError:" + Fore.RESET +" endblock not found")
-                        exit()
-                    line_index = jump_to
+                    line_index = block('endblock', lines)+1
                     continue
+            if re.match(r' *\[ *scene *: *(.+?) *\]', line):
+                line_index = block('endscene', lines)+1
+                continue
+
+            if re.match(r' *\[ *endscene *\]', line):
+                line_index = in_game_vars['_scene_return'].pop() #returns and removes the last indice
+                continue
 
-            if re.match(r'[ ]*\[[ ]*endblock[ ]*\]', line):
+            if re.match(r' *\[ *endblock *\]', line):
                 line_index += 1
                 continue
-            if re.match(r'[ ]*\[[ ]*abort[ ]*\]', line):
+            if re.match(r' *\[ *abort *\]', line):
                 break
 
             txtout(trim(line))
             line_index += 1
     save()
 
 def main():
```

