# Comparing `tmp/eric_chen_forward-0.0.5.tar.gz` & `tmp/eric_chen_forward-0.0.6.tar.gz`

## Comparing `eric_chen_forward-0.0.5.tar` & `eric_chen_forward-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/eric_chen_forward/database.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/eric_chen_forward/model.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/eric_chen_forward/url_classifier_demo.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/eric_chen_forward/util.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/LICENSE
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/eric_chen_forward/database.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/eric_chen_forward/model.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/eric_chen_forward/url_classifier_demo.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/eric_chen_forward/util.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/LICENSE
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.6/PKG-INFO
```

### Comparing `eric_chen_forward-0.0.5/eric_chen_forward/model.py` & `eric_chen_forward-0.0.6/eric_chen_forward/model.py`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.5/eric_chen_forward/url_classifier_demo.py` & `eric_chen_forward-0.0.6/eric_chen_forward/url_classifier_demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,100 +4,70 @@
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 from trafilatura import fetch_url, extract
 from trafilatura.settings import use_config
 from transformers import AutoTokenizer, BartForConditionalGeneration
 
-def Demo(max_summary_length=100):
-    with open('model.pkl', 'rb') as f:
+def Demo(model_file_path, max_summary_length=100):
+    
+    with open(model_file_path, 'rb') as f:
         model = pickle.load(f)
 
-    def extract_paragraphs(url, use_trafilatura=False):
-        if use_trafilatura:
-            config = use_config()
-            config.set("DEFAULT", "EXTRACTION_TIMEOUT", "0")
-            downloaded = fetch_url(url)
-            result = extract(downloaded, config=config)
-            return result
-        else:
-            data = requests.get(url).text
-            soup = BeautifulSoup(data, 'lxml')
-            h = soup.find('header')
-            if h:
-                h.decompose()
-            f = soup.find('footer')
-            if f:
-                f.decompose()
-            if soup.body is None:
-                return None
-            
-            paragraphs = []
-            for p in soup.find_all('p'):
-                if len(p) > 0 and 'block' not in p:
-                    text = p.get_text(strip=True, separator='\n')
-                    if len(paragraphs) > 0 and len(paragraphs[-1].split()) < 100:
-                        paragraphs[-1] += text
-                    else:
-                        paragraphs.append(text)
-            return paragraphs
+    def extract_paragraphs(url):
+        config = use_config()
+        config.set("DEFAULT", "EXTRACTION_TIMEOUT", "0")
+        downloaded = fetch_url(url)
+        result = extract(downloaded, config=config, output_format='xml', include_links=True, include_formatting=True)
+
+        soup = BeautifulSoup(result, 'lxml')
+        paragraphs = []
+        for p in soup.find_all('p'):
+            text = p.get_text(strip=True, separator='\n')
+            if '.' in text:
+                paragraphs.append(text)
+        return paragraphs
 
 
 
     title = st.text_input(label="Enter url", placeholder='url')
 
-    tab1, tab2, tab3, tab4 = st.tabs(['BeautifulSoup', 'Trafilatura', 'BeautifulSoup + Summarization', 'Trafilatura + Summarization'])
+    tab1, tab2, tab3 = st.tabs(['Paragraph form', 'Passage form', 'Passage form + summarization'])
 
     bart_model = BartForConditionalGeneration.from_pretrained("facebook/bart-large-cnn")
     tokenizer = AutoTokenizer.from_pretrained("facebook/bart-large-cnn")
 
     if title:
-        paragraphs1 = extract_paragraphs(title, use_trafilatura=False)
-        paragraphs2 = extract_paragraphs(title, use_trafilatura=True)
+        paragraphs = extract_paragraphs(title)
+        passage = ' '.join(paragraphs)
         with tab1:
-            for paragraph in paragraphs1:
+            for paragraph in paragraphs:
                 cleaned_text = util.clean_document(paragraph)
                 if len(cleaned_text) == 0:
                     continue
                 temp = pd.DataFrame()
                 temp['cleaned_text'] = [cleaned_text]
                 temp['num_years'] = [util.num_years(paragraph)]
                 pred = model.predict(temp[['cleaned_text', 'num_years']])
                 
                 st.write("Predicted Category: " + pred[0])
                 st.write(paragraph)
                 st.markdown('''---''')
         with tab2:
-            cleaned_text = util.clean_document(paragraphs2)
+            cleaned_text = util.clean_document(passage)
             temp = pd.DataFrame()
             temp['cleaned_text'] = [cleaned_text]
-            temp['num_years'] = [util.num_years(paragraphs2)]
+            temp['num_years'] = [util.num_years(passage)]
             pred = model.predict(temp[['cleaned_text', 'num_years']])
             
             st.write("Predicted Category: " + pred[0])
-            st.write(paragraphs2)
+            st.write(passage)
             st.markdown('''---''')
         with tab3:
-            for paragraph in paragraphs1:
-                inputs = tokenizer([paragraph], max_length=1024, return_tensors="pt")
-                summary_ids = bart_model.generate(inputs["input_ids"], num_beams=2, min_length=0, max_length=max_summary_length)
-                summary = tokenizer.batch_decode(summary_ids, skip_special_tokens=True, clean_up_tokenization_spaces=False, truncation=True)[0]
-                cleaned_text = util.clean_document(summary)
-                if len(cleaned_text) == 0:
-                    continue
-                temp = pd.DataFrame()
-                temp['cleaned_text'] = [cleaned_text]
-                temp['num_years'] = [util.num_years(summary)]
-                pred = model.predict(temp[['cleaned_text', 'num_years']])
-                
-                st.write("Predicted Category: " + pred[0])
-                st.write(summary)
-                st.markdown('''---''')
-        with tab4:
-            inputs = tokenizer([paragraphs2], max_length=1024, return_tensors="pt")
+            inputs = tokenizer([passage], max_length=1024, return_tensors="pt")
             summary_ids = bart_model.generate(inputs["input_ids"], num_beams=2, min_length=0, max_length=max_summary_length)
             summary = tokenizer.batch_decode(summary_ids, skip_special_tokens=True, clean_up_tokenization_spaces=False, truncation=True)[0]
             cleaned_text = util.clean_document(summary)
             temp = pd.DataFrame()
             temp['cleaned_text'] = [cleaned_text]
             temp['num_years'] = [util.num_years(summary)]
             pred = model.predict(temp[['cleaned_text', 'num_years']])
```

