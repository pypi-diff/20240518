# Comparing `tmp/ifctester-0.0.240423.tar.gz` & `tmp/ifctester-0.0.240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.240423.tar", last modified: Tue Apr 23 09:49:55 2024, max compression
+gzip compressed data, was "ifctester-0.0.240518.tar", last modified: Sat May 18 01:17:43 2024, max compression
```

## Comparing `ifctester-0.0.240423.tar` & `ifctester-0.0.240518.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.079672 ifctester-0.0.240423/
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 09:49:55.079672 ifctester-0.0.240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 09:49:47.000000 ifctester-0.0.240423/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.075672 ifctester-0.0.240423/ifctester/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49995 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/ids.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    21793 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.075672 ifctester-0.0.240423/ifctester/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.079672 ifctester-0.0.240423/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-23 09:49:52.000000 ifctester-0.0.240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:49:55.079672 ifctester-0.0.240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.075672 ifctester-0.0.240423/test/
--rw-r--r--   0 runner    (1001) docker     (127)    89195 2024-04-23 09:49:47.000000 ifctester-0.0.240423/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-04-23 09:49:47.000000 ifctester-0.0.240423/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:17:43.316141 ifctester-0.0.240518/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 01:17:43.316141 ifctester-0.0.240518/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-18 01:17:39.000000 ifctester-0.0.240518/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:17:43.312141 ifctester-0.0.240518/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/ids.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    28224 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:17:43.316141 ifctester-0.0.240518/ifctester/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-05-18 01:17:39.000000 ifctester-0.0.240518/ifctester/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:17:43.316141 ifctester-0.0.240518/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 01:17:43.000000 ifctester-0.0.240518/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-18 01:17:43.000000 ifctester-0.0.240518/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:17:43.000000 ifctester-0.0.240518/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-18 01:17:43.000000 ifctester-0.0.240518/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 01:17:43.000000 ifctester-0.0.240518/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-18 01:17:41.000000 ifctester-0.0.240518/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:17:43.316141 ifctester-0.0.240518/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:17:43.316141 ifctester-0.0.240518/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    89220 2024-05-18 01:17:39.000000 ifctester-0.0.240518/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-05-18 01:17:39.000000 ifctester-0.0.240518/test/test_ids.py
```

### Comparing `ifctester-0.0.240423/PKG-INFO` & `ifctester-0.0.240518/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.240423
+Version: 0.0.240518
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifctester-0.0.240423/README.md` & `ifctester-0.0.240518/README.md`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240423/ifctester/__init__.py` & `ifctester-0.0.240518/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240423/ifctester/__main__.py` & `ifctester-0.0.240518/ifctester/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,48 +22,50 @@
 import argparse
 import ifcopenshell
 from . import ids
 from . import reporter
 
 parser = argparse.ArgumentParser(description="Uses an IDS to audit an IFC")
 parser.add_argument("ids", type=str, help="Path to an IDS")
-parser.add_argument("ifc", type=str, help="Path to an IFC")
+parser.add_argument("ifc", type=str, help="Path to an IFC", nargs="?")
 parser.add_argument(
     "-r", "--reporter", type=str, help="The reporting method to view audit results", default="Console"
 )
 parser.add_argument(
     "--no-color", help="Disable colour output (supported by Console reporting)", action="store_true"
 )
 parser.add_argument(
     "--excel-safe", help="Make sure exported ODS is safely exported for Excel", action="store_true"
 )
 parser.add_argument(
     "-o", "--output", help="Output file (supported for all types of reporting except Console)"
 )
 args = parser.parse_args()
 
-start = time.time()
 specs = ids.open(args.ids)
-ifc = ifcopenshell.open(args.ifc)
-print("Finished loading:", time.time() - start)
-start = time.time()
-specs.validate(ifc)
-print("Finished validating:", time.time() - start)
-start = time.time()
+if args.ifc:
+    start = time.time()
+    ifc = ifcopenshell.open(args.ifc)
+    print("Finished loading:", time.time() - start)
+    start = time.time()
+    specs.validate(ifc)
+    print("Finished validating:", time.time() - start)
 
 if args.reporter == "Console":
     engine = reporter.Console(specs, use_colour=not args.no_color)
 elif args.reporter == "Txt":
     engine = reporter.Txt(specs)
 elif args.reporter == "Json":
     engine = reporter.Json(specs)
 elif args.reporter == "Html":
     engine = reporter.Html(specs)
 elif args.reporter == "Ods":
     engine = reporter.Ods(specs, excel_safe=args.excel_safe)
+elif args.reporter == "OdsSummary":
+    engine = reporter.OdsSummary(specs, excel_safe=args.excel_safe)
 elif args.reporter == "Bcf":
     engine = reporter.Bcf(specs)
 
 engine.report()
 
 if args.output:
     engine.to_file(args.output)
```

