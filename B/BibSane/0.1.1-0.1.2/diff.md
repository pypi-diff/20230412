# Comparing `tmp/BibSane-0.1.1.tar.gz` & `tmp/BibSane-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BibSane-0.1.1.tar", last modified: Fri Mar 24 18:13:02 2023, max compression
+gzip compressed data, was "BibSane-0.1.2.tar", last modified: Wed Apr 12 08:16:56 2023, max compression
```

## Comparing `BibSane-0.1.1.tar` & `BibSane-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-03-24 18:13:02.024156 BibSane-0.1.1/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-03-24 18:13:02.024156 BibSane-0.1.1/BibSane.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43613 2023-03-24 18:13:02.000000 BibSane-0.1.1/BibSane.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      231 2023-03-24 18:13:02.000000 BibSane-0.1.1/BibSane.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-03-24 18:13:02.000000 BibSane-0.1.1/BibSane.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       41 2023-03-24 18:13:02.000000 BibSane-0.1.1/BibSane.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2023-03-24 18:13:02.000000 BibSane-0.1.1/BibSane.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2023-03-24 18:13:02.000000 BibSane-0.1.1/BibSane.egg-info/top_level.txt
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2023-03-21 10:14:38.000000 BibSane-0.1.1/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43613 2023-03-24 18:13:02.024156 BibSane-0.1.1/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     2110 2023-03-24 18:08:11.000000 BibSane-0.1.1/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)    19319 2023-03-24 18:08:11.000000 BibSane-0.1.1/bibsane.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1152 2023-03-24 18:11:59.000000 BibSane-0.1.1/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-03-24 18:13:02.024156 BibSane-0.1.1/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:16:56.152399 BibSane-0.1.2/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:16:56.152399 BibSane-0.1.2/BibSane.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    43635 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)      231 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       41 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       33 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        8 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/top_level.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)    35149 2023-03-21 10:14:38.000000 BibSane-0.1.2/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)    43635 2023-04-12 08:16:56.152399 BibSane-0.1.2/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     2110 2023-03-24 18:08:11.000000 BibSane-0.1.2/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)    20484 2023-04-12 08:15:05.000000 BibSane-0.1.2/bibsane.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1152 2023-04-12 01:32:16.000000 BibSane-0.1.2/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-12 08:16:56.152399 BibSane-0.1.2/setup.cfg
```

### Comparing `BibSane-0.1.1/BibSane.egg-info/PKG-INFO` & `BibSane-0.1.2/BibSane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BibSane
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sanitize BibTeX files without going insane
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,14 +689,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: COPYING
 
 # BibSane
 
 Sanitize BibTeX files without going insane.
 
 BibSane is comparable to [bibexport](https://www.ctan.org/pkg/bibexport) and [checkcites](https://www.ctan.org/tex-archive/support/checkcites), but has a few important improvements.
```

### Comparing `BibSane-0.1.1/COPYING` & `BibSane-0.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `BibSane-0.1.1/PKG-INFO` & `BibSane-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BibSane
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sanitize BibTeX files without going insane
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,14 +689,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: COPYING
 
 # BibSane
 
 Sanitize BibTeX files without going insane.
 
 BibSane is comparable to [bibexport](https://www.ctan.org/pkg/bibexport) and [checkcites](https://www.ctan.org/tex-archive/support/checkcites), but has a few important improvements.
```

### Comparing `BibSane-0.1.1/README.md` & `BibSane-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `BibSane-0.1.1/bibsane.py` & `BibSane-0.1.2/bibsane.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 import argparse
 import enum
 import hashlib
 import json
 import os
 import re
 import shutil
-import sys
 import tempfile
 import urllib.parse
 import urllib.request
+from collections.abc import Collection
 from glob import glob
 
 import attrs
 import bibtexparser
 import cattrs
 import yaml
 
@@ -79,14 +79,15 @@
     abbreviate_journal: str = attrs.field(default=None)
     # sort key = {year}{first author lowercase last name}
     sort: bool = attrs.field(default=False)
     citation_policies: dict[str, dict[str, FieldPolicy]] = attrs.field(default=attrs.Factory(dict))
 
     @classmethod
     def from_file(cls, fn_yaml):
+        """Instantiate a configuration from a YAML config file."""
         if fn_yaml is None:
             config = Config()
             config.root = os.getcwd()
         else:
             with open(fn_yaml) as f:
                 data = yaml.safe_load(f)
                 config = cattrs.structure(data, Config)
@@ -95,52 +96,49 @@
 
 
 RETURN_CODE_UNCHANGED = 0
 RETURN_CODE_CHANGED = 1
 RETURN_CODE_BROKEN = 2
 
 
-def main():
-    fns_aux, config, verbose = parse_args()
+def main() -> int:
+    """Bibsane main program."""
+    fns_aux, verbose, config = parse_args()
     if len(fns_aux) == 0:
         # Only select aux files for which corresponding tex files exist.
         fns_aux = [
             fn for fn in glob("**/*.aux", recursive=True) if os.path.isfile(fn[:-4] + ".tex")
         ]
-    first = True
-    for fn_aux in fns_aux:
-        if first:
-            first = False
-        else:
+    for ifn, fn_aux in enumerate(fns_aux):
+        if ifn > 0:
             print()
-        process_aux(fn_aux, config, verbose)
+        return process_aux(fn_aux, verbose, config)
 
 
-def parse_args():
+def parse_args() -> tuple[list[str], bool, Config]:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser("bibsane")
     parser.add_argument("aux", nargs="*", help="The LaTeX aux file of your document")
     parser.add_argument("-q", "--quiet", default=False, action="store_true")
     parser.add_argument("-c", "--config", help="An optional configuration file")
     args = parser.parse_args()
     config = Config.from_file(args.config)
-    return args.aux, config, not args.quiet
+    return args.aux, not args.quiet, config
 
 
-def process_aux(fn_aux, config, verbose):
+def process_aux(fn_aux: str, verbose: bool, config: Config) -> int:
     """Main program."""
     # Load the aux file.
     if not fn_aux.endswith(".aux"):
         if verbose:
             print("Please, give an aux file as command-line argument, got:", fn_aux)
         return RETURN_CODE_BROKEN
-    else:
-        if verbose:
-            print("📂 Loading", fn_aux)
-        citations, fns_bib = parse_aux(fn_aux)
+    if verbose:
+        print("📂 Loading", fn_aux)
+    citations, fns_bib = parse_aux(fn_aux)
 
     if verbose:
         print(f"   Found {len(citations)} citations")
     citations = set(citations)
     if verbose:
         print(f"   Found {len(citations)} unique citations")
     if len(citations) == 0:
@@ -243,18 +241,19 @@
     if config.sort:
         if verbose:
             print("🔨 Sorting by Year + First author")
         entries = sort_entries(entries)
 
     # Overwrite if needed.
     fn_out = os.path.join(os.path.dirname(fn_aux), config.bibtex_out)
+    print(fn_out)
     return write_output(entries, fn_out, retcode, verbose)
 
 
-def parse_aux(fn_aux):
+def parse_aux(fn_aux: str) -> tuple[list[str], list[str]]:
     """Parse the relevant parts of a LaTeX aux file."""
     root = os.path.dirname(fn_aux)
     citations = []
     bibdata = []
     with open(fn_aux) as f:
         for line in f:
             parse_aux_line("citation", line, citations)
@@ -263,24 +262,24 @@
     for fn_bib in bibdata:
         if not fn_bib.endswith(".bib"):
             fn_bib += ".bib"
         fns_bib.append(os.path.join(root, fn_bib))
     return citations, fns_bib
 
 
-def parse_aux_line(prefix, line, words):
+def parse_aux_line(prefix: str, line: str, words: list[str]):
     """Parse a (simple) line from a LaTeX aux file."""
     if line.startswith(rf"\{prefix}{{"):
         assert line.endswith("}\n")
         assert line.count("{") == 1
         assert line.count("}") == 1
         words.extend(line[line.find("{") + 1 : -2].split(","))
 
 
-def collect_entries(fns_bib, config):
+def collect_entries(fns_bib: list[str], config: Config) -> tuple[list[dict[str, str]], bool]:
     """Collect entries from multiple BibTeX files."""
     # Collect stuff
     seen_ids = set()
     seen_dois = set()
     entries = []
     valid = True
     for fn_bib in fns_bib:
@@ -303,15 +302,17 @@
                     valid = False
                 seen_dois.add(entry["doi"])
             entries.append(entry)
             seen_ids.add(entry["ID"])
     return entries, valid
 
 
-def drop_check_citations(entries, citations, drop):
+def drop_check_citations(
+    entries: list[dict[str, str]], citations: Collection[str], drop
+) -> tuple[list[dict[str, str]], bool]:
     """Drop unused citations and complain about missing ones."""
     # Drop unused entries
     result = []
     for entry in entries:
         if entry["ID"] not in citations:
             print("     Dropping unused id:", entry["ID"])
             continue
@@ -327,32 +328,34 @@
         if citation not in defined:
             print("   💀 Missing reference:", citation)
             valid = False
 
     return result, valid
 
 
-def clean_entries(entries, citation_policies):
+def clean_entries(
+    entries: list[dict[str, str]], citation_policies: dict[str, dict[str, FieldPolicy]]
+) -> tuple[list[dict[str, str]], bool]:
     """Clean the irrelevant fields in each entry and complain about missing ones."""
     cleaned = []
     valid = True
     for old_entry in entries:
         eid = old_entry.pop("ID")
         etype = old_entry.pop("ENTRYTYPE")
         new_entry = {"ENTRYTYPE": etype, "ID": eid}
         if "bibsane" in old_entry:
             etype = old_entry.pop("bibsane")
             new_entry["bibsane"] = etype
-        policy = citation_policies.get(etype)
-        if policy is None:
+        entry_policy = citation_policies.get(etype)
+        if entry_policy is None:
             print(f"   🤔 {eid}: @{etype} is not configured")
             valid = False
             continue
         cleaned.append(new_entry)
-        for field, policy in policy.items():
+        for field, policy in entry_policy.items():
             if policy == FieldPolicy.MUST:
                 if field not in old_entry:
                     print(f"   🫥 {eid}: @{etype} missing field {field}")
                     valid = False
                 else:
                     new_entry[field] = old_entry.pop(field)
             else:
@@ -361,15 +364,15 @@
                     new_entry[field] = old_entry.pop(field)
         if len(old_entry) > 0:
             for field in old_entry:
                 print(f"   💨 {eid}: @{etype} discarding field {field}")
     return cleaned, valid
 
 
-def fix_bad_practices(entries):
+def fix_bad_practices(entries: list[dict[str, str]]) -> list[dict[str, str]]:
     """Fix unwarranted use of braces."""
     result = []
     for old_record in entries:
         # Strip all braces
         new_record = {
             key: value.replace("{", "").replace("}", "") for (key, value) in old_record.items()
         }
@@ -377,15 +380,16 @@
         for field in "author", "editor", "title":
             if field in old_record:
                 new_record[field] = old_record[field]
         result.append(new_record)
     return result
 
 
-def potential_mistakes(entries):
+def potential_mistakes(entries: list[dict[str, str]]) -> bool:
+    """Detect potential mistakes in the BibTeX entry keys."""
     id_case_map = {}
     for entry in entries:
         id_case_map.setdefault(entry["ID"].lower(), []).append(entry["ID"])
 
     mistakes = False
     for groups in id_case_map.values():
         if len(groups) > 1:
@@ -399,40 +403,40 @@
     "http://doi.org/",
     "http://dx.doi.org/",
     "https://dx.doi.org/",
     "doi:",
 ]
 
 