### Comparing `eric_chen_forward-0.0.5/eric_chen_forward/util.py` & `eric_chen_forward-0.0.6/eric_chen_forward/util.py`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.5/.gitignore` & `eric_chen_forward-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.5/LICENSE` & `eric_chen_forward-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.5/README.md` & `eric_chen_forward-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     model = pickle.load(f)
 ```
 
 To run the classifier demo:
 ```python
 from eric_chen_forward import url_classifier_demo
 
-url_classifier_demo.Demo()
+url_classifier_demo.Demo('file path of model.pkl')
 ```
```

### Comparing `eric_chen_forward-0.0.5/pyproject.toml` & `eric_chen_forward-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "eric_chen_forward"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Eric Chen", email="ezchen2556@gmail.com" },
 ]
 description = "Classifier for institution and scholar data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `eric_chen_forward-0.0.5/PKG-INFO` & `eric_chen_forward-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eric_chen_forward
-Version: 0.0.5
+Version: 0.0.6
 Summary: Classifier for institution and scholar data
 Project-URL: Homepage, https://github.com/ezrc2/eric_chen_forward
 Author-email: Eric Chen <ezchen2556@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -48,9 +48,9 @@
     model = pickle.load(f)
 ```
 
 To run the classifier demo:
 ```python
 from eric_chen_forward import url_classifier_demo
 
-url_classifier_demo.Demo()
+url_classifier_demo.Demo('file path of model.pkl')
 ```
```

