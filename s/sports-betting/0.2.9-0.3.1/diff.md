# Comparing `tmp/sports-betting-0.2.9.tar.gz` & `tmp/sports-betting-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports-betting-0.2.9.tar", last modified: Mon Apr  3 10:53:12 2023, max compression
+gzip compressed data, was "sports-betting-0.3.1.tar", last modified: Wed Apr 12 13:14:57 2023, max compression
```

## Comparing `sports-betting-0.2.9.tar` & `sports-betting-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2023-03-19 20:16:05.503737 sports-betting-0.2.9/LICENSE
--rw-r--r--   0        0        0     4623 2023-04-02 22:40:36.047660 sports-betting-0.2.9/README.md
--rw-r--r--   0        0        0     5238 2023-04-02 10:08:54.448761 sports-betting-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1000 2023-03-28 19:30:08.219738 sports-betting-0.2.9/src/sportsbet/__init__.py
--rw-r--r--   0        0        0      131 2023-03-29 08:50:29.899413 sports-betting-0.2.9/src/sportsbet/__main__.py
--rw-r--r--   0        0        0     9728 2023-04-02 16:01:26.734826 sports-betting-0.2.9/src/sportsbet/cli.py
--rw-r--r--   0        0        0      262 2023-04-03 10:26:53.384350 sports-betting-0.2.9/src/sportsbet/datasets/__init__.py
--rw-r--r--   0        0        0    18241 2023-04-03 10:41:34.502247 sports-betting-0.2.9/src/sportsbet/datasets/_base.py
--rw-r--r--   0        0        0    15335 2023-04-03 10:46:09.686630 sports-betting-0.2.9/src/sportsbet/datasets/_dummy.py
--rw-r--r--   0        0        0        0 2022-02-01 22:10:48.200518 sports-betting-0.2.9/src/sportsbet/datasets/_soccer/__init__.py
--rw-r--r--   0        0        0    21380 2023-04-03 10:32:12.102023 sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_data.py
--rw-r--r--   0        0        0    28656 2023-04-03 09:50:40.497677 sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_fd.py
--rw-r--r--   0        0        0     5102 2023-04-03 09:50:49.333755 sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_fte.py
--rw-r--r--   0        0        0     2595 2023-03-27 20:39:08.417256 sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_utils.py
--rw-r--r--   0        0        0      200 2023-04-03 10:27:16.832023 sports-betting-0.2.9/src/sportsbet/evaluation/__init__.py
--rw-r--r--   0        0        0    10959 2023-04-02 21:31:02.653237 sports-betting-0.2.9/src/sportsbet/evaluation/_base.py
--rw-r--r--   0        0        0     5529 2023-04-03 09:48:05.265783 sports-betting-0.2.9/src/sportsbet/evaluation/_classifier.py
--rw-r--r--   0        0        0        0 2023-03-16 12:43:26.515457 sports-betting-0.2.9/src/sportsbet/py.typed
--rw-r--r--   0        0        0      162 2023-03-16 12:43:17.857452 sports-betting-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0      310 2023-03-25 10:59:47.785429 sports-betting-0.2.9/tests/conftest.py
--rw-r--r--   0        0        0       28 2023-03-24 22:39:56.568853 sports-betting-0.2.9/tests/datasets/__init__.py
--rw-r--r--   0        0        0    18705 2023-03-28 15:26:00.605472 sports-betting-0.2.9/tests/datasets/test_dummy.py
--rw-r--r--   0        0        0       30 2023-03-24 22:40:31.109809 sports-betting-0.2.9/tests/evaluation/__init__.py
--rw-r--r--   0        0        0     7350 2023-04-02 15:06:18.413287 sports-betting-0.2.9/tests/evaluation/test_classifier.py
--rw-r--r--   0        0        0     7311 2023-04-02 21:31:27.333484 sports-betting-0.2.9/tests/test_cli.py
--rw-r--r--   0        0        0     5845 1970-01-01 00:00:00.000000 sports-betting-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-12 10:43:30.277668 sports-betting-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4879 2023-04-12 10:43:30.473663 sports-betting-0.3.1/README.md
+-rw-r--r--   0        0        0     5343 2023-04-12 10:43:30.475057 sports-betting-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1029 2023-04-12 10:43:30.475247 sports-betting-0.3.1/src/sportsbet/__init__.py
+-rw-r--r--   0        0        0      131 2023-03-29 08:50:29.899413 sports-betting-0.3.1/src/sportsbet/__main__.py
+-rw-r--r--   0        0        0     9737 2023-04-11 16:49:24.909001 sports-betting-0.3.1/src/sportsbet/cli.py
+-rw-r--r--   0        0        0      298 2023-04-11 16:49:24.909882 sports-betting-0.3.1/src/sportsbet/datasets/__init__.py
+-rw-r--r--   0        0        0    18249 2023-04-11 16:49:24.910843 sports-betting-0.3.1/src/sportsbet/datasets/_base.py
+-rw-r--r--   0        0        0    15554 2023-04-03 15:00:25.774832 sports-betting-0.3.1/src/sportsbet/datasets/_dummy.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:17:21.696007 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/__init__.py
+-rw-r--r--   0        0        0    21586 2023-04-03 15:00:25.775440 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_data.py
+-rw-r--r--   0        0        0    28790 2023-04-03 15:00:25.775835 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fd.py
+-rw-r--r--   0        0        0     5122 2023-04-03 15:00:25.776337 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fte.py
+-rw-r--r--   0        0        0     2595 2023-03-27 20:39:08.417256 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_utils.py
+-rw-r--r--   0        0        0      200 2023-04-03 10:27:16.832023 sports-betting-0.3.1/src/sportsbet/evaluation/__init__.py
+-rw-r--r--   0        0        0    10944 2023-04-11 16:49:24.911729 sports-betting-0.3.1/src/sportsbet/evaluation/_base.py
+-rw-r--r--   0        0        0     5529 2023-04-03 09:48:05.265783 sports-betting-0.3.1/src/sportsbet/evaluation/_classifier.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:43:30.443650 sports-betting-0.3.1/src/sportsbet/py.typed
+-rw-r--r--   0        0        0      162 2023-04-12 10:43:30.222813 sports-betting-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-12 10:43:30.475416 sports-betting-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0       28 2023-03-24 22:39:56.568853 sports-betting-0.3.1/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    18705 2023-03-28 15:26:00.605472 sports-betting-0.3.1/tests/datasets/test_dummy.py
+-rw-r--r--   0        0        0       30 2023-03-24 22:40:31.109809 sports-betting-0.3.1/tests/evaluation/__init__.py
+-rw-r--r--   0        0        0     7350 2023-04-02 15:06:18.413287 sports-betting-0.3.1/tests/evaluation/test_classifier.py
+-rw-r--r--   0        0        0     7311 2023-04-02 21:31:27.333484 sports-betting-0.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 sports-betting-0.3.1/PKG-INFO
```

### Comparing `sports-betting-0.2.9/LICENSE` & `sports-betting-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sports-betting-0.2.9/README.md` & `sports-betting-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [scikit-learn]: <http://scikit-learn.org/stable/>
-[imbalanced-learn]: <http://imbalanced-learn.org/stable/>
 [black badge]: <https://img.shields.io/badge/%20style-black-000000.svg>
 [black]: <https://github.com/psf/black>
 [docformatter badge]: <https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg>
 [docformatter]: <https://github.com/PyCQA/docformatter>
 [ruff badge]: <https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json>
 [ruff]: <https://github.com/charliermarsh/ruff>
 [mypy badge]: <http://www.mypy-lang.org/static/mypy_badge.svg>
