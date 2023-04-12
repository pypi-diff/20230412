# Comparing `tmp/multi_date_picker-0.0.1.tar.gz` & `tmp/multi_date_picker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_date_picker-0.0.1.tar", last modified: Wed Apr 12 15:36:38 2023, max compression
+gzip compressed data, was "multi_date_picker-0.0.2.tar", last modified: Wed Apr 12 20:03:30 2023, max compression
```

## Comparing `multi_date_picker-0.0.1.tar` & `multi_date_picker-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 15:36:38.199424 multi_date_picker-0.0.1/
--rw-r--r--   0 larky      (501) staff       (20)        0 2023-04-12 13:15:35.000000 multi_date_picker-0.0.1/LICENSE
--rw-r--r--   0 larky      (501) staff       (20)      403 2023-04-12 13:15:35.000000 multi_date_picker-0.0.1/MANIFEST.in
--rw-r--r--   0 larky      (501) staff       (20)      196 2023-04-12 15:36:38.199303 multi_date_picker-0.0.1/PKG-INFO
--rw-r--r--   0 larky      (501) staff       (20)     3676 2023-04-12 13:15:35.000000 multi_date_picker-0.0.1/README.md
-drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 15:36:38.198347 multi_date_picker-0.0.1/multi_date_picker/
--rw-r--r--   0 larky      (501) staff       (20)     7577 2023-04-12 15:28:16.000000 multi_date_picker-0.0.1/multi_date_picker/MultiDatePicker.py
--rw-r--r--   0 larky      (501) staff       (20)     2507 2023-04-12 13:15:35.000000 multi_date_picker-0.0.1/multi_date_picker/__init__.py
--rw-r--r--   0 larky      (501) staff       (20)       81 2023-04-12 15:28:16.000000 multi_date_picker-0.0.1/multi_date_picker/_imports_.py
--rw-r--r--   0 larky      (501) staff       (20)    12569 2023-04-12 15:28:16.000000 multi_date_picker-0.0.1/multi_date_picker/metadata.json
--rw-r--r--   0 larky      (501) staff       (20)    76300 2023-04-12 15:28:16.000000 multi_date_picker-0.0.1/multi_date_picker/multi_date_picker.min.js
--rw-r--r--   0 larky      (501) staff       (20)      101 2023-04-12 15:28:16.000000 multi_date_picker-0.0.1/multi_date_picker/multi_date_picker.min.js.map
--rw-r--r--   0 larky      (501) staff       (20)     1822 2023-04-12 15:28:16.000000 multi_date_picker-0.0.1/multi_date_picker/package-info.json
-drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 15:36:38.198927 multi_date_picker-0.0.1/multi_date_picker.egg-info/
--rw-r--r--   0 larky      (501) staff       (20)      196 2023-04-12 15:36:38.000000 multi_date_picker-0.0.1/multi_date_picker.egg-info/PKG-INFO
--rw-r--r--   0 larky      (501) staff       (20)      491 2023-04-12 15:36:38.000000 multi_date_picker-0.0.1/multi_date_picker.egg-info/SOURCES.txt
--rw-r--r--   0 larky      (501) staff       (20)        1 2023-04-12 15:36:38.000000 multi_date_picker-0.0.1/multi_date_picker.egg-info/dependency_links.txt
--rw-r--r--   0 larky      (501) staff       (20)       18 2023-04-12 15:36:38.000000 multi_date_picker-0.0.1/multi_date_picker.egg-info/top_level.txt
--rw-r--r--   0 larky      (501) staff       (20)     1822 2023-04-12 13:21:50.000000 multi_date_picker-0.0.1/package.json
--rw-r--r--   0 larky      (501) staff       (20)       38 2023-04-12 15:36:38.199455 multi_date_picker-0.0.1/setup.cfg
--rw-r--r--   0 larky      (501) staff       (20)      510 2023-04-12 13:15:35.000000 multi_date_picker-0.0.1/setup.py
-drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 15:36:38.199042 multi_date_picker-0.0.1/tests/
--rw-r--r--   0 larky      (501) staff       (20)      920 2023-04-12 13:15:35.000000 multi_date_picker-0.0.1/tests/test_usage.py
+drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 20:03:30.453245 multi_date_picker-0.0.2/
+-rw-r--r--   0 larky      (501) staff       (20)        0 2023-04-12 13:15:35.000000 multi_date_picker-0.0.2/LICENSE
+-rw-r--r--   0 larky      (501) staff       (20)      403 2023-04-12 13:15:35.000000 multi_date_picker-0.0.2/MANIFEST.in
+-rw-r--r--   0 larky      (501) staff       (20)      196 2023-04-12 20:03:30.453095 multi_date_picker-0.0.2/PKG-INFO
+-rw-r--r--   0 larky      (501) staff       (20)     3676 2023-04-12 13:15:35.000000 multi_date_picker-0.0.2/README.md
+drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 20:03:30.452278 multi_date_picker-0.0.2/multi_date_picker/
+-rw-r--r--   0 larky      (501) staff       (20)    11701 2023-04-12 20:03:26.000000 multi_date_picker-0.0.2/multi_date_picker/MultiDatePicker.py
+-rw-r--r--   0 larky      (501) staff       (20)     2507 2023-04-12 13:15:35.000000 multi_date_picker-0.0.2/multi_date_picker/__init__.py
+-rw-r--r--   0 larky      (501) staff       (20)       81 2023-04-12 20:03:26.000000 multi_date_picker-0.0.2/multi_date_picker/_imports_.py
+-rw-r--r--   0 larky      (501) staff       (20)    16555 2023-04-12 20:03:26.000000 multi_date_picker-0.0.2/multi_date_picker/metadata.json
+-rw-r--r--   0 larky      (501) staff       (20)    75835 2023-04-12 20:03:25.000000 multi_date_picker-0.0.2/multi_date_picker/multi_date_picker.min.js
+-rw-r--r--   0 larky      (501) staff       (20)      101 2023-04-12 20:03:25.000000 multi_date_picker-0.0.2/multi_date_picker/multi_date_picker.min.js.map
+-rw-r--r--   0 larky      (501) staff       (20)     1822 2023-04-12 20:03:26.000000 multi_date_picker-0.0.2/multi_date_picker/package-info.json
+drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 20:03:30.452743 multi_date_picker-0.0.2/multi_date_picker.egg-info/
+-rw-r--r--   0 larky      (501) staff       (20)      196 2023-04-12 20:03:30.000000 multi_date_picker-0.0.2/multi_date_picker.egg-info/PKG-INFO
+-rw-r--r--   0 larky      (501) staff       (20)      491 2023-04-12 20:03:30.000000 multi_date_picker-0.0.2/multi_date_picker.egg-info/SOURCES.txt
+-rw-r--r--   0 larky      (501) staff       (20)        1 2023-04-12 20:03:30.000000 multi_date_picker-0.0.2/multi_date_picker.egg-info/dependency_links.txt
+-rw-r--r--   0 larky      (501) staff       (20)       18 2023-04-12 20:03:30.000000 multi_date_picker-0.0.2/multi_date_picker.egg-info/top_level.txt
+-rw-r--r--   0 larky      (501) staff       (20)     1822 2023-04-12 20:03:18.000000 multi_date_picker-0.0.2/package.json
+-rw-r--r--   0 larky      (501) staff       (20)       38 2023-04-12 20:03:30.453283 multi_date_picker-0.0.2/setup.cfg
+-rw-r--r--   0 larky      (501) staff       (20)      510 2023-04-12 13:15:35.000000 multi_date_picker-0.0.2/setup.py
+drwxr-xr-x   0 larky      (501) staff       (20)        0 2023-04-12 20:03:30.452847 multi_date_picker-0.0.2/tests/
+-rw-r--r--   0 larky      (501) staff       (20)      920 2023-04-12 13:15:35.000000 multi_date_picker-0.0.2/tests/test_usage.py
```

### Comparing `multi_date_picker-0.0.1/README.md` & `multi_date_picker-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `multi_date_picker-0.0.1/multi_date_picker/__init__.py` & `multi_date_picker-0.0.2/multi_date_picker/__init__.py`

 * *Files identical despite different names*

