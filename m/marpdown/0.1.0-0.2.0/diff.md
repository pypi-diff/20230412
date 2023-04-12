# Comparing `tmp/marpdown-0.1.0.tar.gz` & `tmp/marpdown-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marpdown-0.1.0.tar", last modified: Wed Apr 12 15:01:49 2023, max compression
+gzip compressed data, was "marpdown-0.2.0.tar", last modified: Wed Apr 12 15:35:43 2023, max compression
```

## Comparing `marpdown-0.1.0.tar` & `marpdown-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:01:49.990766 marpdown-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      404 2023-04-12 15:01:49.989766 marpdown-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 15:01:49.980763 marpdown-0.1.0/marpdown/
--rw-rw-rw-   0        0        0       83 2023-04-12 14:41:19.000000 marpdown-0.1.0/marpdown/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-04-12 13:42:16.000000 marpdown-0.1.0/marpdown/css.py
--rw-rw-rw-   0        0        0     2440 2023-04-12 14:58:53.000000 marpdown-0.1.0/marpdown/ppt.py
--rw-rw-rw-   0        0        0     1468 2023-04-12 14:53:02.000000 marpdown-0.1.0/marpdown/slide.py
--rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.1.0/marpdown/writer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:01:49.988601 marpdown-0.1.0/marpdown.egg-info/
--rw-rw-rw-   0        0        0      404 2023-04-12 15:01:49.000000 marpdown-0.1.0/marpdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-12 15:01:49.000000 marpdown-0.1.0/marpdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:01:49.000000 marpdown-0.1.0/marpdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 15:01:49.000000 marpdown-0.1.0/marpdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 15:01:49.990766 marpdown-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-04-12 15:01:13.000000 marpdown-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:35:43.300639 marpdown-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-04-12 15:35:43.299638 marpdown-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 15:35:43.289650 marpdown-0.2.0/marpdown/
+-rw-rw-rw-   0        0        0       83 2023-04-12 14:41:19.000000 marpdown-0.2.0/marpdown/__init__.py
+-rw-rw-rw-   0        0        0     2138 2023-04-12 15:33:58.000000 marpdown-0.2.0/marpdown/css.py
+-rw-rw-rw-   0        0        0     2545 2023-04-12 15:26:33.000000 marpdown-0.2.0/marpdown/ppt.py
+-rw-rw-rw-   0        0        0     1518 2023-04-12 15:20:25.000000 marpdown-0.2.0/marpdown/slide.py
+-rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.2.0/marpdown/writer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:35:43.297652 marpdown-0.2.0/marpdown.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:35:43.300639 marpdown-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-04-12 15:35:28.000000 marpdown-0.2.0/setup.py
```

### Comparing `marpdown-0.1.0/LICENSE` & `marpdown-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marpdown-0.1.0/marpdown/css.py` & `marpdown-0.2.0/marpdown/css.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,32 +61,33 @@
   border-radius: 50%;
 }
 
 .timeline-content {
   padding-left: 60px;
 }'''
 
-TOC = '''.highlight-wrapper {
+TOC = '''
+.highlight-wrapper {
     margin-bottom: 1.25em; /* 添加底部边距，可根据需要调整 */
   }
 
    .highlight-container {
     position: absolute;
     left: 0;
     right: 0;
     background-color: #0065bd; /* 设置背景颜色为蓝色 */
     padding-left: 3.17em; /* 添加左边距，可根据需要调整 */
-    padding-top: 0.2em; /* 添加左边距，可根据需要调整 */
     padding-bottom: 0.2em; /* 添加左边距，可根据需要调整 */
     display: flex; /* 设置为弹性布局 */
     align-items: center; /* 垂直居中 */
     height: 1.5em; /* 设置容器高度 */
   }
   
   .highlight {
     color: #ffffff; /* 设置字体颜色为白色 */
     margin: 0; /* 移除默认的margin */
-  }'''
+  }
+'''
 
 def load_css():
     tmp = [BASE,TOC,TIMELINE]
     return '\n'.join(tmp)
```

### Comparing `marpdown-0.1.0/marpdown/ppt.py` & `marpdown-0.2.0/marpdown/ppt.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,39 +18,43 @@
         self.paginate = paginate
         self._class = _class
         self.backgroundImage = backgroundImage
 
 
 
     def __setup__(self):
-        self.writer.append(f'''---\nmarp: true\nfooter: {self.footer}\npaginate: {self.paginate}''')
+        self.writer.append(f'''---\nmarp: true\nfooter: "{self.footer}"\npaginate: {self.paginate}''')
         if self._class is not None:
             self.writer.append(f"_class: {self._class}")
         if self.backgroundImage is not None:
-            self.writer.append(f"backgroundImage: {self.backgroundImage}")
+            self.writer.append(f"backgroundImage: url('{self.backgroundImage}')")
         self.__start_new_slide__()
         self.writer.append('<style>')
         self.writer.append(load_css())
         self.writer.append('</style>')
 
     def build(self):
         self.writer.clear()
         self.__setup__()
         s = self.slides[0]
-        if s.bgimage is not None:
-            self.writer.append(f'![bg]({s.bgimage})')
+        self.__build_bgimage__(s)
         self.writer.append(s.content)
 
         for s in self.slides[1:]:
             self.__start_new_slide__()
-            if s.bgimage is not None:
-                self.writer.append(f'![bg]({s.bgimage})')
+            self.__build_bgimage__(s)
             self.writer.append(s.content)
         return self.writer.getValue()
 
+    def __build_bgimage__(self, s):
+        if s.bgimage is not None:
+            self.writer.append(f'![bg]({s.bgimage})')
+        else:
+            self.writer.append(f'![bg]({self.backgroundImage})')
+
     def store(self,path:str, overwrite = True):
         self.build()
         self.writer.store(path, overwrite)
 
     # subscriptable and slice-able
     def __getitem__(self, item):
         return self.slides[item]
```

### Comparing `marpdown-0.1.0/marpdown/slide.py` & `marpdown-0.2.0/marpdown/slide.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 class BaseSlide:
-    def __init__(self,content:str='',backgroundImage: str = None, ):
+    def __init__(self,*,content:str='',backgroundImage: str = None, ):
         self.content = content
         self.bgimage = backgroundImage
 
 class TOCSlide(BaseSlide):
     def __init__(self, title: str, toc: list[str],focus = -1,backgroundImage: str = None):
         self.toc = toc
         content = f'''# {title}\n\n'''
         if focus == -1:
             tmp = [f'''### {i+1}. {t}''' for i,t in enumerate(toc)]
             content += '\n'.join(tmp)
         else:
             tmp = [f'''### {i + 1}. {t}''' for i, t in enumerate(toc)]
             tmp[focus] = f'''### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> {focus+1}. {toc[focus]}</div></div></div>'''
             content += '\n'.join(tmp)
-        super().__init__(content, backgroundImage)
+        super().__init__(content=content, backgroundImage=backgroundImage)
 
 class TimelineSlide(BaseSlide):
     def __init__(self, title:str,timelines: list[tuple],backgroundImage: str = None,):
         content ="# " + title + "\n"
         content += '''<ul class="timeline">\n'''
         for tl in timelines:
             name, detail = tl
@@ -27,8 +27,8 @@
                         <div class="timeline-marker"></div>
                         <div class="timeline-content">
                           <h4>{name}</h4>
                           {detail}
                         </div></li>'''
         content += '</ul>'
 
-        super().__init__(content, backgroundImage)
+        super().__init__(content=content, backgroundImage=backgroundImage)
```

### Comparing `marpdown-0.1.0/marpdown/writer.py` & `marpdown-0.2.0/marpdown/writer.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.1.0/setup.py` & `marpdown-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
 
 ]
 
 setup(
     name="marpdown",
-    version="0.1.0",
+    version="0.2.0",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of RL algorithms",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/marpdown",
     packages=find_packages(),
```