@@ -38,20 +37,29 @@
 Python sports betting toolbox.
 
 The `sports-betting` package is a collection of tools that makes it easy to create machine learning models for sports betting and
 evaluate their performance. It is compatible with [scikit-learn].
 
 ## Installation
 
-`sports-betting` is currently available on the PyPi's repository, and you can install it via `pip`:
+For user installation, `sports-betting` is currently available on the PyPi's repository, and you can install it via `pip`:
 
 ```bash
 pip install sports-betting
 ```
 
+Development installation requires to clone the repository and then use [PDM](https://github.com/pdm-project/pdm) to install the
+project as well as the main and development dependencies:
+
+```bash
+git clone https://github.com/georgedouzas/sports-betting.git
+cd sports-betting
+pdm install
+```
+
 ## Usage
 
 ### API
 
 The `sports-betting` package makes it easy to download sports betting data:
 
 ```python
```

### Comparing `sports-betting-0.2.9/pyproject.toml` & `sports-betting-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,42 +8,43 @@
 name = "sports-betting"
 description = "Python sports betting toolbox."
 authors = [
     { name = "Georgios Douzas", email = "gdouzas@icloud.com" },
 ]
 license = "MIT"
 readme = "README.md"
-requires-python = ">=3.10, <3.11"
+requires-python = ">=3.9, <3.11"
 keywords = []
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "nptyping>=2.5.0",
-    "pandas>=1.0.0",
+    "pandas>=1.0.0, <=1.5.3",
     "scikit-learn>=1.0.0",
     "cloudpickle>=2.0.0",
     "beautifulsoup4>=4.0.0",
     "vectorbt>=0.24.5",
     "QuantStats>=0.0.47",
     "typing-extensions>=4.5.0",
     "click>=8.1.3",
     "rich>=13.3.3",
 ]