### Comparing `multi_date_picker-0.0.1/multi_date_picker/metadata.json` & `multi_date_picker-0.0.2/multi_date_picker/metadata.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949930555555555%*

 * *Differences: {"'src/lib/components/MultiDatePicker.react.js'": "{'props': {'value': {'type': {'value': {delete: "*

 * *                                                  "[3, 1]}}}, 'multiple': {'description': 'If "*

 * *                                                  '`multiple` is true, the date picker allows '*

 * *                                                  'selecting\\nmultiple dates. The `value` prop '*

 * *                                                  'should be an array of dates.\\nExample usage: '*

 * *                       […]*

```diff
@@ -1,240 +1,240 @@
 {
     "src/lib/components/MultiDatePicker.react.js": {
         "description": "ExampleComponent is an example component.\nIt takes a property, `label`, and\ndisplays it.\nIt renders an input with the property `value`\nwhich is editable by the user.",
         "displayName": "MultiDatePicker",
         "methods": [],
         "props": {
             "animations": {
-                "description": "",
+                "description": "List of animations to apply to the calendar",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
             "arrow": {
-                "description": "",
+                "description": "Whether to display an arrow next to the input",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
                             "name": "bool"
                         },
                         {
                             "name": "element"
                         }
                     ]
                 }
             },
             "arrowClassName": {
-                "description": "",
+                "description": "CSS class name for the arrow",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "arrowStyle": {
-                "description": "",
+                "description": "Style object for the arrow",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
             "buttons": {
-                "description": "",
+                "description": "Whether to display navigation buttons",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "calendar": {
-                "description": "",
+                "description": "Type of calendar to use (e.g. 'gregorian', 'persian')",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "calendarPosition": {
-                "description": "",
+                "description": "Specifies the position of the calendar relative to the input field",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "className": {
-                "description": "",
+                "description": "Custom CSS class name for the component",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "containerClassName": {
-                "description": "",
+                "description": "Sets the CSS class for the container of the date picker",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "containerStyle": {
-                "description": "",
+                "description": "Defines the style object for the container of the date picker",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
             "currentDate": {
-                "description": "",
+                "description": "Current date to use as a basis for the month(s) displayed",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
             "digits": {
-                "description": "",
+                "description": "List of digits to use in the calendar",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
             "disableDayPicker": {
-                "description": "",
+                "description": "Whether to disable the day picker",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "disableMonthPicker": {
-                "description": "",
+                "description": "Whether to disable the month picker",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "disableYearPicker": {
-                "description": "",
+                "description": "Whether to disable the year picker",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "disabled": {
-                "description": "",
+                "description": "Whether the input is disabled",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "displayWeekNumbers": {
-                "description": "",
+                "description": "Whether to display week numbers",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "editable": {
-                "description": "",
+                "description": "Determines whether the date picker input field is editable or not",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "fixMainPosition": {
-                "description": "",
+                "description": "Determines whether the date picker should be fixed in the main position",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "fixRelativePosition": {
-                "description": "",
+                "description": "Determines whether the date picker should be fixed in the relative position",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "format": {
-                "description": "",
+                "description": "The `format` prop specifies the format in which the date\nshould be displayed in the input field. The supported\nformats are similar to those in the `Date.prototype.toLocaleDateString()`\nmethod, such as \"dd/MM/yyyy\", \"MM/dd/yyyy\", \"yyyy-MM-dd\", etc.\nExample usage: format=\"yyyy-MM-dd\"",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "formattingIgnoreList": {
-                "description": "",
+                "description": "List of format tokens to ignore when parsing the `value`",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
             "fullYear": {
-                "description": "",
+                "description": "Whether to display the full year (i.e. 12 months)",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "hideMonth": {
-                "description": "",
+                "description": "Whether to hide the month dropdown",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "hideOnScroll": {
-                "description": "",
+                "description": "Controls whether or not the date picker should hide when scrolling",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "hideYear": {
-                "description": "",
+                "description": "Whether to hide the year dropdown",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "id": {
                 "description": "The ID used to identify this component in Dash callbacks.",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "inputClass": {
-                "description": "",
+                "description": "CSS class name for the input field",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "inputMode": {
-                "description": "",
+                "description": "Sets the input mode for the date picker",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "locale": {
-                "description": "",
+                "description": "Language/locale to use (e.g. 'en-US', 'fa-IR')",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "mapDays": {
-                "description": "",
+                "description": "Custom function to modify the appearance of each day",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "maxDate": {
-                "description": "",
+                "description": "Latest selectable date (can be a string, number, or `Date` object)",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
                             "name": "instanceOf",
                             "value": "Date"
@@ -248,15 +248,15 @@
                         {
                             "name": "number"
                         }
                     ]
                 }
             },
             "minDate": {
-                "description": "",
+                "description": "Earliest selectable date (can be a string, number, or `Date` object)",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
                             "name": "instanceOf",
                             "value": "Date"
@@ -270,281 +270,281 @@
                         {
                             "name": "number"
                         }
                     ]
                 }
             },
             "mobileButtons": {
-                "description": "",
+                "description": "Sets the buttons for the mobile version of the date picker",
                 "required": false,
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "instanceOf",
                         "value": "HTMLButtonElement"
                     }
                 }
             },
             "mobileLabels": {
-                "description": "",
+                "description": "Sets the mobile labels for the date picker",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
             "months": {
-                "description": "",
+                "description": "List of month names",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
             "multiple": {
-                "description": "",
+                "description": "If `multiple` is true, the date picker allows selecting\nmultiple dates. The `value` prop should be an array of dates.\nExample usage: multiple={true} value={[\"2023-04-12\", \"2023-04-15\"]}",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "name": {
-                "description": "",
+                "description": "Name of the input field",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "numberOfMonths": {
-                "description": "",
+                "description": "Number of months to display at once",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
             "offsetX": {
-                "description": "",
+                "description": "Sets the horizontal offset for the date picker",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
             "offsetY": {
-                "description": "",
+                "description": "Sets the vertical offset for the date picker",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
             "onChange": {
-                "description": "",
+                "description": "Function called when the value changes",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onClose": {
-                "description": "",
+                "description": "Callback function called when the date picker is closed",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onFocusedDateChange": {
-                "description": "",
+                "description": "Function called when the focused date changes",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onMonthChange": {
-                "description": "",
+                "description": "Function called when the selected month changes",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onOpen": {
-                "description": "",
+                "description": "Callback function called when the date picker is opened",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onOpenPickNewDate": {
-                "description": "",
+                "description": "Determines whether a new date should be picked when the date picker is opened",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "onPositionChange": {
-                "description": "",
+                "description": "Callback function called when the position of the date picker changes",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onPropsChange": {
-                "description": "",
+                "description": "Function called when any prop changes",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onYearChange": {
-                "description": "",
+                "description": "Function called when the selected year changes",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "onlyMonthPicker": {
-                "description": "",
+                "description": "If `onlyMonthPicker` is true, the date picker displays\na dropdown for selecting a month, but not a day or year.\nExample usage: onlyMonthPicker={true}",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "onlyShowInRangeDates": {
-                "description": "",
+                "description": "Restricts the date picker to only show dates within a specified range",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "onlyYearPicker": {
-                "description": "",
+                "description": "If `onlyYearPicker` is true, the date picker displays\na dropdown for selecting a year, but not a day or month.\nExample usage: onlyYearPicker={true}",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "placeholder": {
-                "description": "",
+                "description": "Placeholder text for the input field",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "plugins": {
-                "description": "",
+                "description": "List of additional plugins to use",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
             "portal": {
-                "description": "",
+                "description": "Determines whether the date picker should be rendered inside a portal",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "portalTarget": {
-                "description": "",
+                "description": "Specifies the target for the portal",
                 "required": false,
                 "type": {
                     "name": "instanceOf",
                     "value": "HTMLElement"
                 }
             },
             "range": {
-                "description": "",
+                "description": "If `range` is true, the date picker allows selecting\na date range. The `value` prop should be an array with\ntwo dates representing the start and end of the range.\nExample usage: range={true} value={[\"2023-04-12\", \"2023-04-15\"]}",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "rangeHover": {
-                "description": "",
+                "description": "Whether to enable the range hover effect",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "readOnly": {
-                "description": "",
+                "description": "Whether the input is read-only",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "render": {
-                "description": "",
+                "description": "Defines the render function or component for the input field",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
                             "name": "elementType"
                         },
                         {
                             "name": "func"
                         }
                     ]
                 }
             },
             "renderButton": {
-                "description": "",
+                "description": "Custom function or element to render navigation buttons",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
                             "name": "func"
                         },
                         {
                             "name": "element"
                         }
                     ]
                 }
             },
             "scrollSensitive": {
-                "description": "",
+                "description": "Determines if the date picker should respond to scroll events",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
             "shadow": {
-                "description": "",
+                "description": "Whether to display a shadow around the calendar",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "showOtherDays": {
-                "description": "",
+                "description": "Whether to show days from other months",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "sort": {
-                "description": "",
+                "description": "Whether to sort the months and weekdays alphabetically",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "style": {
-                "description": "",
+                "description": "Style object for the input field",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
             "title": {
-                "description": "",
+                "description": "Title of the input field",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "value": {
                 "description": "The value displayed in the input.",
@@ -553,58 +553,52 @@
                     "name": "union",
                     "value": [
                         {
                             "name": "instanceOf",
                             "value": "Date"
                         },
                         {
-                            "name": "object"
-                        },
-                        {
                             "name": "string"
                         },
                         {
-                            "name": "number"
-                        },
-                        {
                             "name": "array"
                         }
                     ]
                 }
             },
             "weekDays": {
-                "description": "",
+                "description": "List of week day names",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
             "weekNumber": {
-                "description": "",
+                "description": "Format string for the week number label",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "weekPicker": {
-                "description": "",
+                "description": "Whether to enable the week picker",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
             "weekStartDayIndex": {
-                "description": "",
+                "description": "Index of the day on which each week starts (0 = Sunday, 1 = Monday, etc.)",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
             "zIndex": {
-                "description": "",
+                "description": "Custom z-index value for the component",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             }
         }
     }
```

### Comparing `multi_date_picker-0.0.1/multi_date_picker/multi_date_picker.min.js` & `multi_date_picker-0.0.2/multi_date_picker/multi_date_picker.min.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -63,15 +63,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(a()),
                 r = o(e);
             if (!t) return r;
             var n = r.split("/"),
                 i = n.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_0_1m1681313296"), n.splice(-1, 1, i.join(".")), n.join("/")
+            return i.splice(1, 0, "v0_0_2m1681329805"), n.splice(-1, 1, i.join(".")), n.join("/")
         }
     }
     return r(r.s = 6)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -361,24 +361,24 @@
             Y = e.weekNumber,
             E = void 0 === Y ? "" : Y,
             C = e.rangeHover,
             j = n.useRef({}),
             I = t.today,
             L = t.minDate,
             A = t.maxDate,