### Comparing `ifctester-0.0.240423/ifctester/facet.py` & `ifctester-0.0.240518/ifctester/facet.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,18 @@
             elif isinstance(value, dict) and "restriction" in value.keys():
                 setattr(self, name, Restriction().parse(value["restriction"]))
             else:
                 setattr(self, name, value)
         return self
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: list[ifcopenshell.entity_instance]
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]]
     ) -> list[ifcopenshell.entity_instance]:
+        if not elements:
+            return []
         return [e for e in elements if self(e)]
 
     def to_string(
         self,
         clause_type: str,
         specification: Optional[Specification] = None,
         requirement: Optional[Facet] = None,
@@ -129,14 +131,15 @@
                 value = getattr(self, key)
                 key_variable = "{" + key + "}"
                 if value is not None and key_variable in template:
                     template = template.replace(key_variable, str(value))
                     total_replacements += 1
                 if total_replacements == total_variables:
                     return template
+        return "This facet cannot be interpreted"
 
     def to_ids_value(self, parameter: Union[str, Restriction, list]) -> dict[str, Any]:
         if isinstance(parameter, str):
             parameter_dict = {"simpleValue": parameter}
         elif isinstance(parameter, Restriction):
             parameter_dict = {"xs:restriction": [parameter.asdict()]}
         elif isinstance(parameter, list):
```

### Comparing `ifctester-0.0.240423/ifctester/ids.py` & `ifctester-0.0.240518/ifctester/ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
         description=None,
         author=None,
         date=None,
         purpose=None,
         milestone=None,
     ):
         # Not part of the IDS spec, but very useful in practice
-        self.filepath = None
-        self.filename = None
+        self.filepath: Optional[str] = None
+        self.filename: Optional[str] = None
 
         self.specifications: List[Specification] = []
         self.info = {}
         self.info["title"] = title or "Untitled"
         if copyright:
             self.info["copyright"] = copyright
         if version:
@@ -170,14 +170,15 @@
         self.maxOccurs: Union[int, str] = maxOccurs
         self.ifcVersion = ifcVersion
         self.identifier = identifier
         self.description = description
         self.instructions = instructions
 
         self.applicable_entities: list[ifcopenshell.entity_instance] = []