-version = "0.2.9"
+version = "0.3.1"
 
 [project.urls]
 Homepage = "https://georgedouzas.github.io/sports-betting"
 Documentation = "https://georgedouzas.github.io/sports-betting"
 Changelog = "https://georgedouzas.github.io/sports-betting/changelog"
 Repository = "https://github/georgedouzas/sports-betting"
 Issues = "https://github/georgedouzas/sports-betting/issues"
@@ -66,15 +67,15 @@
 formatting = "nox --error-on-external-run -R -s formatting -- {args:all}"
 checks = "nox --error-on-external-run -R -s checks -- {args:all}"
 tests = "nox --error-on-external-run -R -s tests"
 changelog = "nox --error-on-external-run -R -s changelog"
 release = "nox --error-on-external-run -R -s release -- {args}"
 
 [tool.pdm.scripts.clean]
-shell = "rm -rf .mypy_cache .pytest_cache tests/.pytest_cache build dist htmlcov pip-wheel-metadata site __pycache__ && find . -type d -name __pycache__ | xargs rm -rf && find . -name '*.rej'  -delete && find . -name '.coverage*'  -delete"
+shell = "rm -rf .mypy_cache .pytest_cache tests/.pytest_cache build dist htmlcov pip-wheel-metadata site __pycache__ docs/generated .nox .ruff_cache pdm.lock && find . -type d -name __pycache__ | xargs rm -rf && find . -name '*.rej'  -delete && find . -name '.coverage*'  -delete"
 
 [tool.pdm.dev-dependencies]
 maintenance = [
     "nox>=2022.8.7",
 ]
 docs = [
     "mkdocs>=1.3",
@@ -224,20 +225,21 @@
     "RUF",
 ]
 extend-exclude = [
     "docs/generated",
 ]
 force-exclude = true
 line-length = 120
-target-version = "py310"
+target-version = "py39"
 
 [tool.ruff.per-file-ignores]
 "docs/examples/*" = [
     "ANN",
     "D",
+    "B018",
 ]
 "docs/generated/*" = [
     "ANN",
     "D",
 ]
 "test_*" = [
     "ANN",
```

### Comparing `sports-betting-0.2.9/src/sportsbet/__init__.py` & `sports-betting-0.3.1/src/sportsbet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 - [`datasets`][sportsbet.datasets]: Provides the classes to extract sports betting datasets.
 - [`evaluation`][sportsbet.evaluation]: Provides the classes to create and evaluate sports betting predictive models.
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
-from typing import Any
+from typing import Any, Union
 
 import numpy as np
 import pandas as pd
 from nptyping import Bool, Float, NDArray, Shape
 
 Param = dict[str, Any]
-ParamGrid = dict[str, list[Any]] | list[dict[str, list[Any]]]
-TrainingData = tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame | None]
-FixturesData = tuple[pd.DataFrame, None, pd.DataFrame | None]
+ParamGrid = Union[dict[str, list[Any]], list[dict[str, list[Any]]]]
+TrainingData = tuple[pd.DataFrame, pd.DataFrame, Union[pd.DataFrame, None]]
+FixturesData = tuple[pd.DataFrame, None, Union[pd.DataFrame, None]]
 Data = NDArray[Shape['*, *'], Float]
 BoolData = NDArray[Shape['*, *'], Bool]