-def normalize_doi(entries):
+def normalize_doi(entries: list[dict[str, str]]) -> tuple[list[dict[str, str]], bool]:
     """Normalize the DOIs in the entries."""
     result = []
-    value = True
+    valid = True
     for entry in entries:
         doi = entry.get("doi")
         if doi is not None:
             doi = doi.lower()
             for proxy in DOI_PROXIES:
                 if doi.startswith(proxy):
                     doi = doi[len(proxy) :]
                     break
             if doi.count("/") == 0 or not doi.startswith("10."):
                 print("   🤕 invalid DOI:", doi)
-                value = False
+                valid = False
             entry = entry | {"doi": doi}
         result.append(entry)
-    return result, value
+    return result, valid
 
 
-def normalize_whitespace(entries):
+def normalize_whitespace(entries: list[dict[str, str]]) -> list[dict[str, str]]:
     """Normalize the whitespace inside the field values."""
     return [{key: re.sub(r"\s+", " ", value) for key, value in entry.items()} for entry in entries]
 
 
-def normalize_names(entries):
+def normalize_names(entries: list[dict[str, str]]) -> list[dict[str, str]]:
     """Normalize the author and editor names."""
     raise NotImplementedError("processing of names is not robust in BibtexParser 1.4.0")
     result = []
     for entry in entries:
         # Warning: bibtexparser modifies entries in place.
         # It does not hurt in this case, but it can otherwise give unexpected results.
         for field in "author", "editor":