+        self.failed_entities: set[ifcopenshell.entity_instance] = set()
         self.status = None
 
     def asdict(self):
         results = {
             "@name": self.name,
             "@ifcVersion": self.ifcVersion,
             "applicability": {},
@@ -295,14 +296,15 @@
     def get_usage(self) -> Cardinality:
         if self.minOccurs != 0:
             return "required"
         elif self.minOccurs == 0 and self.maxOccurs != 0:
             return "optional"
         elif self.maxOccurs == 0:
             return "prohibited"
+        return "required"  # Fallback
 
     def set_usage(self, usage: Cardinality) -> None:
         if usage == "optional":
             self.minOccurs = 0
             self.maxOccurs = "unbounded"
         elif usage == "prohibited":
             self.minOccurs = 0
```

### Comparing `ifctester-0.0.240423/ifctester/ids.xsd` & `ifctester-0.0.240518/ifctester/ids.xsd`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240423/ifctester/reporter.py` & `ifctester-0.0.240518/ifctester/reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,14 +87,17 @@
     percent_checks_pass: ResultsPercent
     required: bool
     applicability: list[str]
     requirements: list[ResultsRequirement]
 
 
 class ResultsRequirement(TypedDict):
+    facet_type: str
+    label: str
+    value: str
     description: str
     status: bool
     failed_entities: list[ResultsFailedEntity]
     total_applicable: int
     total_pass: int
     total_fail: int
     percent_pass: ResultsPercent
@@ -287,16 +290,56 @@
         requirements = []
         for requirement in specification.requirements:
             total_fail = len(requirement.failures)
             total_pass = total_applicable - total_fail
             percent_pass = math.floor((total_pass / total_applicable) * 100) if total_applicable else "N/A"
             total_checks += total_applicable
             total_checks_pass += total_pass
+            facet_type = type(requirement).__name__
+            value = ""
+            if facet_type == "Entity":
+                if requirement.predefinedType:
+                    label = "IFC Class / Predefined Type"
+                    value = f"{requirement.name}.{requirement.predefinedType}"
+                else:
+                    label = "IFC Class"
+                    value = requirement.name
+            elif facet_type == "Attribute":
+                label = requirement.name
+                if requirement.value:
+                    value = requirement.value
+            elif facet_type == "Classification":
+                if requirement.system and requirement.value:
+                    label = "System / Reference"
+                    value = f"{requirement.system} / {requirement.value}"
+                elif requirement.system:
+                    label = "System"
+                    value = requirement.system
+                elif requirement.value:
+                    label = "Reference"
+                    value = requirement.value
+            elif facet_type == "PartOf":
+                label = requirement.relation
+                if requirement.predefinedType:
+                    value = f"{requirement.name}.{requirement.predefinedType}"
+                else:
+                    value = requirement.name
+            elif facet_type == "Property":
+                label = f"{requirement.propertySet}.{requirement.baseName}"
+                if requirement.value:
+                    value = requirement.value
+            elif facet_type == "Material":
+                label = "Name / Category"
+                if requirement.value:
+                    value = requirement.value
             requirements.append(
                 ResultsRequirement(
+                    facet_type=facet_type,
+                    label=label,
+                    value=value,
                     description=requirement.to_string("requirement", specification, requirement),
                     status=requirement.status,
                     failed_entities=self.report_failed_entities(requirement),
                     total_applicable=total_applicable,
                     total_pass=total_pass,
                     total_fail=total_fail,
                     percent_pass=percent_pass,
@@ -497,14 +540,136 @@
             for requirement in specification["requirements"]:
                 if requirement["status"]:
                     continue
                 for failure in requirement["failed_entities"]:
                     element = failure.get("element", None)
                     element_type = failure.get("element_type", None)
                     row = [
+                        requirement["description"],
+                        failure.get("reason", "No reason provided"),
+                        failure["class"],
+                        failure["predefined_type"],
+                        failure["name"],
+                        failure["description"],
+                        failure["global_id"],
+                        failure["tag"],
+                        str(element) if element else "N/A",
+                        str(element_type) if element_type else "N/A",
+                    ]
+                    tr = TableRow()
+                    c = 0
+                    for col in row:
+                        tc = TableCell(valuetype="string", stylename="t")
+                        if col is None:
+                            col = "NULL"
+                        tc.addElement(P(text=col))
+                        tr.addElement(tc)
+                        c += 1
+                    table.addElement(tr)
+            self.doc.spreadsheet.addElement(table)
+
+        self.doc.save(filepath, addsuffix=not filepath.lower().endswith(".ods"))
+
+
+class OdsSummary(Json):
+    def __init__(self, ids: Ids, excel_safe=False):
+        super().__init__(ids)
+        self.excel_safe = excel_safe
+        self.colours = {
+            "h": "cccccc",  # Header
+            "p": "97cc64",  # Pass
+            "f": "fb5a3e",  # Fail
+            "t": "ffffff",  # Regular text
+        }
+
+    def excel_safe_spreadsheet_name(self, name: str) -> str:
+        if not self.excel_safe:
+            return name
+
+        warning = (
+            f'WARNING. Sheet name "{name}" is not valid for Excel and will be changed. '
+            "See: https://support.microsoft.com/en-us/office/rename-a-worksheet-3f1f7148-ee83-404d-8ef0-9ff99fbad1f9"
+        )
+
+        if not name or name == "History":
+            print(warning)
+            return "placeholder spreadsheet name"
+
+        if name.startswith("'") or name.endswith("'"):
+            print(warning)
+            name = name.strip("'")
+
+        pattern = r"[\\\/\?\*\:\[\]]"
+        if re.search(pattern, name):
+            name = re.sub(pattern, "", name)
+            print(warning)
+
+        if len(name) > 31:
+            name = name[:31]
+            print(warning)
+        return name
+
+    def to_file(self, filepath: str) -> None:
+        from odf.opendocument import OpenDocumentSpreadsheet
+        from odf.style import Style, TableCellProperties
+        from odf.table import Table, TableRow, TableCell
+        from odf.text import P
+
+        self.doc = OpenDocumentSpreadsheet()
+
+        self.cell_formats = {}
+        for key, value in self.colours.items():
+            style = Style(name=key, family="table-cell")
+            style.addElement(TableCellProperties(backgroundcolor="#" + value))
+            self.doc.automaticstyles.addElement(style)
+            self.cell_formats[key] = style
+
+        table = Table(name=self.excel_safe_spreadsheet_name(self.results["title"]))
+        tr = TableRow()
+        for header in ["Specification", "Applicability", "Facet Type", "Data Name", "Value Requirements"]:
+            tc = TableCell(valuetype="string", stylename="h")
+            tc.addElement(P(text=header))
+            tr.addElement(tc)
+        table.addElement(tr)
+
+        rows = []
+        for specification in self.results["specifications"]:
+            applicability = ", ".join(specification["applicability"])
+            for requirement in specification["requirements"]:
+                rows.append(
+                    [
+                        specification["name"],
+                        applicability,
+                        requirement["facet_type"],
+                        requirement["label"],
+                        requirement["value"],
+                    ]
+                )
+
+        for row in rows:
+            tr = TableRow()
+            c = 0
+            for col in row:
+                tc = TableCell(valuetype="string")
+                if col is None:
+                    col = "NULL"
+                tc.addElement(P(text=col))
+                tr.addElement(tc)
+                c += 1
+            table.addElement(tr)
+        self.doc.spreadsheet.addElement(table)
+
+        while False:
+            for requirement in specification["requirements"]:
+                if requirement["status"]:
+                    continue
+                for failure in requirement["failed_entities"]:
+                    element = failure.get("element", None)
+                    element_type = failure.get("element_type", None)
+                    row = [
                         requirement["description"],
                         failure.get("reason", "No reason provided"),
                         failure["class"],
                         failure["predefined_type"],
                         failure["name"],
                         failure["description"],
                         failure["global_id"],
```

### Comparing `ifctester-0.0.240423/ifctester/templates/report.html` & `ifctester-0.0.240518/ifctester/templates/report.html`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240423/ifctester.egg-info/PKG-INFO` & `ifctester-0.0.240518/ifctester.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.240423
+Version: 0.0.240518
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifctester-0.0.240423/pyproject.toml` & `ifctester-0.0.240518/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifctester"
-version = "0.0.240423"
+version = "0.0.240518"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC model auditing tool with support for IDS"
 readme = "README.md"
 keywords = ["IFC", "IDS", "BIM"]
 classifiers = [
```

### Comparing `ifctester-0.0.240423/test/test_facet.py` & `ifctester-0.0.240518/test/test_facet.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcTester.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import uuid
 import ifcopenshell
 import ifcopenshell.api
+import ifcopenshell.guid
 import ifctester.facet
 from ifctester.facet import Entity, Attribute, Classification, Property, PartOf, Material, Restriction
 
 
 def set_facet(facet):
     pass
```

### Comparing `ifctester-0.0.240423/test/test_ids.py` & `ifctester-0.0.240518/test/test_ids.py`

 * *Files identical despite different names*