-Schema = list[tuple[str, type[int] | type[float] | type[object] | type[np.datetime64]]]
+Schema = list[tuple[str, Union[type[int], type[float], type[object], type[np.datetime64]]]]
 Outputs = list[tuple[str, Callable[..., pd.DataFrame]]]
```

### Comparing `sports-betting-0.2.9/src/sportsbet/cli.py` & `sports-betting-0.3.1/src/sportsbet/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,32 +87,34 @@
 
 
 def print_console(dfs: list[pd.DataFrame], titles: list[str]) -> None:
     """Print to the console."""
     pd.set_option('display.max_rows', None)
     console = Console()
     with console.pager(styles=True):
-        for df, title in zip(dfs, titles, strict=True):
+        for df, title in zip(dfs, titles):
             formatted_title = Panel.fit(f'[bold green]{title}')
             console.print(formatted_title)
             console.print(df)
 
 
 @click.group()
 def main() -> None:
     """CLI for sports-betting.
 
     This command is executed when you type `sportsbet` or `python -m
     sportsbet`.
     """
+    return
 
 
 @main.group()
 def dataloader() -> None:
     """Use or create a dataloader."""
+    return
 
 
 @dataloader.command()
 def names() -> None:
     """List the sports names that can be selected."""
     sports = [
         (name.lower().replace('dataloader', ''), 'Yes')
```

### Comparing `sports-betting-0.2.9/src/sportsbet/datasets/_base.py` & `sports-betting-0.3.1/src/sportsbet/datasets/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     indices = names_combinations_similarity.groupby(_cols('_x')).iloc[0].idxmax().to_numpy()
     names_matching = names_combinations.take(indices)
 
     # Teams matching
     matching1 = names_matching.loc[:, ['home_team_x', 'home_team_y']].drop_duplicates()
     matching2 = names_matching.loc[:, ['away_team_x', 'away_team_y']].drop_duplicates()
     matching1.columns = matching2.columns = cols = ['team1', 'team2']
-    matching = matching1.append(matching2)
+    matching = pd.concat([matching1, matching2])
     similarity = matching.apply(lambda row: SequenceMatcher(None, row.team1, row.team2).ratio(), axis=1)
     names_combinations_similarity = pd.concat([matching, similarity], axis=1).reset_index(drop=True)
     indices = names_combinations_similarity.groupby('team1').iloc[0].idxmax()
     names_mapping = names_combinations_similarity.take(indices)[cols].reset_index(drop=True)
 
     return names_mapping
 
@@ -339,15 +339,14 @@
 
         Returns:
             (X, None, O):
                 Each of the components represent the fixtures input data `X`, the
                 multi-output targets `Y` equal to `None` and the
                 corresponding odds `O`, respectively.
         """
-
         # Extract fixtures data
         if not (
             hasattr(self, 'input_cols_')
             and hasattr(self, 'output_cols_')
             and hasattr(self, 'odds_cols_')
             and hasattr(self, 'target_cols_')
         ):
@@ -359,15 +358,15 @@
         # Extract fixtures data
         data = data[data['fixtures']].drop(columns=['fixtures'])
 
         # Convert data types
         data = self._convert_data_types(data)
 
         # Remove past data
-        data = data[data.index >= pd.to_datetime('today')]
+        data = data.loc[data.index >= pd.to_datetime('today')]
 
         # Extract odds
         O_fix = data[self.odds_cols_].reset_index(drop=True) if self.odds_type_ is not None else None
 
         return data[self.input_cols_], None, O_fix
 
     def save(self: Self, path: str) -> Self:
@@ -412,15 +411,14 @@
         It can be used to get the allowed odds types of the dataloader's method
         `extract_train_data`.
 
         Returns:
             odds_types:
                 A list of available odds types.
         """
-
         # Check param grid
         self._check_param_grid()
 
         # Validate the data
         data = self._validate_data()
 
         # Extract train data
```

### Comparing `sports-betting-0.2.9/src/sportsbet/datasets/_dummy.py` & `sports-betting-0.3.1/src/sportsbet/datasets/_dummy.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import pandas as pd
 import pytz
 from sklearn.model_selection import ParameterGrid
 from typing_extensions import Self
 
-from .. import FixturesData, TrainingData
+from .. import FixturesData, ParamGrid, TrainingData
 from ._base import _BaseDataLoader
 
 OVER_UNDER = 2.5
 
 
 class DummySoccerDataLoader(_BaseDataLoader):
     """Dataloader for soccer dummy data.
@@ -37,33 +37,33 @@
             The default value `None` corresponds to all parameters.
 
     Attributes:
         param_grid_ (ParameterGrid):
             The checked value of parameters grid. It includes all possible parameters if
             `param_grid` is `None`.
 
-        dropped_na_cols_:
+        dropped_na_cols_ (pd.Index):
             The columns with missing values that are dropped.
 
-        drop_na_thres_:
+        drop_na_thres_(float):
             The checked value of `drop_na_thres`.
 
-        odds_type_:
+        odds_type_ (str | None):
             The checked value of `odds_type`.
 
-        input_cols_:
+        input_cols_ (pd.Index):
             The columns of `X_train` and `X_fix`.
 
-        output_cols_:
+        output_cols_ (pd.Index):
             The columns of `Y_train` and `Y_fix`.
 
-        odds_cols_:
+        odds_cols_ (pd.Index):
             The columns of `O_train` and `O_fix`.
 
-        target_cols_:
+        target_cols_ (pd.Index):
             The columns used for the extraction of output and odds columns.
 
     Examples:
         >>> from sportsbet.datasets import DummySoccerDataLoader
         >>> import pandas as pd
         >>> # Get all available parameters to select the training data
         >>> DummySoccerDataLoader.get_all_params()
@@ -100,24 +100,24 @@
         >>> # Fixtures data have always no output
         >>> Y_fix is None
         True
     """
 
     DATE = datetime.now(tz=pytz.utc) + timedelta(2)
     SCHEMA = [
-        ('division', int),
+        ('division', np.int64),
         ('league', object),
         ('date', np.datetime64),
-        ('year', int),
+        ('year', np.int64),
         ('home_team', object),
         ('away_team', object),
         ('home_soccer_index', float),
         ('away_soccer_index', float),
-        ('target__home_team__full_time_goals', int),
-        ('target__away_team__full_time_goals', int),
+        ('target__home_team__full_time_goals', np.int64),
+        ('target__away_team__full_time_goals', np.int64),
         ('odds__interwetten__home_win__full_time_goals', float),
         ('odds__interwetten__draw__full_time_goals', float),
         ('odds__interwetten__away_win__full_time_goals', float),
         ('odds__williamhill__home_win__full_time_goals', float),
         ('odds__williamhill__draw__full_time_goals', float),
         ('odds__williamhill__away_win__full_time_goals', float),
         (f'odds__pinnacle__over_{OVER_UNDER}__full_time_goals', float),
@@ -369,14 +369,17 @@
                 True,
                 False,
                 False,
             ],
         },
     )
 
