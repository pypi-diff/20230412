# Comparing `tmp/clara_ai-0.0.1.tar.gz` & `tmp/clara_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clara_ai-0.0.1.tar", max compression
+gzip compressed data, was "clara_ai-0.0.2.tar", max compression
```

## Comparing `clara_ai-0.0.1.tar` & `clara_ai-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1534 2023-04-12 17:21:29.648887 clara_ai-0.0.1/LICENSE
--rw-r--r--   0        0        0      693 2023-04-12 17:21:29.648887 clara_ai-0.0.1/README.md
--rw-r--r--   0        0        0     1916 2023-04-12 17:21:29.648887 clara_ai-0.0.1/clara/cli.py
--rw-r--r--   0        0        0       54 2023-04-12 17:21:29.648887 clara_ai-0.0.1/clara/console.py
--rw-r--r--   0        0        0     1682 2023-04-12 17:21:29.648887 clara_ai-0.0.1/clara/consts.py
--rw-r--r--   0        0        0     3517 2023-04-12 17:21:29.648887 clara_ai-0.0.1/clara/index.py
--rw-r--r--   0        0        0      545 2023-04-12 17:21:29.652887 clara_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 clara_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1534 2023-04-12 20:56:15.471438 clara_ai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1888 2023-04-12 20:56:15.471438 clara_ai-0.0.2/README.md
+-rw-r--r--   0        0        0     2558 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/cli.py
+-rw-r--r--   0        0        0       54 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/console.py
+-rw-r--r--   0        0        0     1682 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/consts.py
+-rw-r--r--   0        0        0     3269 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/index.py
+-rw-r--r--   0        0        0      545 2023-04-12 20:56:15.471438 clara_ai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 clara_ai-0.0.2/PKG-INFO
```

### Comparing `clara_ai-0.0.1/LICENSE` & `clara_ai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.1/clara/cli.py` & `clara_ai-0.0.2/clara/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,62 @@
-import fire
 import logging
+import shutil
+
+import fire
+from rich.prompt import Confirm
 
 from .console import console
-from .index import RepositoryIndexPersisted
+from .index import RepositoryIndex, RepositoryIndexPersisted
 
 
 # Disable ChromaDB logging
 logger = logging.getLogger("chromadb").setLevel(logging.ERROR)
 
 
 class Clara:
     """CLARA: Code Language Assistant & Repository Analyzer"""
 
     def config(self, path: str = "."):
-        """Get config for a given path"""
+        """Show config for a given path."""
         index = RepositoryIndexPersisted(path)
         console.print(f"Vector DB persist path = [blue underline]{index.persist_path}")
 
-    def chat(self, path: str = "."):
-        """Chat about the code"""
+    def clean(self, path: str = "."):
+        """Delete vector DB for a given path."""
         index = RepositoryIndexPersisted(path)
+        if Confirm.ask(
+            "Are you sure you want to remove "
+            f"[blue underline]{index.persist_path}[/blue underline]?",
+            default=False,
+        ):
+            shutil.rmtree(index.persist_path)
+
+    def chat(self, path: str = ".", memory_storage: bool = False):
+        """Chat about the code."""
+
+        if memory_storage:
+            index = RepositoryIndex(path)
 
-        if not index.load():
+        else:
+            index = RepositoryIndexPersisted(path)
+
+        if memory_storage or not index.load():
             with console.status(
                 f"Ingesting code repository from path: [blue underline]{path} …",
                 spinner="weather",
             ):
                 index.ingest()
 
-            with console.status(
-                f"Storing vector database in path: [blue underline]{index.persist_path} …",
-                spinner="weather",
-            ):
-                index.persist()
+            if not memory_storage:
+                with console.status(
+                    "Storing vector database in path: "
+                    "[blue underline]{index.persist_path} …",
+                    spinner="weather",
+                ):
+                    index.persist()
 
         console.rule("[bold blue]CHAT")
         console.print("Hi, I'm Clara!", ":scroll::mag::robot:")
         console.print("How can I help you?")
         console.print()
 
         try:
```

### Comparing `clara_ai-0.0.1/clara/consts.py` & `clara_ai-0.0.2/clara/consts.py`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.1/clara/index.py` & `clara_ai-0.0.2/clara/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         return matched_files
 
     def load(self) -> List[Document]:
         """Load from file path."""
         documents = []
         for file_path in self._get_files_by_wildcards(self.path, self.wildcards):
-            console.log(f"Adding: [blue underline]{file_path}", "…")
+            console.log(f"Loading [blue underline]{file_path}", "…")
             with open(file_path, encoding=self.encoding) as f:
                 text = f.read()
             metadata = {"source": file_path}
             documents.append(Document(page_content=text, metadata=metadata))
         return documents
 
 
@@ -51,45 +51,38 @@
     question: str
     answer: str
     sources: str
 
 
 class RepositoryIndex:
     def __init__(self, path: str):
-        self.path = path
+        self.path = os.path.abspath(path)
         self.index = None
 
     def ingest(self):
         code_loader = MultipleTextLoader(self.path, WILDCARDS)
         self.index = VectorstoreIndexCreator().from_loaders([code_loader])
 
     def query_with_sources(self, query: str) -> QueryResult:
         return QueryResult(**self.index.query_with_sources(query))
 
 
-class RepositoryIndexPersisted:
+class RepositoryIndexPersisted(RepositoryIndex):
     def __init__(self, path: str):
-        self.path = pathlib.Path(path).resolve()
-        self.index = None
-
+        super().__init__(path)
         self.persist_path = self.get_persist_path()
 
     def get_persist_path(self) -> str:
         hashed_path = hashlib.sha256(str(self.path).encode("utf-8")).hexdigest()
         short_hash = hashed_path[:8]
-
         base_name = os.path.basename(self.path)
-
         return os.path.join(BASE_PERSIST_PATH, f"{base_name}_{short_hash}")
 
     def ingest(self):
-        console.log("Create persist directory:", self.persist_path)
         pathlib.Path(self.persist_path).mkdir(parents=True, exist_ok=True)
-        console.log("Done! :check:")
-
         code_loader = MultipleTextLoader(self.path, WILDCARDS)
         self.index = VectorstoreIndexCreator(
             vectorstore_kwargs={"persist_directory": self.persist_path}
         ).from_loaders([code_loader])
 
     def persist(self):
         self.index.vectorstore.persist()
@@ -101,10 +94,7 @@
         vectorstore = Chroma(
             persist_directory=self.persist_path,
             embedding_function=OpenAIEmbeddings(),
         )
         self.index = VectorStoreIndexWrapper(vectorstore=vectorstore)
 
         return True
-
-    def query_with_sources(self, query: str) -> QueryResult:
-        return QueryResult(**self.index.query_with_sources(query))
```

### Comparing `clara_ai-0.0.1/pyproject.toml` & `clara_ai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clara-ai"
-version = "0.0.1"
+version = "0.0.2"
 description = "CLARA: Code Language Assistant & Repository Analyzer"
 authors = ["Cristóbal Carnero Liñán <cristobal@seednapse.ai>"]
 readme = "README.md"
 packages = [{include = "clara"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