-            T = t.range,
-            W = t.date,
+            W = t.range,
+            T = t.date,
             R = t.selectedDate,
             F = t.onlyMonthPicker,
             z = t.onlyYearPicker,
             H = !F && !z,
             V = p(n.useState(), 2),
             _ = V[0],
             B = V[1];
-        j.current.date = W;
+        j.current.date = T;
         var J = n.useMemo((function() {
             return H ? function(e, t, r, n) {
                 if (!e) return [];
                 for (var a = [], o = 0; o < r; o++) {
                     var i = (e = new u.default(e).toFirstOfMonth()).monthIndex,
                         s = [];
                     e.toFirstOfWeek().add(n, "day"), e.monthIndex === i && e.day > 1 && e.subtract(7, "days");
@@ -390,15 +390,15 @@
                         }), e.day += 1;
                         if (s.push(d), l > 2 && e.monthIndex !== i && !t) break
                     }
                     a.push(s)
                 }
                 return a
             }(j.current.date, o, y, g) : []
-        }), [W.monthIndex, W.year, W.calendar, W.locale, H, o, y, g]);
+        }), [T.monthIndex, T.year, T.calendar, T.locale, H, o, y, g]);
         return H && s.default.createElement("div", {
             className: "rmdp-day-picker ".concat(S ? "rmdp-full-year" : ""),
             style: {
                 display: S ? "grid" : "flex"
             },
             onMouseLeave: function() {
                 return C && B()
@@ -451,15 +451,15 @@
                             i = e.current;
                         if (!U(e) || o) n.push("rmdp-day-hidden");
                         else {
                             (L && a < L || A && a > A || e.disabled) && (n.push("rmdp-disabled"), e.disabled || (e.disabled = !0)), i || n.push("rmdp-deactive");
                             var s = t > 1 && i || 1 === t;
                             e.disabled && l || (x(a, I) && n.push("rmdp-today"), r = a, [].concat(R).some((function(e) {
                                 return x(e, r)
-                            })) && s && !T && n.push("rmdp-selected")), T && !e.disabled && s && (n.push(O(a, R)), n = n.concat(M(a, R, _, C)))
+                            })) && s && !W && n.push("rmdp-selected")), W && !e.disabled && s && (n.push(O(a, R)), n = n.concat(M(a, R, _, C)))
                         }
                         return n.join(" ")
                     }(e, y);
                     return (e.hidden || e.disabled) && (b = b.replace("sd", "")), s.default.createElement("div", {
                         key: a,
                         className: w,
                         onMouseEnter: function() {
@@ -562,22 +562,22 @@
                 className: "rmdp-header-values",
                 style: w
             }, !f && s.default.createElement("span", {
                 style: {
                     cursor: d || o || x ? "default" : "pointer"
                 },
                 onClick: function() {
-                    return !o && T("mustShowMonthPicker")
+                    return !o && W("mustShowMonthPicker")
                 }
             }, e, !h && (m ? "،" : ",")), !h && s.default.createElement("span", {
                 style: {
                     cursor: d || a || D ? "default" : "pointer"
                 },
                 onClick: function() {
-                    return !a && T("mustShowYearPicker")
+                    return !a && W("mustShowYearPicker")
                 }
             }, v[t]))
         })), i && L("right")));
 
         function L(e) {
             var t = function() {
                     return A("right" === e ? 1 : -1)
@@ -597,15 +597,15 @@
         function A(e) {
             d || e < 0 && E || e > 0 && C || (y ? k.year += e : O || D ? (N += 12 * e, e < 0 && M && N < M.year && (N = M.year), e > 0 && S && N > S.year && (N = S.year)) : (k.toFirstOfMonth(), x ? k.year += e : (k.month += e, u(k))), r(c(c({}, t), {}, {
                 date: k,
                 year: N
             })))
         }
 
-        function T(e) {
+        function W(e) {
             if (!d) {
                 var n = {
                     mustShowMonthPicker: !1,
                     mustShowYearPicker: !1
                 };
                 n[e] = !t[e], r(c(c({}, t), n))
             }
@@ -842,20 +842,20 @@
             calendar: t
         }), e
     }
 
     function A(e) {
         "_self" in s.default.createElement("div") && console.warn(e.join("\n"))
     }
-    var T = new u.default,
-        W = T.calendar,
-        R = T.locale;
+    var W = new u.default,
+        T = W.calendar,
+        R = W.locale;
 
     function F(e, t) {
-        return e && e.constructor !== Object && (A(z("calendar")), e = void 0), t && t.constructor !== Object && (A(z("locale")), t = void 0), [e || W, t || R]
+        return e && e.constructor !== Object && (A(z("calendar")), e = void 0), t && t.constructor !== Object && (A(z("locale")), t = void 0), [e || T, t || R]
     }
 
     function z(e) {
         return ["".concat(e, " must be an object"), "https://shahabyazdi.github.io/react-multi-date-picker/calendars/"]
     }
 
     function H(e) {
@@ -892,16 +892,16 @@
             x = e.weekDays,
             D = e.months,
             O = e.children,
             M = e.onChange,
             P = e.showOtherDays,
             L = e.minDate,
             A = e.maxDate,
-            T = e.mapDays,
-            W = e.disableMonthPicker,
+            W = e.mapDays,
+            T = e.disableMonthPicker,
             R = e.disableYearPicker,
             z = e.formattingIgnoreList,
             H = e.onReady,
             _ = e.onlyShowInRangeDates,
             J = void 0 === _ || _,
             K = e.zIndex,
             $ = void 0 === K ? 100 : K,
@@ -933,15 +933,15 @@
             ke = e.displayWeekNumbers,
             xe = e.weekNumber,
             De = e.weekPicker,
             Oe = e.rangeHover;
         !te || te instanceof u.default || (console.warn("currentDate must be instance of DateObject"), te = void 0), ("number" != typeof se || se < 0 || se > 6) && (se = 0), ("number" != typeof ee || ee < 1 || d || f) && (ee = 1), (v || b || w(a)) && (b || v || (v = !0), v && b && (v = !1)), De && (b = !0, v = !1), we && (ee = 12, d = !1, f = !1), f && !pe && (pe = !0);
         var Me = F(o, i),
             Se = p(Me, 2);
-        o = Se[0], i = Se[1], l = I(d, f, l), z = Y(z), T = [].concat(T).filter(Boolean), Z = [].concat.apply([], Z);
+        o = Se[0], i = Se[1], l = I(d, f, l), z = Y(z), W = [].concat(W).filter(Boolean), Z = [].concat.apply([], Z);
         var Pe = n.useState({}),
             Ne = p(Pe, 2),
             Ye = Ne[0],
             Ee = Ne[1],
             Ce = {},
             je = n.useRef({
                 mustCallOnReady: !0,
@@ -1029,69 +1029,69 @@
             Le = {
                 top: [],
                 bottom: [],
                 left: [],
                 right: []
             },
             Ae = V(null === (r = Ye.date) || void 0 === r ? void 0 : r.locale),
-            Te = {
+            We = {
                 state: Ye,
                 setState: Ee,
                 onChange: Ve,
                 sort: G,
                 handleFocusedDate: Be,
                 isRTL: Ae,
                 fullYear: we,
                 monthAndYears: $e(),
                 rangeHover: Oe
             },
-            We = arguments[0],
-            Re = We.datePickerProps,
-            Fe = We.DatePicker,
-            ze = m(We, B);
+            Te = arguments[0],
+            Re = Te.datePickerProps,
+            Fe = Te.DatePicker,
+            ze = m(Te, B);
         return He(), Ye.today ? s.default.createElement("div", {
             ref: Ke,
             className: "rmdp-wrapper rmdp-".concat(ve ? "shadow" : "border", " ").concat(k || ""),
             style: {
                 zIndex: $
             }
         }, Le.top, s.default.createElement("div", {
             style: {
                 display: "flex"
             },
             className: Ie
         }, Le.left, !le && s.default.createElement("div", {
             className: "rmdp-calendar ".concat(Ae ? "rmdp-rtl" : "", " ").concat(Ue(["left", "right"]))
-        }, s.default.createElement(N, h({}, Te, {
+        }, s.default.createElement(N, h({}, We, {
             disableYearPicker: R,
-            disableMonthPicker: W,
+            disableMonthPicker: T,
             buttons: ae,
             renderButton: oe,
             handleMonthChange: Je,
             disabled: me,
             hideMonth: pe,
             hideYear: ye
         })), s.default.createElement("div", {
             style: {
                 position: "relative"
             }
-        }, s.default.createElement(S, h({}, Te, {
+        }, s.default.createElement(S, h({}, We, {
             showOtherDays: P,
-            mapDays: T,
+            mapDays: W,
             onlyShowInRangeDates: J,
             customWeekDays: x,
             numberOfMonths: ee,
             weekStartDayIndex: se,
             hideWeekDays: be,
             displayWeekNumbers: ke,
             weekNumber: xe
-        })), !we && s.default.createElement(s.default.Fragment, null, !W && s.default.createElement(E, h({}, Te, {
+        })), !we && s.default.createElement(s.default.Fragment, null, !T && s.default.createElement(E, h({}, We, {
             customMonths: D,
             handleMonthChange: Je
-        })), !R && s.default.createElement(j, h({}, Te, {
+        })), !R && s.default.createElement(j, h({}, We, {
             onYearChange: ce
         }))))), Le.right), Le.bottom, O) : null;
 
         function He() {
             if (je.current.isReady && w(Z)) {
                 var e = {
                         state: Ye,
@@ -1122,15 +1122,15 @@
                                     ["top", "bottom"].includes(i) ? (l === i && s > a && (o.bottom = !0), l === i && s < a && (o.top = !0)) : (Ie.includes("border-top") && (o.top = !0), Ie.includes("border-bottom") && (o.bottom = !0), l === i && s > a && (o.right = !0), l === i && s < a && (o.left = !0))
                                 } Le[i].push(n.cloneElement(r, c({
                                 key: a,
                                 position: i,
                                 nodes: o
                             }, e)))
                         }
-                    } else "mapDays" === r.type && T.push(r.fn(e))
+                    } else "mapDays" === r.type && W.push(r.fn(e))
                 }))
             }
         }
 
         function Ve(e, t) {
             if (!me) {
                 if (e || null === e) {
@@ -1249,16 +1249,16 @@
             M = e.id,
             S = e.title,
             P = e.placeholder,
             N = e.required,
             E = e.style,
             j = void 0 === E ? {} : E,
             L = e.className,
-            T = void 0 === L ? "" : L,
-            W = e.inputClass,
+            W = void 0 === L ? "" : L,
+            T = e.inputClass,
             R = e.disabled,
             z = e.render,
             _ = e.weekDays,
             B = e.months,
             U = e.children,
             X = e.inputMode,
             q = e.scrollSensitive,
@@ -1295,16 +1295,16 @@
             Ye = e.onOpenPickNewDate,
             Ee = void 0 === Ye || Ye,
             Ce = e.mobileButtons,
             je = void 0 === Ce ? [] : Ce,
             Ie = m(e, K),
             Le = n.useState(),
             Ae = p(Le, 2),
-            Te = Ae[0],
-            We = Ae[1],
+            We = Ae[0],
+            Te = Ae[1],
             Re = n.useState(),
             Fe = p(Re, 2),
             ze = Fe[0],
             He = Fe[1],
             Ve = n.useState(""),
             _e = p(Ve, 2),
             Be = _e[0],
@@ -1400,84 +1400,84 @@
             }
             r || s || !n ? s && !r && (s = void 0) : e = n, k || D || w(e) ? (w(e) || (e = [e]), e = e.map(d).filter((function(e) {
                 return void 0 !== e
             })), k && e.length > 2 && (e = [e[0], l()]), Je(Z(e, at))) : (w(e) && (e = l()), e = d(e), document.activeElement !== G(tt) && Je(e ? e.format() : "")), nt.current = c(c({}, nt.current), {}, {
                 date: e,
                 separator: at,
                 initialValue: s || r
-            }), nt.current.mobile && et.current.isOpen ? He(e) : We(e)
+            }), nt.current.mobile && et.current.isOpen ? He(e) : Te(e)
         }), [r, a, o, i, k, D, at, d, y, _, B, ke, ne]), n.useEffect((function() {
             var e = nt.current.selection;
             if (e) {
                 var t = G(tt);
                 t && (t.setSelectionRange(e, e), nt.current.selection = void 0, et.current.refreshPosition())
             }
-        }), [Be]), (D || k || w(Te) || !ue) && (X = "none"), s.default.createElement(l.default, h({
+        }), [Be]), (D || k || w(We) || !ue) && (X = "none"), s.default.createElement(l.default, h({
             ref: ct,
             element: ft(),
             popper: Ke && ht(),
             active: !it && Ge,
             position: se,
             arrow: !it && be,
             fixMainPosition: !Q || ge,
             zIndex: pe,
             onChange: !it && ve,
             containerClassName: "rmdp-container ".concat(oe),
-            arrowClassName: ["rmdp-ep-arrow", "rmdp-ep-".concat(Oe ? "shadow" : "border"), T, he].join(" ")
+            arrowClassName: ["rmdp-ep-arrow", "rmdp-ep-".concat(Oe ? "shadow" : "border"), W, he].join(" ")
         }, Ie));
 
         function ct(e) {
             if (e && (e.openCalendar = function() {
                     return setTimeout((function() {
                         return bt()
                     }), 10)
                 }, e.closeCalendar = st, e.isOpen = Ke && Ge), et.current = e, t instanceof Function) return t(e);
             t && (t.current = e)
         }
 
         function ft() {
             if ("string" == typeof Se && A(["the type Prop is deprecated.", "https://shahabyazdi.github.io/react-multi-date-picker/types/"]), z) {
-                var e, t = w(Te) || D || k ? Z(Te, at) : Be;
+                var e, t = w(We) || D || k ? Z(We, at) : Be;
                 return s.default.createElement("div", {
                     ref: tt
                 }, n.isValidElement(z) ? n.cloneElement(z, (f(e = {}, D || k ? "stringDates" : "stringDate", t), f(e, "value", t), f(e, "openCalendar", bt), f(e, "handleValueChange", wt), f(e, "locale", o), f(e, "separator", at), e)) : z instanceof Function ? z(t, bt, wt, o, at) : null)
             }
             return s.default.createElement("input", {
                 ref: tt,
                 type: "text",
                 name: O,
                 id: M,
                 title: S,
                 required: N,
                 onFocus: bt,
-                className: W || "rmdp-input",
+                className: T || "rmdp-input",
                 placeholder: P,
                 value: Be,
                 onChange: wt,
                 style: j,
                 autoComplete: "off",
                 disabled: !!R,
                 inputMode: X || (it ? "none" : void 0),
                 readOnly: xe
             })
         }
 
         function ht() {
             return s.default.createElement(J, h({
                 ref: rt,
-                value: ze || Te,
+                value: ze || We,
                 onChange: vt,
                 range: k,
                 multiple: D,
                 calendar: a,
                 locale: o,
                 format: i,
                 onlyMonthPicker: d,
                 onlyYearPicker: y,
-                className: T + (it ? " rmdp-mobile" : ""),
+                className: W + (it ? " rmdp-mobile" : ""),
                 weekDays: _,
                 months: B,
                 digits: ke,
                 minDate: te,
                 maxDate: re,
                 formattingIgnoreList: JSON.parse(ne),
                 onPropsChange: we,
@@ -1487,15 +1487,15 @@
                 datePickerProps: ot,
                 onFocusedDateChange: xt,
                 weekPicker: Pe
             }, Ie), U, it && pt())
         }
 
         function mt() {
-            return "string" == typeof T && T.includes("rmdp-mobile")
+            return "string" == typeof W && W.includes("rmdp-mobile")
         }
 
         function pt() {
             var e = [].concat.apply([], ot.plugins || []).some((function(e) {
                 var t = e.props;
                 return !(void 0 === t ? {} : t).disabled
             }));
@@ -1555,21 +1555,21 @@
 
         function gt() {
             return Ee && !r && !nt.current.date && !k && !D && !it
         }
 
         function vt(e, t) {
             if (it && !t) return He(e);
-            We(e), nt.current = c(c({}, nt.current), {}, {
+            Te(e), nt.current = c(c({}, nt.current), {}, {
                 date: e
             }), null == b || b(e), e && Je(Z(e, at))
         }
 
         function wt(e) {
-            if (!w(Te) && ue) {
+            if (!w(We) && ue) {
                 nt.current.selection = e.target.selectionStart;
                 var t = e.target.value,
                     r = {
                         calendar: a,
                         locale: o,
                         format: i,
                         ignoreList: JSON.parse(ne)
@@ -1739,19 +1739,19 @@
                     Y = u(e.current, P, N),
                     E = Y.top,
                     C = Y.left,
                     j = Y.height,
                     I = Y.width,
                     L = Y.right,
                     A = Y.bottom,
-                    T = u(t.current, P, N),
-                    W = T.top,
-                    R = T.left,
-                    F = T.height,
-                    z = T.width,
+                    W = u(t.current, P, N),
+                    T = W.top,
+                    R = W.left,
+                    F = W.height,
+                    z = W.width,
                     H = document.documentElement,
                     V = H.clientHeight,
                     _ = H.clientWidth,
                     B = t.current.parentNode,
                     J = function(e) {
                         if (!e) return [0, 0];
                         var t = i((e.style.transform.match(/translate\((.*?)px,\s(.*?)px\)/) || []).map((function(e) {
@@ -1788,15 +1788,15 @@
                     ne = I - z,
                     ae = j - F,
                     oe = "left" === G ? 0 : "right" === G ? ne : ne / 2,
                     ie = ne - oe,
                     se = "top" === G ? 0 : "bottom" === G ? ae : ae / 2,
                     le = ae - se,
                     ue = C - R + X,
-                    de = E - W + K,
+                    de = E - T + K,
                     ce = 0,
                     fe = 0,
                     he = d(e.current),
                     me = [],
                     pe = r.current,
                     ye = u(pe, P, N) || {},
                     be = ye.height,
@@ -1945,16 +1945,16 @@
                 Y = void 0 === N || N,
                 E = n.portal,
                 C = n.portalTarget,
                 j = "undefined" != typeof window,
                 I = j && C instanceof HTMLElement,
                 L = !0 === m,
                 A = s && !0 === Y,
-                T = t.useRef(),
                 W = t.useRef(),
+                T = t.useRef(),
                 R = t.useRef(),
                 F = t.useRef(),
                 z = t.useMemo((function() {
                     return {
                         position: d,
                         fixMainPosition: v,
                         fixRelativePosition: w,
@@ -1963,15 +1963,15 @@
                         defaultArrow: L,
                         animations: D,
                         zIndex: M,
                         onChange: P
                     }
                 }), [d, v, w, k, x, L, D, P, M]),
                 H = t.useCallback((function() {
-                    R.current && (R.current.style.transition = ""), W.current && (W.current.parentNode.style.transition = "")
+                    R.current && (R.current.style.transition = ""), T.current && (T.current.parentNode.style.transition = "")
                 }), []),
                 V = {
                     element: a({
                         display: "inline-block",
                         height: "max-content"
                     }, c),
                     arrow: a({
@@ -1997,30 +1997,30 @@
                     var e = F.current;
                     return document.body.appendChild(e),
                         function() {
                             return document.body.removeChild(e)
                         }
                 }
             }), [E, I]), t.useEffect((function() {
-                if (!A) return H(), W.current.parentNode.style.visibility = "hidden", void(R.current && (R.current.style.visibility = "hidden"));
+                if (!A) return H(), T.current.parentNode.style.visibility = "hidden", void(R.current && (R.current.style.visibility = "hidden"));
 
                 function e(e) {
-                    e && "resize" !== e.type && !e.target.contains(T.current) || (e && H(), l(T, W, R, z, e))
+                    e && "resize" !== e.type && !e.target.contains(W.current) || (e && H(), l(W, T, R, z, e))
                 }
                 return e(), document.addEventListener("scroll", e, !0), window.addEventListener("resize", e),
                     function() {
                         document.removeEventListener("scroll", e, !0), window.removeEventListener("resize", e)
                     }
             }), [A, z, H]), t.useEffect((function() {
                 var e = {
                         portal: E,
                         isValidPortalTarget: I
                     },
                     t = F.current.data;
-                JSON.stringify(e) !== JSON.stringify(t) && (F.current.data = e, T.current.refreshPosition())
+                JSON.stringify(e) !== JSON.stringify(t) && (F.current.data = e, W.current.refreshPosition())
             }), [E, I]);
             var _ = r.default.createElement(r.default.Fragment, null, function() {
                 if (!m || !A) return null;
                 var e = r.default.createElement("div", {
                         ref: R,
                         style: V.arrow
                     }),
@@ -2030,23 +2030,23 @@
                         className: "ep-arrow ".concat(S ? "ep-shadow" : "", " ").concat(g)
                     };
                 return t.cloneElement(e, n)
             }(), r.default.createElement("div", {
                 className: S ? "ep-popper-shadow" : "",
                 style: V.popper
             }, r.default.createElement("div", {
-                ref: W
+                ref: T
             }, s)));
             return r.default.createElement("div", {
                 ref: function(e) {
                     if (e && (e.removeTransition = H, e.refreshPosition = function() {
                             return setTimeout((function() {
-                                return l(T, W, R, z, {})
+                                return l(W, T, R, z, {})
                             }), 10)
-                        }), T.current = e, o instanceof Function) return o(e);
+                        }), W.current = e, o instanceof Function) return o(e);
                     o && (o.current = e)
                 },
                 className: h,
                 style: V.element
             }, i, E && j ? e.createPortal(_, I ? C : F.current) : _)
         }))
     }(r(4), r(1))
@@ -2340,16 +2340,16 @@
         Y = new WeakMap,
         E = new WeakMap,
         C = new WeakMap,
         j = new WeakMap,
         I = new WeakMap,
         L = new WeakMap,
         A = new WeakMap,
-        T = new WeakMap,
         W = new WeakMap,
+        T = new WeakMap,
         R = new WeakMap,
         F = new WeakMap,
         z = new WeakMap,
         H = new WeakMap,
         V = new WeakMap,
         _ = new WeakMap,
         B = new WeakMap,
@@ -2382,18 +2382,18 @@
                     value: void 0
                 }), b(this, L, {
                     writable: !0,
                     value: void 0
                 }), b(this, A, {
                     writable: !0,
                     value: k
-                }), b(this, T, {
+                }), b(this, W, {
                     writable: !0,
                     value: x
-                }), b(this, W, {
+                }), b(this, T, {
                     writable: !0,
                     value: !1
                 }), b(this, R, {
                     writable: !0,
                     value: {}
                 }), b(this, F, {
                     writable: !0,
@@ -2407,15 +2407,15 @@
                 }), b(this, V, {
                     writable: !0,
                     value: function(e, t) {
                         switch (e) {
                             case "YYYY":
                                 return ["year", t];
                             case "YY":
-                                return ["year", "".concat(g(r, T).century).concat(t)];
+                                return ["year", "".concat(g(r, W).century).concat(t)];
                             case "MMMM":
                             case "MMM":
                                 return ["month", r.months.findIndex((function(e) {
                                     var r = e.name,
                                         n = e.shortName;
                                     return new RegExp(t, "i").test(r + n)
                                 })) + 1];
@@ -2445,15 +2445,15 @@
                             default:
                                 return []
                         }
                     }
                 }), b(this, _, {
                     writable: !0,
                     value: function() {
-                        return 0 === g(r, P) && 0 !== g(r, T).startYear
+                        return 0 === g(r, P) && 0 !== g(r, W).startYear
                     }
                 }), b(this, B, {
                     writable: !0,
                     value: function() {
                         if (g(r, H) && r.isValid) {
                             var e = Math.floor,
                                 t = function(t, r) {
@@ -2483,17 +2483,17 @@
                                             return e >= t || e < 0
                                         }(r[a], i)) {
                                         var s = d(t(r[a], i), 2),
                                             l = s[0],
                                             u = s[1];
                                         r[o] += l, r[a] = u
                                     }
-                                })), v(r, H, !0), n(); g(r, Y) < -g(r, T).yearLength || g(r, Y) > g(r, T).yearLength;) {
+                                })), v(r, H, !0), n(); g(r, Y) < -g(r, W).yearLength || g(r, Y) > g(r, W).yearLength;) {
                                 if (g(r, N) > 0) {
-                                    for (var a = g(r, T).getMonthLengths(r.isLeap), o = 0; o < g(r, N); o++) v(r, Y, g(r, Y) + a[o]);
+                                    for (var a = g(r, W).getMonthLengths(r.isLeap), o = 0; o < g(r, N); o++) v(r, Y, g(r, Y) + a[o]);
                                     v(r, N, 0)
                                 }
                                 var i = r.isLeap ? r.calendar.yearLength + 1 : r.calendar.yearLength;
                                 v(r, Y, g(r, Y) + i * (g(r, Y) < 0 ? 1 : -1)), v(r, P, g(r, P) + (g(r, Y) < 0 ? -1 : 1))
                             }
                             for (;;) {
                                 var s;
@@ -2530,15 +2530,15 @@
                 var n = D(t) ? l({}, t) : t,
                     a = !0;
                 if (n && "boolean" != typeof n || (n = {
                         date: new Date
                     }), D(n) || (n = {
                         date: n
                     }), 0 !== Object.keys(n).length) {
-                    for (var o in D(n.calendar) && v(this, T, n.calendar), D(n.locale) && v(this, A, n.locale), isNaN(n.year) && isNaN(n.month) && isNaN(n.day) && !n.date && (n.date = new Date), n.date && ("string" == typeof n.date && n.format && v(this, L, n.format), this.setDate(n.date), n.calendar && this.convert(n.calendar), a = !1), delete n.calendar, delete n.locale, delete n.date, n) this.set(o, n[o]);
+                    for (var o in D(n.calendar) && v(this, W, n.calendar), D(n.locale) && v(this, A, n.locale), isNaN(n.year) && isNaN(n.month) && isNaN(n.day) && !n.date && (n.date = new Date), n.date && ("string" == typeof n.date && n.format && v(this, L, n.format), this.setDate(n.date), n.calendar && this.convert(n.calendar), a = !1), delete n.calendar, delete n.locale, delete n.date, n) this.set(o, n[o]);
                     g(this, _).call(this) && v(this, P, -1), a && g(this, B).call(this)
                 }
             }
             var t, r;
             return t = e, (r = [{
                 key: "parse",
                 value: function(e) {
@@ -2565,38 +2565,38 @@
                             return new RegExp(w, "i").test(e.name)
                         }))), b[1] = w;
                         var k = d(b.map(O), 7),
                             x = k[0],
                             D = k[1],
                             M = k[2],
                             S = k[3],