+    def __init__(self: Self, param_grid: ParamGrid | None = None) -> None:
+        super().__init__(param_grid)
+
     @classmethod
     def _get_full_param_grid(cls: type[DummySoccerDataLoader]) -> ParameterGrid:
         return ParameterGrid(
             [
                 {'league': ['Greece'], 'division': [1], 'year': [2017, 2019]},
                 {'league': ['Spain'], 'division': [1], 'year': [1997]},
                 {'league': ['Spain'], 'division': [2], 'year': [1999]},
```

### Comparing `sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_data.py` & `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from functools import lru_cache
 
 import pandas as pd
 from sklearn.model_selection import ParameterGrid
 from typing_extensions import Self
 
-from ... import FixturesData, TrainingData
+from ... import FixturesData, ParamGrid, TrainingData
 from .._base import _BaseDataLoader
 from ._fd import _FDSoccerDataLoader
 from ._fte import _FTESoccerDataLoader
 from ._utils import OUTPUTS
 
 NAMES_MAPPING = {
     'SK Austria Klagenfurt': 'A. Klagenfurt',
@@ -374,27 +374,34 @@
             `param_grid` parameter of the scikit-learn's ParameterGrid class.
             The default value `None` corresponds to all parameters.
 
     Attributes:
         param_grid_ (ParameterGrid):
             The checked value of parameters grid. It includes all possible parameters if
             `param_grid` is `None`.
-        dropped_na_cols_:
+
+        dropped_na_cols_ (pd.Index):
             The columns with missing values that are dropped.
-        drop_na_thres_:
+
+        drop_na_thres_(float):
             The checked value of `drop_na_thres`.
-        odds_type_:
+
+        odds_type_ (str | None):
             The checked value of `odds_type`.
-        input_cols_:
+
+        input_cols_ (pd.Index):
             The columns of `X_train` and `X_fix`.
-        output_cols_:
+
+        output_cols_ (pd.Index):
             The columns of `Y_train` and `Y_fix`.
-        odds_cols_:
+
+        odds_cols_ (pd.Index):
             The columns of `O_train` and `O_fix`.
-        target_cols_:
+
+        target_cols_ (pd.Index):
             The columns used for the extraction of output and odds columns.
 
     Examples:
         >>> from sportsbet.datasets import SoccerDataLoader
         >>> import pandas as pd
         >>> # Get all available parameters to select the training data
         >>> SoccerDataLoader.get_all_params()
@@ -424,14 +431,17 @@
     SCHEMA = (
         _FDSoccerDataLoader.SCHEMA
         + [col for col in _FTESoccerDataLoader.SCHEMA if col not in _FDSoccerDataLoader.SCHEMA]
         + [('data_source', object)]
     )
     OUTPUTS = OUTPUTS
 
+    def __init__(self: Self, param_grid: ParamGrid | None = None) -> None:
+        super().__init__(param_grid)
+
     @classmethod
     @lru_cache
     def _get_full_param_grid(cls: type[SoccerDataLoader]) -> ParameterGrid:
         fd_full_param_grid_df = pd.DataFrame(_FDSoccerDataLoader.get_all_params()).assign(data_source='footballdata')
         fte_full_param_grid_df = pd.DataFrame(_FTESoccerDataLoader.get_all_params()).assign(
             data_source='fivethirtyeight',
         )
```

### Comparing `sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_fd.py` & `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fd.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,15 +274,15 @@
     league = base_url.replace('.php', '')
     if base_url[0].islower():
         league = league[:-1].capitalize()
     return league
 
 
 def _extract_csv_urls(base_url: str) -> set[str]:
-    html = urlopen('/'.join([URL, base_url]))
+    html = urlopen('/'.join([URL, base_url]))  # noqa: S310
     bsObj = BeautifulSoup(html.read(), features='html.parser')
     return {el.get('href') for el in bsObj.find_all('a') if el.get('href').endswith('csv')}
 
 
 def _param_grid_to_csv_urls(param_grid: ParameterGrid) -> list[tuple[Param, str]]:
     urls = []
     for params in param_grid:
@@ -306,16 +306,16 @@
 
     It downloads historical and fixtures data from
     [Football-Data.co.uk](https://www.football-data.co.uk/data.php).
     """
 
     SCHEMA = [
         ('league', object),
-        ('division', int),
-        ('year', int),
+        ('division', np.int64),
+        ('year', np.int64),
         ('home_team', object),
         ('away_team', object),
         ('date', np.datetime64),
         ('odds__bet365__home_win__full_time_goals', float),
         ('odds__bet365__draw__full_time_goals', float),
         ('odds__bet365__away_win__full_time_goals', float),
         ('odds__bet365__over_2.5__full_time_goals', float),
@@ -453,36 +453,36 @@
             float,
         ),
         ('odds__market_average__size_of_handicap_home_team__full_time_goals', object),
         (
             'odds__market_average_closing__size_of_asian_handicap_home_team__full_time_goals',
             object,
         ),
-        ('target__home_team__full_time_goals', int),
-        ('target__away_team__full_time_goals', int),
-        ('target__home_team__half_time_goals', int),
-        ('target__away_team__half_time_goals', int),
-        ('target__home_team__shots', int),
-        ('target__away_team__shots', int),
-        ('target__home_team__shots_on_target', int),
-        ('target__away_team__shots_on_target', int),
-        ('target__home_team__hit_woodork', int),
-        ('target__away_team__hit_woodork', int),
-        ('target__home_team__corners', int),
-        ('target__away_team__corners', int),
-        ('target__home_team__fouls_committed', int),
-        ('target__away_team__fouls_committed', int),
-        ('target__home_team__free_kicks_conceded', int),
-        ('target__away_team__free_kicks_conceded', int),
-        ('target__home_team__offsides', int),
-        ('target__away_team__offsides', int),
-        ('target__home_team__yellow_cards', int),
-        ('target__away_team__yellow_cards', int),
-        ('target__home_team__red_cards', int),
-        ('target__away_team__red_cards', int),
+        ('target__home_team__full_time_goals', np.int64),
+        ('target__away_team__full_time_goals', np.int64),
+        ('target__home_team__half_time_goals', np.int64),
+        ('target__away_team__half_time_goals', np.int64),
+        ('target__home_team__shots', np.int64),
+        ('target__away_team__shots', np.int64),
+        ('target__home_team__shots_on_target', np.int64),
+        ('target__away_team__shots_on_target', np.int64),
+        ('target__home_team__hit_woodork', np.int64),
+        ('target__away_team__hit_woodork', np.int64),
+        ('target__home_team__corners', np.int64),
+        ('target__away_team__corners', np.int64),
+        ('target__home_team__fouls_committed', np.int64),
+        ('target__away_team__fouls_committed', np.int64),
+        ('target__home_team__free_kicks_conceded', np.int64),
+        ('target__away_team__free_kicks_conceded', np.int64),
+        ('target__home_team__offsides', np.int64),
+        ('target__away_team__offsides', np.int64),
+        ('target__home_team__yellow_cards', np.int64),
+        ('target__away_team__yellow_cards', np.int64),
+        ('target__home_team__red_cards', np.int64),
+        ('target__away_team__red_cards', np.int64),
         ('target__home_team__bookings_points', float),
         ('target__away_team__bookings_points', float),
     ]
     OUTPUTS = OUTPUTS
 
     @classmethod
     @lru_cache
```

### Comparing `sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_fte.py` & `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fte.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,32 +103,32 @@
     """Dataloader for FiveThirtyEight soccer data.
 
     It downloads historical and fixtures data from
     [FiveThirtyEight](https://github.com/fivethirtyeight/data/tree/master/soccer-spi).
     """
 
     SCHEMA = [
-        ('year', int),
-        ('division', int),
+        ('year', np.int64),
+        ('division', np.int64),
         ('match_quality', float),
         ('league', object),
         ('home_team', object),
         ('away_team', object),
         ('date', np.datetime64),
         ('home_team_soccer_power_index', float),
         ('away_team_soccer_power_index', float),
         ('home_team_probability_win', float),
         ('away_team_probability_win', float),
         ('probability_draw', float),
         ('home_team_projected_score', float),
         ('away_team_projected_score', float),
         ('home_team_match_importance', float),
         ('away_team_match_importance', float),
-        ('target__home_team__full_time_goals', int),
-        ('target__away_team__full_time_goals', int),
+        ('target__home_team__full_time_goals', np.int64),
+        ('target__away_team__full_time_goals', np.int64),
         ('target__home_team__full_time_shot_expected_goals', float),
         ('target__away_team__full_time_shot_expected_goals', float),
         ('target__home_team__full_time_non_shot_expected_goals', float),
         ('target__away_team__full_time_non_shot_expected_goals', float),
         ('target__home_team__full_time_adjusted_goals', float),
         ('target__away_team__full_time_adjusted_goals', float),
     ]
```

### Comparing `sports-betting-0.2.9/src/sportsbet/datasets/_soccer/_utils.py` & `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_utils.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.2.9/src/sportsbet/evaluation/_base.py` & `sports-betting-0.3.1/src/sportsbet/evaluation/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     Warning: This class should not be used directly. Use the derive classes
     instead.
     """
 
     def _check_backtest_params(self: Self, tscv: TimeSeriesSplit | None, init_cash: float | None) -> Self:
         """Check backtest parameters."""
-
         # Check cross validator
         if tscv is None:
             tscv = TimeSeriesSplit()
         if not isinstance(tscv, TimeSeriesSplit):
             error_msg = 'Parameter `tscv` should be a TimeSeriesSplit cross-validator object.'
             raise TypeError(error_msg)
         self.tscv_ = tscv
@@ -61,15 +60,14 @@
     def _extract_portfolio(self: Self, prices: pd.DataFrame, orders: pd.DataFrame) -> Portfolio:
         """Extract portfolio."""
         return Portfolio.from_orders(prices, orders, freq='0.5D', cash_sharing=True, init_cash=self.init_cash_)
 
     @staticmethod
     def _extract_stats(portfolio: Portfolio, training_start: int, training_end: int) -> pd.DataFrame:
         """Extract statistics from portfolio."""
-
         portfolio_stats = portfolio.stats()
         if portfolio_stats is None:
             return pd.DataFrame([])
 
         # Reshape data
         stats = pd.DataFrame(portfolio_stats.to_numpy().reshape(1, -1), columns=portfolio_stats.index)
 
@@ -303,15 +301,15 @@
             portfolio = self._extract_portfolio(prices, orders)
             results.append(
                 (
                     self._extract_stats(portfolio, X.index[train_ind[0]], X.index[train_ind[-1]]),
                     portfolio.plot_value,
                 ),
             )
-        self.backtest_results_, plot_value_funcs = zip(*results, strict=True)
+        self.backtest_results_, plot_value_funcs = zip(*results)
         self.backtest_results_ = pd.concat(self.backtest_results_, ignore_index=True)
         self.backtest_plot_value_ = lambda ind: plot_value_funcs[ind]()
 
         if refit:
             self.fit(X, Y)
 
         return self
```

### Comparing `sports-betting-0.2.9/src/sportsbet/evaluation/_classifier.py` & `sports-betting-0.3.1/src/sportsbet/evaluation/_classifier.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.2.9/tests/datasets/test_dummy.py` & `sports-betting-0.3.1/tests/datasets/test_dummy.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.2.9/tests/evaluation/test_classifier.py` & `sports-betting-0.3.1/tests/evaluation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.2.9/tests/test_cli.py` & `sports-betting-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.2.9/PKG-INFO` & `sports-betting-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sports-betting
-Version: 0.2.9
+Version: 0.3.1
 Summary: Python sports betting toolbox.
 License: MIT
 Author-email: Georgios Douzas <gdouzas@icloud.com>
-Requires-Python: >=3.10, <3.11
+Requires-Python: >=3.9, <3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Changelog, https://georgedouzas.github.io/sports-betting/changelog
 Project-URL: Discussions, https://github/georgedouzas/sports-betting/discussions
 Project-URL: Documentation, https://georgedouzas.github.io/sports-betting
@@ -22,15 +23,14 @@
 Project-URL: Gitter, https://gitter.im/sports-betting/community
 Project-URL: Homepage, https://georgedouzas.github.io/sports-betting
 Project-URL: Issues, https://github/georgedouzas/sports-betting/issues
 Project-URL: Repository, https://github/georgedouzas/sports-betting
 Description-Content-Type: text/markdown
 
 [scikit-learn]: <http://scikit-learn.org/stable/>
-[imbalanced-learn]: <http://imbalanced-learn.org/stable/>
 [black badge]: <https://img.shields.io/badge/%20style-black-000000.svg>
 [black]: <https://github.com/psf/black>
 [docformatter badge]: <https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg>
 [docformatter]: <https://github.com/PyCQA/docformatter>
 [ruff badge]: <https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json>
 [ruff]: <https://github.com/charliermarsh/ruff>
 [mypy badge]: <http://www.mypy-lang.org/static/mypy_badge.svg>
@@ -65,20 +65,29 @@
 Python sports betting toolbox.
 
 The `sports-betting` package is a collection of tools that makes it easy to create machine learning models for sports betting and
 evaluate their performance. It is compatible with [scikit-learn].
 
 ## Installation
 
-`sports-betting` is currently available on the PyPi's repository, and you can install it via `pip`:
+For user installation, `sports-betting` is currently available on the PyPi's repository, and you can install it via `pip`:
 
 ```bash
 pip install sports-betting
 ```
 
+Development installation requires to clone the repository and then use [PDM](https://github.com/pdm-project/pdm) to install the
+project as well as the main and development dependencies:
+
+```bash
+git clone https://github.com/georgedouzas/sports-betting.git
+cd sports-betting
+pdm install
+```
+
 ## Usage
 
 ### API
 
 The `sports-betting` package makes it easy to download sports betting data:
 
 ```python
```

