# Comparing `tmp/folder_tree_generator-0.1.1.tar.gz` & `tmp/folder_tree_generator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folder_tree_generator-0.1.1.tar", max compression
+gzip compressed data, was "folder_tree_generator-0.1.3.tar", max compression
```

## Comparing `folder_tree_generator-0.1.1.tar` & `folder_tree_generator-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2064 2023-04-08 17:38:53.034685 folder_tree_generator-0.1.1/README.md
--rw-r--r--   0        0        0     3003 2023-04-11 22:24:34.256693 folder_tree_generator-0.1.1/folder_tree_generator.py
--rw-r--r--   0        0        0      562 2023-04-11 22:39:02.619532 folder_tree_generator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2437 2023-04-11 23:35:17.507501 folder_tree_generator-0.1.3/README.md
+-rw-r--r--   0        0        0     3003 2023-04-11 22:24:34.256693 folder_tree_generator-0.1.3/folder_tree_generator.py
+-rw-r--r--   0        0        0      562 2023-04-11 23:35:27.187919 folder_tree_generator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.3/PKG-INFO
```

### Comparing `folder_tree_generator-0.1.1/folder_tree_generator.py` & `folder_tree_generator-0.1.3/folder_tree_generator.py`

 * *Files identical despite different names*

### Comparing `folder_tree_generator-0.1.1/pyproject.toml` & `folder_tree_generator-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "folder-tree-generator"
-version = "0.1.1"
+version = "0.1.3"
 description = "Takes a folder path and outputs a text representation of the folders and files, supports ignore files."
 authors = ["Sean Dearnaley <SeanDearnaley@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 coverage = "^7.2.3"
```

### Comparing `folder_tree_generator-0.1.1/PKG-INFO` & `folder_tree_generator-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,99 @@
 Metadata-Version: 2.1
 Name: folder-tree-generator
-Version: 0.1.1
+Version: 0.1.3
 Summary: Takes a folder path and outputs a text representation of the folders and files, supports ignore files.
 Author: Sean Dearnaley
 Author-email: SeanDearnaley@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coverage (>=7.2.3,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Folder Tree Generator
 
-This script generates a tree representation of a folder's structure, including subfolders and files. It also takes into account `.gitignore` files to exclude ignored files and folders from the generated tree.
 
-## Why?
-
-I needed a way to generate folder structures in a standard text format that I could copy and paste into GPT without including all the build artifacts, eg. repository structures for code analysis.  If you wanted to make your own ignore file it should be a simple adapation of a gitignore file, in 90% of my use cases, the gitignore is sufficient.
-
-## Usage
+[![PyPI version](https://badge.fury.io/py/folder-tree-generator.svg)](https://badge.fury.io/py/folder-tree-generator)
 
-To use the script, run the following command:
+![Test](https://github.com/seandearnaley/folder-tree-generator/workflows/Run%20pytest/badge.svg)
 
-```bash
-python3 main.py <root_folder>
-```
-
-Replace `<root_folder>` with the path to the folder you want to generate the tree for.
 
-## Example
+Folder Tree Generator is a Python module that takes a folder path and outputs a text representation of the folders and files. It supports ignore files, such as `.gitignore`, to exclude certain files or folders from the output.
 
-Suppose you have the following folder structure:
+typical string output:
 
-```
+```text
 my_project/
 |-- .gitignore
 |-- main.py
 |-- utils.py
 |-- data/
 |   |-- input.txt
 |   |-- output.txt
 ```
 
-And the `.gitignore` file contains:
+## Why?
+
+I needed a way to generate folder structures in a standard text format that I could copy and paste into GPT without including all the build artifacts, eg. repository structures for code analysis.  If you wanted to make your own ignore file it should be a simple adapation of a gitignore file, in 90% of my use cases, the gitignore is sufficient.
+
+## Installation
+
+You can install the module from PyPI using pip:
+
+```bash
+pip install folder-tree-generator
+```
+
+## Usage
+
+You can use the module as a command-line tool or import it in your Python script.
+
+### Command-line usage
 
+```bash
+python -m folder_tree_generator /path/to/your/folder
 ```
-data/output.txt
+
+### Python script usage
+
+```python
+from folder_tree_generator import generate_tree
+
+output_text = generate_tree("/path/to/your/folder")
+print(output_text)
 ```
 
-Running the script with `python3 main.py my_project` will output the following tree:
+## Configuration
+
+By default, the module looks for a `.gitignore` file in the root folder to determine which files and folders to ignore. You can change the ignore file name by passing an optional argument to the `generate_tree` function:
 
+```python
+output_text = generate_tree("/path/to/your/folder", ignore_file_name=".myignore")
 ```
-my_project/
-|-- .gitignore
-|-- main.py
-|-- utils.py
-|-- data/
-|   |-- input.txt
+
+## Development
+
+To set up the development environment, clone the repository and install the required dependencies using Poetry:
+
+```bash
+git clone https://github.com/seandearnaley/folder-tree-generator.git
+cd folder-tree-generator
+poetry install
 ```
 
-As you can see, the `data/output.txt` file is excluded from the tree because it's listed in the `.gitignore` file.
+To run the tests, use the following command:
 
-## Functions
+```bash
+poetry run pytest
+```
 
-The script contains the following functions:
+Make sure to update the README.md file with these changes.
 
-- `parse_gitignore(gitignore_path: Path) -> List[str]`: Parses a `.gitignore` file and returns a list of ignored patterns.
-- `should_ignore(entry: Path, ignored_patterns: List[str]) -> bool`: Checks if a file or folder should be ignored based on the list of ignored patterns.
-- `generate_tree(root: Path, indent: str = "", ignored_patterns: Optional[List[str]] = None) -> str`: Generates a tree of a folder, taking into account the ignored patterns.
-- `main(root_folder: str) -> None`: The main function that takes the root folder as an argument and prints the generated tree.
+## Contributing
 
-## Requirements
+Contributions are welcome! Please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/seandearnaley/folder-tree-generator).
 
-- Python 3.6 or higher
-- The `pathlib` library (included in the Python standard library since version 3.4)
+## License
 
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