@@ -443,26 +447,26 @@
                 names = [bibtexparser.latexenc.latex_to_unicode(name) for name in names]
                 names = [bibtexparser.latexenc.string_to_latex(name) for name in names]
                 entry[field] = " and ".join(names)
         result.append(entry)
     return result
 
 
-def fix_page_double_hyphen(entries):
+def fix_page_double_hyphen(entries: list[dict[str, str]]) -> list[dict[str, str]]:
     """Fix page ranges for which no double hyphen is used."""
     result = []
     for entry in entries:
         # Warning: bibtexparser modifies entries in place.
         # It does not hurt in this case, but it can otherwise give unexpected results.
         entry = bibtexparser.customization.page_double_hyphen(entry)
         result.append(entry)
     return result
 
 
-def abbreviate_journal_iso(entries, fn_cache):
+def abbreviate_journal_iso(entries: list[dict[str, str]], fn_cache: str) -> list[dict[str, str]]:
     """Replace journal names by their ISO abbreviation."""
 
     # Initialize cache
     if fn_cache is None or not os.path.isfile(fn_cache):
         cache = {}
     else:
         with open(fn_cache) as f:
@@ -484,23 +488,24 @@
     if fn_cache is not None:
         with open(fn_cache, "w") as f:
             json.dump(cache, f, indent=2)
             f.write("\n")
     return result
 
 