-                            T = k[4],
-                            W = k[5],
+                            W = k[4],
+                            T = k[5],
                             R = k[6];
-                        v(this, P, x), v(this, N, D), v(this, Y, M), v(this, E, S), v(this, C, T), v(this, j, W), v(this, I, R)
+                        v(this, P, x), v(this, N, D), v(this, Y, M), v(this, E, S), v(this, C, W), v(this, j, T), v(this, I, R)
                     }
                     var F = d(g(this, A).meridiems[1], 2),
                         z = F[0],
                         H = F[1];
                     return g(this, E) < 12 && (e.includes(z) || e.includes(H)) && v(this, E, g(this, E) + 12), g(this, B).call(this), this
                 }
             }, {
                 key: "convert",
                 value: function() {
                     var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : x,
                         r = arguments.length > 1 ? arguments[1] : void 0;
-                    if (D(r) && v(this, A, r), !D(t) || t.name === g(this, T).name) return this;
+                    if (D(r) && v(this, A, r), !D(t) || t.name === g(this, W).name) return this;
                     var n = this.toJulianDay() - t.epoch,
                         a = new e({
                             calendar: t,
                             year: t.guessYear(n, g(this, P)),
                             month: 1,
                             day: 1
                         });
-                    return a.day += n - a.toDays(), v(this, P, a.year), v(this, N, a.month.index), v(this, Y, a.day), v(this, T, t), this
+                    return a.day += n - a.toDays(), v(this, P, a.year), v(this, N, a.month.index), v(this, Y, a.day), v(this, W, t), this
                 }
             }, {
                 key: "format",
                 value: function(e, t) {
                     if (!this.isValid || e && "string" != typeof e) return "";
                     e || (e = g(this, L) || "YYYY/MM/DD"), M(t) || (t = []), t = (t = t.concat(g(this, z))).filter((function(e) {
                         return "string" == typeof e || (console.warn("type of all items in the ignore list must be string, found", n(e)), !1)
@@ -2765,15 +2765,15 @@
             }, {
                 key: "setDate",
                 value: function(t) {
                     if ("string" == typeof t) {
                         if (!g(this, F).test(t)) return this.parse(t);
                         t = new Date(t)
                     }
-                    return "number" == typeof t && (t = new Date(t)), t instanceof Date && (v(this, T, x), v(this, P, t.getFullYear()), v(this, N, t.getMonth()), v(this, Y, t.getDate()), v(this, E, t.getHours()), v(this, C, t.getMinutes()), v(this, j, t.getSeconds()), v(this, I, t.getMilliseconds()), v(this, W, !1)), t instanceof e && (v(this, P, t.year), v(this, N, t.month.index), v(this, Y, t.day), v(this, E, t.hour), v(this, C, t.minute), v(this, j, t.second), v(this, I, t.millisecond), v(this, A, t.locale), v(this, L, t._format), v(this, T, t.calendar), v(this, W, t.isUTC), v(this, z, t.ignoreList), v(this, R, t.custom)), this
+                    return "number" == typeof t && (t = new Date(t)), t instanceof Date && (v(this, W, x), v(this, P, t.getFullYear()), v(this, N, t.getMonth()), v(this, Y, t.getDate()), v(this, E, t.getHours()), v(this, C, t.getMinutes()), v(this, j, t.getSeconds()), v(this, I, t.getMilliseconds()), v(this, T, !1)), t instanceof e && (v(this, P, t.year), v(this, N, t.month.index), v(this, Y, t.day), v(this, E, t.hour), v(this, C, t.minute), v(this, j, t.second), v(this, I, t.millisecond), v(this, A, t.locale), v(this, L, t._format), v(this, W, t.calendar), v(this, T, t.isUTC), v(this, z, t.ignoreList), v(this, R, t.custom)), this
                 }
             }, {
                 key: "setIgnoreList",
                 value: function(e) {
                     return this.ignoreList = e, this
                 }
             }, {
@@ -2876,30 +2876,30 @@
                 value: function() {
                     return this.format()
                 }
             }, {
                 key: "toDate",
                 value: function() {
                     var t = new e(this);
-                    return "gregorian" !== g(this, T).name && t.convert(x), new Date(t.year, t.month.index, t.day, t.hour, t.minute, t.second, t.millisecond)
+                    return "gregorian" !== g(this, W).name && t.convert(x), new Date(t.year, t.month.index, t.day, t.hour, t.minute, t.second, t.millisecond)
                 }
             }, {
                 key: "toUTC",
                 value: function() {
-                    return g(this, W) || (this.minute += this.toDate().getTimezoneOffset(), v(this, W, !0)), this
+                    return g(this, T) || (this.minute += this.toDate().getTimezoneOffset(), v(this, T, !0)), this
                 }
             }, {
                 key: "toUnix",
                 value: function() {
                     return this.unix
                 }
             }, {
                 key: "toJulianDay",
                 value: function() {
-                    return this.toDays() + g(this, T).epoch
+                    return this.toDays() + g(this, W).epoch
                 }
             }, {
                 key: "toObject",
                 value: function() {
                     return {
                         year: g(this, P),
                         month: this.month,
@@ -2908,15 +2908,15 @@
                         hour: g(this, E),
                         minute: g(this, C),
                         second: g(this, j),
                         millisecond: g(this, I),
                         weekOfYear: this.weekOfYear,
                         dayOfYear: this.dayOfYear,
                         daysLeft: this.daysLeft,
-                        calendar: g(this, T),
+                        calendar: g(this, W),
                         locale: g(this, A),
                         format: g(this, L) || "YYYY/MM/DD",
                         ignoreList: g(this, z)
                     }
                 }
             }, {
                 key: "toJSON",
@@ -2927,36 +2927,36 @@
                 key: "valueOf",
                 value: function() {
                     return this.toDate().valueOf()
                 }
             }, {
                 key: "toDays",
                 value: function() {
-                    if (this.isValid) return g(this, T).getAllDays(this)
+                    if (this.isValid) return g(this, W).getAllDays(this)
                 }
             }, {
                 key: "dayOfBeginning",
                 get: function() {
                     return this.toDays()
                 }
             }, {
                 key: "dayOfYear",
                 get: function() {
-                    if (this.isValid) return g(this, T).getDayOfYear(this)
+                    if (this.isValid) return g(this, W).getDayOfYear(this)
                 }
             }, {
                 key: "weekOfYear",
                 get: function() {
                     if (this.isValid) return 1 + ~~(this.dayOfYear / 7)
                 }
             }, {
                 key: "daysLeft",
                 get: function() {
                     if (this.isValid) {
-                        var e = g(this, T).yearLength;
+                        var e = g(this, W).yearLength;
                         return (this.isLeap ? e + 1 : e) - this.dayOfYear
                     }
                 }
             }, {
                 key: "year",
                 get: function() {
                     return g(this, P)
@@ -3024,15 +3024,15 @@
                 },
                 set: function(e) {
                     e = O(e), v(this, I, e), S(e, 0, 999) && g(this, B).call(this)
                 }
             }, {
                 key: "months",
                 get: function() {
-                    var e = g(this, T).getMonthLengths(this.isLeap);
+                    var e = g(this, W).getMonthLengths(this.isLeap);
                     return (g(this, R).months || g(this, A).months).map((function(t, r) {
                         var n = d(t, 2);
                         return {
                             name: n[0],
                             shortName: n[1],
                             length: e[r],
                             index: r,
@@ -3068,20 +3068,20 @@
                             return "string" == typeof e
                         }))
                     })) && (g(this, R).weekDays = e)
                 }
             }, {
                 key: "leaps",
                 get: function() {
-                    return g(this, T).getLeaps(g(this, P))
+                    return g(this, W).getLeaps(g(this, P))
                 }
             }, {
                 key: "calendar",
                 get: function() {
-                    return g(this, T)
+                    return g(this, W)
                 },
                 set: function(e) {
                     this.convert(e)
                 }
             }, {
                 key: "locale",
                 get: function() {
@@ -3117,25 +3117,25 @@
                 },
                 set: function(e) {
                     "string" == typeof e && v(this, L, e)
                 }
             }, {
                 key: "isLeap",
                 get: function() {
-                    return g(this, T).isLeap(g(this, P))
+                    return g(this, W).isLeap(g(this, P))
                 }
             }, {
                 key: "isValid",
                 get: function() {
                     return !isNaN(g(this, P)) && !isNaN(g(this, N)) && !isNaN(g(this, Y))
                 }
             }, {
                 key: "isUTC",
                 get: function() {
-                    return g(this, W)
+                    return g(this, T)
                 }
             }, {
                 key: "unix",
                 get: function() {
                     return (this.valueOf() - this.millisecond) / 1e3
                 }
             }, {
@@ -3145,18 +3145,18 @@
                 },
                 set: function(e) {
                     M(e) && v(this, z, e)
                 }
             }, {
                 key: "weekStartDayIndex",
                 get: function() {
-                    return g(this, T).weekStartDayIndex
+                    return g(this, W).weekStartDayIndex
                 },
                 set: function(e) {
-                    void 0 !== (e = O(e)) && (g(this, T).weekStartDayIndex = Math.abs(e) % 7)
+                    void 0 !== (e = O(e)) && (g(this, W).weekStartDayIndex = Math.abs(e) % 7)
                 }
             }, {
                 key: "date",
                 set: function(e) {
                     this.setDate(e)
                 }
             }]) && p(t.prototype, r), Object.defineProperty(t, "prototype", {
@@ -3248,15 +3248,15 @@
 
     function m(e) {
         var t = f(Object(a.useState)(e.value), 2),
             r = t[0],
             n = t[1];
         return Object(a.useEffect)((function() {
             n(e.value)
-        }), [e.value]), o.a.createElement("div", null, "ExampleComponent:", o.a.createElement(u.a, {
+        }), [e.value]), o.a.createElement("div", null, o.a.createElement(u.a, {
             value: r,
             multiple: e.multiple,
             range: e.range,
             onlyMonthPicker: e.onlyMonthPicker,
             onlyYearPicker: e.onlyYearPicker,
             format: e.format,
             formattingIgnoreList: e.formattingIgnoreList,
@@ -3316,23 +3316,71 @@
             offsetX: e.offsetX,
             mobileLabels: e.mobileLabels,
             portal: e.portal,
             portalTarget: e.portalTarget,
             onOpenPickNewDate: e.onOpenPickNewDate,
             mobileButtons: e.mobileButtons,
             onChange: function(t) {
-                n(t), console.log(t), e.setProps({
+                n(t), e.setProps({
                     value: t
                 })
             }
         }))
     }
     var p = m;
     m.defaultProps = {}, m.propTypes = (c(n = {
         id: s.a.string,
-        value: s.a.oneOfType([s.a.instanceOf(Date), s.a.string, s.a.array])
-    }, "value", s.a.oneOfType([s.a.instanceOf(Date), s.a.object, s.a.string, s.a.number, s.a.array])), c(n, "multiple", s.a.bool), c(n, "range", s.a.bool), c(n, "onlyMonthPicker", s.a.bool), c(n, "onlyYearPicker", s.a.bool), c(n, "format", s.a.string), c(n, "formattingIgnoreList", s.a.array), c(n, "calendar", s.a.string), c(n, "locale", s.a.string), c(n, "mapDays", s.a.func), c(n, "onChange", s.a.func), c(n, "className", s.a.string), c(n, "weekDays", s.a.array), c(n, "months", s.a.array), c(n, "showOtherDays", s.a.bool), c(n, "minDate", s.a.oneOfType([s.a.instanceOf(Date), s.a.object, s.a.string, s.a.number])), c(n, "maxDate", s.a.oneOfType([s.a.instanceOf(Date), s.a.object, s.a.string, s.a.number])), c(n, "disableYearPicker", s.a.bool), c(n, "disableMonthPicker", s.a.bool), c(n, "zIndex", s.a.number), c(n, "plugins", s.a.array), c(n, "sort", s.a.bool), c(n, "numberOfMonths", s.a.number), c(n, "currentDate", s.a.object), c(n, "digits", s.a.array), c(n, "buttons", s.a.bool), c(n, "renderButton", s.a.oneOfType([s.a.func, s.a.element])), c(n, "weekStartDayIndex", s.a.number), c(n, "disableDayPicker", s.a.bool), c(n, "onPropsChange", s.a.func), c(n, "onMonthChange", s.a.func), c(n, "onYearChange", s.a.func), c(n, "onFocusedDateChange", s.a.func), c(n, "readOnly", s.a.bool), c(n, "disabled", s.a.bool), c(n, "hideMonth", s.a.bool), c(n, "hideYear", s.a.bool), c(n, "shadow", s.a.bool), c(n, "fullYear", s.a.bool), c(n, "displayWeekNumbers", s.a.bool), c(n, "weekNumber", s.a.string), c(n, "weekPicker", s.a.bool), c(n, "rangeHover", s.a.bool), c(n, "arrow", s.a.oneOfType([s.a.bool, s.a.element])), c(n, "arrowStyle", s.a.object), c(n, "arrowClassName", s.a.string), c(n, "animations", s.a.array), c(n, "inputClass", s.a.string), c(n, "name", s.a.string), c(n, "id", s.a.string), c(n, "title", s.a.string), c(n, "placeholder", s.a.string), c(n, "style", s.a.object), c(n, "render", s.a.oneOfType([s.a.elementType, s.a.func])), c(n, "inputMode", s.a.string), c(n, "scrollSensitive", s.a.bool), c(n, "hideOnScroll", s.a.bool), c(n, "calendarPosition", s.a.string), c(n, "containerStyle", s.a.object), c(n, "containerClassName", s.a.string), c(n, "editable", s.a.bool), c(n, "onlyShowInRangeDates", s.a.bool), c(n, "onOpen", s.a.func), c(n, "onClose", s.a.func), c(n, "fixMainPosition", s.a.bool), c(n, "fixRelativePosition", s.a.bool), c(n, "offsetY", s.a.number), c(n, "offsetX", s.a.number), c(n, "onPositionChange", s.a.func), c(n, "mobileLabels", s.a.object), c(n, "portal", s.a.bool), c(n, "portalTarget", s.a.instanceOf(HTMLElement)), c(n, "onOpenPickNewDate", s.a.bool), c(n, "mobileButtons", s.a.arrayOf(s.a.instanceOf(HTMLButtonElement))), c(n, "setProps", s.a.func), n), r.d(t, "MultiDatePicker", (function() {
+        value: s.a.oneOfType([s.a.instanceOf(Date), s.a.string, s.a.array]),
+        multiple: s.a.bool,
+        range: s.a.bool,
+        onlyMonthPicker: s.a.bool,
+        onlyYearPicker: s.a.bool,
+        format: s.a.string,
+        formattingIgnoreList: s.a.array,
+        calendar: s.a.string,
+        locale: s.a.string,
+        mapDays: s.a.func,
+        onChange: s.a.func,
+        className: s.a.string,
+        weekDays: s.a.array,
+        months: s.a.array,
+        showOtherDays: s.a.bool,
+        minDate: s.a.oneOfType([s.a.instanceOf(Date), s.a.object, s.a.string, s.a.number]),
+        maxDate: s.a.oneOfType([s.a.instanceOf(Date), s.a.object, s.a.string, s.a.number]),
+        disableYearPicker: s.a.bool,
+        disableMonthPicker: s.a.bool,
+        zIndex: s.a.number,
+        plugins: s.a.array,
+        sort: s.a.bool,
+        numberOfMonths: s.a.number,
+        currentDate: s.a.object,
+        digits: s.a.array,
+        buttons: s.a.bool,
+        renderButton: s.a.oneOfType([s.a.func, s.a.element]),
+        weekStartDayIndex: s.a.number,
+        disableDayPicker: s.a.bool,
+        onPropsChange: s.a.func,
+        onMonthChange: s.a.func,
+        onYearChange: s.a.func,
+        onFocusedDateChange: s.a.func,
+        readOnly: s.a.bool,
+        disabled: s.a.bool,
+        hideMonth: s.a.bool,
+        hideYear: s.a.bool,
+        shadow: s.a.bool,
+        fullYear: s.a.bool,
+        displayWeekNumbers: s.a.bool,
+        weekNumber: s.a.string,
+        weekPicker: s.a.bool,
+        rangeHover: s.a.bool,
+        arrow: s.a.oneOfType([s.a.bool, s.a.element]),
+        arrowStyle: s.a.object,
+        arrowClassName: s.a.string,
+        animations: s.a.array,
+        inputClass: s.a.string,
+        name: s.a.string
+    }, "id", s.a.string), c(n, "title", s.a.string), c(n, "placeholder", s.a.string), c(n, "style", s.a.object), c(n, "render", s.a.oneOfType([s.a.elementType, s.a.func])), c(n, "inputMode", s.a.string), c(n, "scrollSensitive", s.a.bool), c(n, "hideOnScroll", s.a.bool), c(n, "calendarPosition", s.a.string), c(n, "containerStyle", s.a.object), c(n, "containerClassName", s.a.string), c(n, "editable", s.a.bool), c(n, "onlyShowInRangeDates", s.a.bool), c(n, "onOpen", s.a.func), c(n, "onClose", s.a.func), c(n, "fixMainPosition", s.a.bool), c(n, "fixRelativePosition", s.a.bool), c(n, "offsetY", s.a.number), c(n, "offsetX", s.a.number), c(n, "onPositionChange", s.a.func), c(n, "mobileLabels", s.a.object), c(n, "portal", s.a.bool), c(n, "portalTarget", s.a.instanceOf(HTMLElement)), c(n, "onOpenPickNewDate", s.a.bool), c(n, "mobileButtons", s.a.arrayOf(s.a.instanceOf(HTMLButtonElement))), c(n, "setProps", s.a.func), n), r.d(t, "MultiDatePicker", (function() {
         return p
     }))
 }]);
 //# sourceMappingURL=multi_date_picker.min.js.map
 //# sourceMappingURL=multi_date_picker.min.js.map
```

### Comparing `multi_date_picker-0.0.1/multi_date_picker/package-info.json` & `multi_date_picker-0.0.2/multi_date_picker/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -44,9 +44,9 @@
         "build:backends": "dash-generate-components ./src/lib/components multi_date_picker -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

### Comparing `multi_date_picker-0.0.1/package.json` & `multi_date_picker-0.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -44,9 +44,9 @@
         "build:backends": "dash-generate-components ./src/lib/components multi_date_picker -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

### Comparing `multi_date_picker-0.0.1/tests/test_usage.py` & `multi_date_picker-0.0.2/tests/test_usage.py`

 * *Files identical despite different names*