-def download_abbrev(journal):
+def download_abbrev(journal: str) -> str:
+    """Download the abbreviation of a full journal name."""
     print("   Downloading abbreviation for:", journal)
     journal_quote = urllib.parse.quote(journal)
     prefix = "https://abbreviso.toolforge.org/abbreviso/a/"
     with urllib.request.urlopen(prefix + journal_quote) as f:
         return f.read().decode()
 
 
-def merge_entries(entries, field):
+def merge_entries(entries: list[dict[str, str]], field: str) -> tuple[list[dict[str, str]], bool]:
     """Merge entries who have the same value for the given field. (case-insensitive)"""
     lookup = {}
     missing_key = []
     merge_conflict = False
     for entry in entries:
         identifier = entry.get(field)
         if identifier is None:
@@ -513,28 +518,29 @@
                     other[key] = value
                 elif other[key] != value:
                     print(f"   😭 Same {field}={identifier}, different {key}:", value, other[key])
                     merge_conflict = True
     return list(lookup.values()) + missing_key, merge_conflict
 
 
-def sort_entries(entries):
+def sort_entries(entries: list[dict[str, str]]) -> list[dict[str, str]]:
     """Sort the entries in convenient way: by year, then by author."""
 
     def keyfn(entry):
         # Make a fake entry to avoid in-place modification.
         entry = {"author": entry.get("author", "Aaaa Aaaa"), "year": entry.get("year", "0000")}
         first_author = bibtexparser.customization.author(entry)["author"][0].lower()
         key = entry["year"] + first_author
         return key
 
     return sorted(entries, key=keyfn)
 
 
-def write_output(entries, fn_out, retcode, verbose):
+def write_output(entries: list[dict[str, str]], fn_out: str, retcode: int, verbose: bool) -> int:
+    """Write out the fixed bibtex file, in case it has changed."""
     if retcode == RETURN_CODE_CHANGED:
         # Write out a single BibTeX database.
         db_out = bibtexparser.bibdatabase.BibDatabase()
         db_out.entries = entries
         writer = bibtexparser.bwriter.BibTexWriter()
         writer.order_entries_by = None
         with tempfile.TemporaryDirectory("bibsane") as dn_tmp:
@@ -553,15 +559,15 @@
                 print("😀 No changes to", fn_out)
     else:
         print(f"💥 Broken bibliography. Not writing: {fn_out}")
 
     return retcode
 
 
-def checksum(path):
+def checksum(path: str) -> bytes:
     """Compute the SHA256 checksum from the contents of a file."""
     with open(path, "rb") as f:
         return hashlib.sha256(f.read()).digest()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `BibSane-0.1.1/pyproject.toml` & `BibSane-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BibSane"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Sanitize BibTeX files without going insane"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.6"
```

