# Comparing `tmp/codeinsight_sdk-0.0.8.tar.gz` & `tmp/codeinsight_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinsight_sdk-0.0.8.tar", max compression
+gzip compressed data, was "codeinsight_sdk-0.0.9.tar", max compression
```

## Comparing `codeinsight_sdk-0.0.8.tar` & `codeinsight_sdk-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/LICENSE
--rw-r--r--   0        0        0      895 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/README.md
--rw-r--r--   0        0        0       38 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/__init__.py
--rw-r--r--   0        0        0     3146 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/client.py
--rw-r--r--   0        0        0     1007 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/exceptions.py
--rw-r--r--   0        0        0     1680 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/experimental.py
--rw-r--r--   0        0        0      321 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/handler.py
--rw-r--r--   0        0        0      109 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/__init__.py
--rw-r--r--   0        0        0     1622 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/inventory.py
--rw-r--r--   0        0        0     7508 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/project.py
--rw-r--r--   0        0        0     1302 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/report.py
--rw-r--r--   0        0        0     1757 2024-01-11 02:51:29.291494 codeinsight_sdk-0.0.8/codeinsight_sdk/models.py
--rw-r--r--   0        0        0      870 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/handlers/__init__.py
--rw-r--r--   0        0        0      279 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/resources/test_codebase.zip
--rw-r--r--   0        0        0     9597 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/test_client.py
--rw-r--r--   0        0        0     3512 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/test_experimental.py
--rw-r--r--   0        0        0      291 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/test_handlers.py
--rw-r--r--   0        0        0      929 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/test_models.py
--rw-r--r--   0        0        0     1027 2024-01-11 02:51:29.295494 codeinsight_sdk-0.0.8/tests/test_not_implemented.py
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 codeinsight_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/LICENSE
+-rw-r--r--   0        0        0      895 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0      476 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/__init__.py
+-rw-r--r--   0        0        0     3143 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/client.py
+-rw-r--r--   0        0        0     1016 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/exceptions.py
+-rw-r--r--   0        0        0     1704 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/experimental.py
+-rw-r--r--   0        0        0      203 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/handler.py
+-rw-r--r--   0        0        0      110 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/__init__.py
+-rw-r--r--   0        0        0     1553 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/inventory.py
+-rw-r--r--   0        0        0     7234 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/project.py
+-rw-r--r--   0        0        0     1303 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/report.py
+-rw-r--r--   0        0        0     1796 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/codeinsight_sdk/models.py
+-rw-r--r--   0        0        0      870 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/handlers/__init__.py
+-rw-r--r--   0        0        0      279 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/resources/test_codebase.zip
+-rw-r--r--   0        0        0     9835 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/test_client.py
+-rw-r--r--   0        0        0     3591 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/test_experimental.py
+-rw-r--r--   0        0        0      174 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/test_handlers.py
+-rw-r--r--   0        0        0      846 2024-01-16 18:51:41.069417 codeinsight_sdk-0.0.9/tests/test_models.py
+-rw-r--r--   0        0        0     1017 2024-01-16 18:51:41.073417 codeinsight_sdk-0.0.9/tests/test_not_implemented.py
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 codeinsight_sdk-0.0.9/PKG-INFO
```

### Comparing `codeinsight_sdk-0.0.8/LICENSE` & `codeinsight_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinsight_sdk-0.0.8/README.md` & `codeinsight_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/client.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,105 +4,119 @@
 from .handlers import ProjectHandler, ReportHandler
 from .exceptions import CodeInsightError
 from .experimental import ExperimentalHandler
 from .handlers.inventory import InventoryHandler
 
 logger = logging.getLogger(__name__)
 
+
 class CodeInsightClient:
     """Client for the code insight API."""
 
-    def __init__(self,
-                 base_url: str,
-                 api_token: str,
-                 timeout: int = 60,
-                 verify_ssl: bool = True,
-                 experimental: bool = False
-                 ):
-
+    def __init__(
+        self,
+        base_url: str,
+        api_token: str,
+        timeout: int = 60,
+        verify_ssl: bool = True,
+        experimental: bool = False,
+    ):
         self.base_url = base_url
         self.api_url = f"{base_url}/codeinsight/api"
         self.__api_token = api_token
         self.__api_headers = {
-            'Content-Type': 'application/json',
+            "Content-Type": "application/json",
             "Authorization": "Bearer %s" % self.__api_token,
             "User-Agent": "codeinsight_sdk_python",
         }
         self.__timeout = timeout
         self.__verify_ssl = verify_ssl
         self.experimental_enabled = experimental
 
-    def request(self, method, url_part: str, params: dict = None, body: any = None, data: any = None, content_type: str = None):
+    def request(
+        self,
+        method,
+        url_part: str,
+        params: dict = None,
+        body: any = None,
+        data: any = None,
+        content_type: str = None,
+    ):
         url = f"{self.api_url}/{url_part}"
 
         # Iterate over params and remove any that are None (Empty)
-        if(params):
+        if params:
             for k, v in list(params.items()):
                 if v is None:
                     del params[k]
 
         # Update headers if content_type is specified
         headers = self.__api_headers
         if content_type:
-            headers['Content-Type'] = content_type
+            headers["Content-Type"] = content_type
 
-        response = requests.request(method, url,
-                                     headers=self.__api_headers, params=params, json=body, data=data,
-                                     timeout=self.__timeout, verify=self.__verify_ssl)
+        response = requests.request(
+            method,
+            url,
+            headers=self.__api_headers,
+            params=params,
+            json=body,
+            data=data,
+            timeout=self.__timeout,
+            verify=self.__verify_ssl,
+        )
 
         if not response.ok:
-            logger.error(f"Error: {response.status_code} - {response.reason}", exc_info=True)
+            logger.error(
+                f"Error: {response.status_code} - {response.reason}", exc_info=True
+            )
             logger.error(response.text)
-            raise CodeInsightError(response)   
+            raise CodeInsightError(response)
 
         return response
 
     @property
     def projects(self) -> ProjectHandler:
         return ProjectHandler(self)
-    
+
     @property
     def reports(self) -> ReportHandler:
         return ReportHandler(self)
-    
+
     @property
     def inventories(self):
         return InventoryHandler(self)
-    
+
     @property
     def experimental(self) -> ExperimentalHandler:
         if self.experimental_enabled == False:
             raise CodeInsightError("Experimental API is not enabled for this instance")
-        else:
-            return ExperimentalHandler(self)
-    
-    
+        return ExperimentalHandler(self)
+
     # Coming soon...?
 
-    
     def vulnerabilites(self):
         raise NotImplementedError
-    
+
     def users(self):
         raise NotImplementedError
-    
+
     def licenses(self):
         raise NotImplementedError
-    
+
     def tasks(self):
         raise NotImplementedError
-    
+
     def rules(self):
         raise NotImplementedError
-    
+
     def files(self):
         raise NotImplementedError
-    
+
     def folders(self):
         raise NotImplementedError
-    
+
     def jobs(self):
         raise NotImplementedError
-    
+
     def components(self):
         raise NotImplementedError
-
```

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/exceptions.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-
 import requests
 import json
 
-class GenericError(Exception): #pragma: no cover
+
+class GenericError(Exception):  # pragma: no cover
     """Generic error class, catch-all for most code insight API errors."""
+
     pass
 
-class NotYetImplementedError(Exception): #pragma: no cover
+
+class NotYetImplementedError(Exception):  # pragma: no cover
     """Error class for API features that have not yet been implemented."""
+
     pass
 
+
 class CodeInsightError(GenericError):
     """Error class for code insight API errors."""
+
     def __init__(self, response: requests.Response):
         try:
             resp = response.json()
             self.code = response.status_code
-            self.message = resp['Error: ']
-            self.arguments = resp['Arguments: ']
-            self.error = resp['Key: ']
+            self.message = resp["Error: "]
+            self.arguments = resp["Arguments: "]
+            self.error = resp["Key: "]
             self.add_note(f"Arguments: {self.arguments}")
             super().__init__("Error: %s - %s" % (self.code, self.message))
 
         except KeyError:
             raise ValueError(f"Error parsing response: {resp}")
         except json.decoder.JSONDecodeError:
             raise ValueError(f"Error decoding response: {resp}")
```

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/experimental.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/experimental.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 from .handler import Handler
 from .models import ProjectInventoryItem
 
+
 class ExperimentalHandler(Handler):
     def __init__(self, client):
         super().__init__(client)
-    
+
     def get(self):
         # Do nothing, there is no get for this handler
         pass
-    
-    def get_project_vulnerabilities(self, project_id:int) -> list[ProjectInventoryItem]:
+
+    def get_project_vulnerabilities(
+        self, project_id: int
+    ) -> list[ProjectInventoryItem]:
         """
         Get all vulnerabilities for a project.
-        
+
         Args:
             project_id (int): The project id.
-        
+
         Returns:
             dict: The vulnerabilities.
         """
         # First we get the inventory summary for the project with vulnerability summary
         # Then we iterate over the inventory items and calling the inventory vulnerability endpoint for each item with a vulnerability
-        inventory = self.client.projects.get_inventory_summary(project_id, vulnerabilitySummary=True)
+        inventory = self.client.projects.get_inventory_summary(
+            project_id, vulnerabilitySummary=True
+        )
 
         # Iterate over the inventory items, find which have vulnerabilities.
         item: ProjectInventoryItem
         vuln_items: list(ProjectInventoryItem) = []
         for item in inventory:
             if item.vulnerabilitySummary is None:
                 continue
-            
+
             # If the item has a vulnerability, get the vulnerability details for this item and append it
-            if sum(item.vulnerabilitySummary[0]['CvssV3'].values()) > 0:
-                
-                vul_detail = self.client.inventories.get_inventory_vulnerabilities(item.id)
+            if sum(item.vulnerabilitySummary[0]["CvssV3"].values()) > 0:
+                vul_detail = self.client.inventories.get_inventory_vulnerabilities(
+                    item.id
+                )
                 item.vulnerabilities = vul_detail
                 vuln_items.append(item)
             else:
                 # If the item has no vulnerabilities, skip it
                 continue
 
-        return vuln_items
+        return vuln_items
```

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/inventory.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/inventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from ..models import ProjectInventoryItem, Vulnerability
 from ..handler import Handler
 
+
 class InventoryHandler(Handler):
-    """ Handles operations related to inventories."""
+    """Handles operations related to inventories."""
 
     def __init__(self, client):
         super().__init__(client)
         self.cls = ProjectInventoryItem
-    
+
     def get(self, inventoryId: int) -> list[ProjectInventoryItem]:
         """
         Get an inventory item by id.
 
         Args:
             inventoryId (int): The inventory item id.
 
         Returns:
             ProjectInventoryItem: The inventory item.
         """
         path = f"inventories/{inventoryId}"
         resp = self.client.request("GET", url_part=path)
         inventory = []
-        for inv_item in resp.json()['data']:
+        for inv_item in resp.json()["data"]:
             inventory.append(ProjectInventoryItem.from_dict(inv_item))
         return inventory
-    
-    def get_inventory_vulnerabilities(self, inventoryId: int,
-                                      limit: int = 25,
-                                      offset: int = 1) -> list[Vulnerability]:
+
+    def get_inventory_vulnerabilities(
+        self, inventoryId: int, limit: int = 25, offset: int = 1
+    ) -> list[Vulnerability]:
         """
         Get all vulnerabilities for an inventory item.
 
         Args:
             inventoryId (int): The inventory item id.
 
         Returns:
@@ -40,11 +41,11 @@
         path = f"inventories/{inventoryId}/vulnerabilities"
         params = {"limit": limit, "offset": offset}
         resp = self.client.request("GET", url_part=path, params=params)
 
         # TODO - Iterate pages
 
         inventory_vuls: list(Vulnerability) = []
-        for v in resp.json()['data']:
+        for v in resp.json()["data"]:
             inventory_vuls.append(Vulnerability.from_dict(v))
 
-        return inventory_vuls
+        return inventory_vuls
```

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/project.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,121 @@
 from typing import List
 
 from ..models import Project, ProjectInventory, ProjectInventoryItem
 from ..handler import Handler
 
 from ..exceptions import CodeInsightError
 
+
 class ProjectHandler(Handler):
     def __init__(self, client):
         super().__init__(client)
         self.cls = Project
 
-    def create(self, name:str, description:str = None, folder:str = None,
-               scanProfileName:str = None,
-               owner:str = None,
-               risk:str = None,
-               folderId:int = None,
-               customFields:List[dict] = None,
-               ) -> int:
+    def create(
+        self,
+        name: str,
+        description: str = None,
+        folder: str = None,
+        scanProfileName: str = None,
+        owner: str = None,
+        risk: str = None,
+        folderId: int = None,
+        customFields: List[dict] = None,
+    ) -> int:
         """
         Creates a project.
 
         Args:
             name (str): The name of the project.
             description (str, optional): The description of the project. Defaults to None.
             folder (str, optional): The folder of the project. Defaults to None.
 
         Returns:
             Project: The created project id.
         """
         path = "projects"
-        data = {"name": name,
-                "description": description,
-                "folderName": folder,
-                "scanProfileName": scanProfileName,
-                "owner": owner,
-                "risk": risk,
-                "folderId": folderId,
-                "customFields": customFields}
+        data = {
+            "name": name,
+            "description": description,
+            "folderName": folder,
+            "scanProfileName": scanProfileName,
+            "owner": owner,
+            "risk": risk,
+            "folderId": folderId,
+            "customFields": customFields,
+        }
         resp = self.client.request("POST", url_part=path, body=data)
         try:
-            project_id = resp.json()['data']['id']
+            project_id = resp.json()["data"]["id"]
         except KeyError:
             raise CodeInsightError(resp)
         return project_id
 
-
-    #Note API endpoints switch between projects and project...
+    # Note API endpoints switch between projects and project...
     def all(self) -> List[Project]:
         """
         Retrieves all projects from the server.
 
         Returns:
             A list of Project objects representing all the projects.
         """
 
         path = "projects"
         resp = self.client.request("GET", url_part=path)
         projects = []
-        for project_data in resp.json()['data']:
+        for project_data in resp.json()["data"]:
             projects.append(self.cls.from_dict(project_data))
         return projects
 
-    def get(self, id:int) -> Project:
+    def get(self, id: int) -> Project:
         """
         Retrieves a project by its ID.
 
         Args:
             id (int): The ID of the project requested.
 
         Returns:
             Project: The retrieved project.
         """
         path = f"projects/{id}"
         resp = self.client.request("GET", url_part=path)
-        project_data = resp.json()['data']
+        project_data = resp.json()["data"]
         return self.cls.from_dict(project_data)
 
-    def get_id(self, project_name:str) -> int:
+    def get_id(self, project_name: str) -> int:
         """
         Retrieves the ID of a project based on its name.
 
         Args:
             projectName (str): The name of the project.
 
         Returns:
             int: The ID of the project.
         """
         path = "project/id"
         params = {"projectName": project_name}
         resp = self.client.request("GET", url_part=path, params=params)
         try:
-            project_id = resp.json()['Content: '] # Yes, the key is called 'Content: ' ...
+            project_id = resp.json()[
+                "Content: "
+            ]  # Yes, the key is called 'Content: ' ...
         except KeyError:
             raise CodeInsightError(resp)
         return project_id
 
-    def get_inventory_summary(self, project_id:int,
-                                vulnerabilitySummary : bool = False,
-                                cvssVersion: str = 'ANY',
-                                published: str = 'ALL',
-                                offset:int = 1,
-                                limit:int = 25) -> List[ProjectInventoryItem]:
+    def get_inventory_summary(
+        self,
+        project_id: int,
+        vulnerabilitySummary: bool = False,
+        cvssVersion: str = "ANY",
+        published: str = "ALL",
+        offset: int = 1,
+        limit: int = 25,
+    ) -> List[ProjectInventoryItem]:
         """
         Retrieves the inventory summary for a specific project.
 
         Args:
             project_id (int): The ID of the project.
             vulnerabilitySummary (bool, optional): Flag to include vulnerability summary. Defaults to False.
             cvssVersion (str, optional): The CVSS version to filter vulnerabilities. Defaults to 'ANY'.
@@ -112,80 +123,95 @@
             offset (int, optional): The offset for pagination. Defaults to 1.
             limit (int, optional): The maximum number of items to return. Defaults to 25.
 
         Returns:
             List[ProjectInventoryItem]: A list of ProjectInventoryItem objects representing the inventory summary.
         """
         path = f"projects/{project_id}/inventorySummary"
-        params = {"vulnerabilitySummary": vulnerabilitySummary,
-                "cvssVersion": cvssVersion,
-                "published": published,
-                "offset": offset,
-                "limit": limit         
+        params = {
+            "vulnerabilitySummary": vulnerabilitySummary,
+            "cvssVersion": cvssVersion,
+            "published": published,
+            "offset": offset,
+            "limit": limit,
         }
         resp = self.client.request("GET", url_part=path, params=params)
-        current_page = int(resp.headers['current-page'])
-        number_of_pages = int(resp.headers['number-of-pages'])
-        total_records = int(resp.headers['total-records'])
+        current_page = int(resp.headers["current-page"])
+        number_of_pages = int(resp.headers["number-of-pages"])
+        total_records = int(resp.headers["total-records"])
         inventory = []
-        for inv_item in resp.json()['data']:
+        for inv_item in resp.json()["data"]:
             inventory.append(ProjectInventoryItem.from_dict(inv_item))
-        
+
         # Iterate through all the pages
         if number_of_pages > offset:
-            params.update({"offset": offset+1})
+            params.update({"offset": offset + 1})
             chunk = self.get_inventory_summary(project_id, **params)
             # Only append the inventory records
             inventory.extend(chunk)
         return inventory
-    
-    def get_inventory(self,project_id:int,
-                      skip_vulnerabilities: bool = False,
-                      published:bool = True,
-                      vendor:str = None,
-                      product:str = None,
-                      page_size: int = 100,
-                      page: int = 1,
-                      review_status: str = None,
-                      alerts: str = None,
-                      include_files: bool = True
-                      ) -> ProjectInventory:
+
+    def get_inventory(
+        self,
+        project_id: int,
+        skip_vulnerabilities: bool = False,
+        published: bool = True,
+        vendor: str = None,
+        product: str = None,
+        page_size: int = 100,
+        page: int = 1,
+        review_status: str = None,
+        alerts: str = None,
+        include_files: bool = True,
+    ) -> ProjectInventory:
         path = f"project/inventory/{project_id}"
-        params = {"skipVulnerabilities": skip_vulnerabilities,
-                    "published": published,
-                    "vendor": vendor,
-                    "product": product,
-                    "page": page,
-                    "pageSize": page_size,
-                    "reviewStatus": review_status,
-                    "alerts": alerts,
-                    "includeFiles": include_files}
+        params = {
+            "skipVulnerabilities": skip_vulnerabilities,
+            "published": published,
+            "vendor": vendor,
+            "product": product,
+            "page": page,
+            "pageSize": page_size,
+            "reviewStatus": review_status,
+            "alerts": alerts,
+            "includeFiles": include_files,
+        }
 
         resp = self.client.request("GET", url_part=path, params=params)
         project_inventory = resp.json()
         project = ProjectInventory.from_dict(project_inventory)
 
         # Iterate through all the pages
-        if int(resp.headers['number-of-pages']) > page:
-            chunk = self.get_inventory(project_id, page=page+1)
+        if int(resp.headers["number-of-pages"]) > page:
+            chunk = self.get_inventory(project_id, page=page + 1)
             # Only append the inventory records
             project.inventoryItems.extend(chunk.inventoryItems)
 
         return project
-    
-    def upload_codebase(self, project_id:int,
-                        codebase_path:str,
-                        deleteExistingFileOnServer: bool = False,
-                        expansionLevel: int = 1,
-                        deleteArchiveAfterExpand: bool = False,
-                        archiveDirSuffix: str = None,
-                        ) -> int:
+
+    def upload_codebase(
+        self,
+        project_id: int,
+        codebase_path: str,
+        deleteExistingFileOnServer: bool = False,
+        expansionLevel: int = 1,
+        deleteArchiveAfterExpand: bool = False,
+        archiveDirSuffix: str = None,
+    ) -> int:
         path = "project/uploadProjectCodebase"
-        params = {"projectId": project_id,
-                    "deleteExistingFileOnServer": deleteExistingFileOnServer,
-                    "expansionLevel": expansionLevel,
-                    "deleteArchiveAfterExpand": deleteArchiveAfterExpand,
-                    "archiveDirSuffix": archiveDirSuffix}
-        code_file = {"file": open(codebase_path, 'rb')}
+        params = {
+            "projectId": project_id,
+            "deleteExistingFileOnServer": deleteExistingFileOnServer,
+            "expansionLevel": expansionLevel,
+            "deleteArchiveAfterExpand": deleteArchiveAfterExpand,
+            "archiveDirSuffix": archiveDirSuffix,
+        }
+        code_file = {"file": open(codebase_path, "rb")}
         content_type = "application/octet-stream"
-        resp = self.client.request("POST", url_part=path, params=params, data=code_file,content_type=content_type)
+        resp = self.client.request(
+            "POST",
+            url_part=path,
+            params=params,
+            data=code_file,
+            content_type=content_type,
+        )
         return resp.status_code
```

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/handlers/report.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/handlers/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,38 +18,38 @@
 
     """
 
     def __init__(self, client):
         super().__init__(client)
         self.cls = Report
 
-    def get(self, id:int):
+    def get(self, id: int):
         """
         Retrieves a report by its ID.
 
         Args:
             id (int): The ID of the report to retrieve.
 
         Returns:
             Report: The report object.
 
         """
         path = f"reports/{id}"
         resp = self.client.request("GET", url_part=path)
-        report_data = resp.json()['data']
+        report_data = resp.json()["data"]
         report = self.cls.from_dict(report_data)
         return report
 
     def all(self):
         """
         Retrieves all reports.
 
         Returns:
             list: A list of report objects.
 
         """
         path = "reports"
         resp = self.client.request("GET", url_part=path)
         reports = []
-        for report_data in resp.json()['data']:
+        for report_data in resp.json()["data"]:
             reports.append(self.cls.from_dict(report_data))
         return reports
```

### Comparing `codeinsight_sdk-0.0.8/codeinsight_sdk/models.py` & `codeinsight_sdk-0.0.9/codeinsight_sdk/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=invalid-name
 # Disable invalid name because the API uses camelCase
 
 from dataclasses import dataclass
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 from typing import Any, Optional, List, Dict
 
+
 @dataclass
 class Project(DataClassJsonMixin):
     id: int
     name: str
     status: Optional[str] = None
     owner: Optional[str] = None
     description: Optional[str] = None
@@ -22,43 +23,46 @@
 class Vulnerability(DataClassJsonMixin):
     vulnerabilityId: int
     vulnerabilityName: str
     vulnerabilityDescription: str
     vulnerabilityCvssV3Score: int
     vulnerabilityCvssV3Severity: str
 
+
 @dataclass
 class ProjectInventoryItem(DataClassJsonMixin):
     itemNumber: int
     id: int
     componentName: str
     componentVersionName: str
     name: str
     type: str
     priority: str
     createdBy: str
-    createdOn: str
-    updatedOn: str
+    createdOn: Optional[str] = None
+    updatedOn: Optional[str] = None
     url: Optional[str] = None
     componentUrl: Optional[str] = None
     componentDescription: Optional[str] = None
     vulnerabilities: Optional[List[Vulnerability]] = None
     vulnerabilitySummary: Optional[List[Dict[str, Dict]]] = None
     filePaths: Optional[List[str]] = None
 
-@dataclass_json #Trying this style instead of DataClassJsonMixin
+
+@dataclass_json  # Trying this style instead of DataClassJsonMixin
 @dataclass
-class ProjectInventory():
+class ProjectInventory:
     projectId: int
     inventoryItems: List[ProjectInventoryItem]
 
+
 @dataclass
 class Report(DataClassJsonMixin):
     id: int
     name: str
     path: str
     default: bool
     enabled: bool
     enableProjectPicker: bool
     order: int
     createdDateTime: str
-    updatedDateTime: str
+    updatedDateTime: str
```

### Comparing `codeinsight_sdk-0.0.8/pyproject.toml` & `codeinsight_sdk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeinsight_sdk"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python client for the Revenera Code Insight"
 authors = ["Zachary Karpinski <1206496+zkarpinski@users.noreply.github.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/zkarpinski/codeinsight-sdk-python"
 keywords = ["revenera", "api", "flexera", "code insight","sdk"]
 include = [
```

### Comparing `codeinsight_sdk-0.0.8/tests/test_client.py` & `codeinsight_sdk-0.0.9/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,69 +9,80 @@
 
 logger = logging.getLogger(__name__)
 
 ## CHANGE ME ##
 TEST_URL = "https://api.revenera.com"
 TEST_API_TOKEN = "your_api_token"
 
+
 class TestCodeInsightClient:
     @pytest.fixture
     def client(self):
         return CodeInsightClient(TEST_URL, TEST_API_TOKEN)
-    
+
     def test_client(self, client):
         assert client.base_url == TEST_URL
-    
+
     def test_client_expertimental_disabled(self, client):
         assert client.experimental_enabled == False
 
     def test_endpoint_not_found(self, client):
         with requests_mock.Mocker() as m:
             m.get(f"{TEST_URL}/codeinsight/api/projects", status_code=404)
             with pytest.raises(Exception):
                 client.projects.all()
 
+
 class TestProjectEndpoints:
     @pytest.fixture
     def client(self):
         return CodeInsightClient(TEST_URL, TEST_API_TOKEN)
-    
+
     def test_create_project(self, client):
         project_name = "Test"
         with requests_mock.Mocker() as m:
             m.post(f"{TEST_URL}/codeinsight/api/projects", text='{"data": {"id":1}}')
             project_id = client.projects.create(project_name)
         assert project_id == 1
-   
+
     def test_get_all_projects(self, client):
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/projects", text='{"data": [{"id":1, "name":"Test"}, {"id":2, "name":"Test 2"}]}')
+            m.get(
+                f"{TEST_URL}/codeinsight/api/projects",
+                text='{"data": [{"id":1, "name":"Test"}, {"id":2, "name":"Test 2"}]}',
+            )
             projects = client.projects.all()
         assert len(projects) > 0
 
     def test_get_project_id(self, client):
         project_name = "Test"
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/project/id", text='{ "Content: ": 1 }') # Yes, the key is called 'Content: ' ...
+            m.get(
+                f"{TEST_URL}/codeinsight/api/project/id", text='{ "Content: ": 1 }'
+            )  # Yes, the key is called 'Content: ' ...
             project_id = client.projects.get_id(project_name)
         assert project_id == 1
 
-    def test_get_project_id_invalid(self,client):
+    def test_get_project_id_invalid(self, client):
         project_name = "Invalid_Project"
         fake_response_json = """{ "Arguments: " : ["",""],
             "Key: ": " InvalidProjectNameParm",
             "Error: ": "The project name entered was not found" }
         """
         with requests_mock.Mocker() as m:
-            # Note, the key names end with a colon and space '...: ' 
-            m.get(f"{TEST_URL}/codeinsight/api/project/id", text=fake_response_json, status_code=400)
+            # Note, the key names end with a colon and space '...: '
+            m.get(
+                f"{TEST_URL}/codeinsight/api/project/id",
+                text=fake_response_json,
+                status_code=400,
+            )
             with pytest.raises(CodeInsightError):
                 client.projects.get_id(project_name)
-    
-    def test_get_project(self,client):
+
+    def test_get_project(self, client):
         project_id = 1
         fake_response_json = """ { "data": {
             "id": 1,
             "name": "Test",
             "description": "Test project",
             "createdBy": "Zach",
             "createdOn": "Today",
@@ -92,24 +103,27 @@
                     "Low": 6,
                     "Unknown": 1
                 }
             }
         }}
         """
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/projects/{project_id}", text=fake_response_json)
+            m.get(
+                f"{TEST_URL}/codeinsight/api/projects/{project_id}",
+                text=fake_response_json,
+            )
             project = client.projects.get(project_id)
         assert project.id == 1
         assert project.name == "Test"
         assert project.vulnerabilities["CvssV3"]["Critical"] == 1
         assert project.vulnerabilities["CvssV3"]["High"] == 1
         assert project.vulnerabilities["CvssV2"]["High"] == 2
         assert project.vulnerabilities["CvssV2"]["Unknown"] == 4
 
-    def test_get_project_inventory_multipage(self,client):
+    def test_get_project_inventory_multipage(self, client):
         project_id = 1
         total_pages = 4
         total_records = total_pages * 2
         response_header = {"content-type": "application/json"}
         response_header["current-page"] = "1"
         response_header["number-of-pages"] = str(total_pages)
         response_header["total-records"] = str(total_records)
@@ -117,31 +131,40 @@
         fake_response_json = """
         { "projectId": 1, "inventoryItems": [
             {"itemNumber":1, "id":1234, "name":"Example component","type":"component","priority":"low","createdBy":"Zach","createdOn":"Today","updatedOn":"Tomorrow","componentName":"snakeyaml","componentVersionName":"2.0","vulnerabilities":[{"vulnerabilityId":1,"vulnerabilityName":"CVE-2020-1234","vulnerabilityDescription":"Example vulnerability","vulnerabilityCvssV3Score":9.8,"vulnerabilityCvssV3Severity":"Critical"}]},
             {"itemNumber":2, "id":1235, "name":"Example component 2","type":"component","priority":"low","createdBy":"Zach","createdOn":"Today","updatedOn":"Tomorrow","componentName":"snakeyaml","componentVersionName":"2.0"}
             ]}
         """
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/project/inventory/{project_id}",
-                text=fake_response_json, headers=response_header)
+            m.get(
+                f"{TEST_URL}/codeinsight/api/project/inventory/{project_id}",
+                text=fake_response_json,
+                headers=response_header,
+            )
             project_inventory = client.projects.get_inventory(project_id)
         assert project_inventory.projectId == project_id
         assert len(project_inventory.inventoryItems) == total_records
-        assert project_inventory.inventoryItems[0].vulnerabilities[0].vulnerabilityName == "CVE-2020-1234"
-    
-    def test_upload_codebase(self,client):
+        assert (
+            project_inventory.inventoryItems[0].vulnerabilities[0].vulnerabilityName
+            == "CVE-2020-1234"
+        )
+
+    def test_upload_codebase(self, client):
         project_id = 1
         codebase_path = "tests/resources/test_codebase.zip"
         with requests_mock.Mocker() as m:
-            m.post(f"{TEST_URL}/codeinsight/api/project/uploadProjectCodebase", text='{"data": {"id":1}}')
+            m.post(
+                f"{TEST_URL}/codeinsight/api/project/uploadProjectCodebase",
+                text='{"data": {"id":1}}',
+            )
             resp = client.projects.upload_codebase(project_id, codebase_path)
         assert resp == 200
 
     #### FIX THIS! ####
-    def test_get_project_inventory_summary(self,client):
+    def test_get_project_inventory_summary(self, client):
         project_id = 1
         total_pages = 4
         total_records = total_pages * 2
         response_header = {"content-type": "application/json"}
         response_header["current-page"] = "1"
         response_header["number-of-pages"] = str(total_pages)
         response_header["total-records"] = str(total_records)
@@ -149,49 +172,50 @@
             {
                 "itemNumber": 1,
                 "id": 12345,
                 "name": "Inventory Item 1",
                 "type":"component",
                 "priority":"low",
                 "createdBy":"Zach",
-                "createdOn":"Today",
-                "updatedOn":"Tomorrow",
                 "componentName":"snakeyaml",
                 "componentVersionName":"2.0"
             },
             {
                 "itemNumber": 2,
                 "id": 12346,
                 "name": "Inventory Item 2",
                 "type":"component",
                 "priority":"low",
                 "createdBy":"Zach",
-                "createdOn":"Today",
-                "updatedOn":"Tomorrow",
                 "componentName":"snakeyaml",
                 "componentVersionName":"2.0"
             }
             ]
         }
         """
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/projects/{project_id}/inventorySummary",
-                text=fake_response_json, headers=response_header)
-            project_inventory_summary = client.projects.get_inventory_summary(project_id)
+            m.get(
+                f"{TEST_URL}/codeinsight/api/projects/{project_id}/inventorySummary",
+                text=fake_response_json,
+                headers=response_header,
+            )
+            project_inventory_summary = client.projects.get_inventory_summary(
+                project_id
+            )
 
         assert len(project_inventory_summary) == 8
         assert project_inventory_summary[1].id == 12346
 
 
 class TestReportsEndpoints:
     @pytest.fixture
     def client(self):
         return CodeInsightClient(TEST_URL, TEST_API_TOKEN)
-    
-    def test_get_reports_all(self,client):
+
+    def test_get_reports_all(self, client):
         fake_response_json = """ { "data": [
             {
                 "id": 1,
                 "name": "Report 1",
                 "path": "path/to/report",
                 "default": true,
                 "enabled": true,
@@ -212,22 +236,21 @@
                 "updatedDateTime": "Tomorrow"
             }
             ]
     
         }
         """
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/reports",
-                text=fake_response_json)
+            m.get(f"{TEST_URL}/codeinsight/api/reports", text=fake_response_json)
             reports = client.reports.all()
         assert len(reports) == 2
         assert reports[1].id == 2
         assert reports[1].enabled == False
 
-    def test_get_report(self,client):
+    def test_get_report(self, client):
         report_id = 1
         fake_response_json = """ { "data":
             {
                 "id": 1,
                 "name": "Report 1",
                 "path": "path/to/report",
                 "default": true,
@@ -236,12 +259,14 @@
                 "order": 1,
                 "createdDateTime": "Today",
                 "updatedDateTime": "Tomorrow"
             }
         }
         """
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/reports/{report_id}",
-                text=fake_response_json)
+            m.get(
+                f"{TEST_URL}/codeinsight/api/reports/{report_id}",
+                text=fake_response_json,
+            )
             report = client.reports.get(1)
         assert report.id == 1
-        assert report.enabled == True
+        assert report.enabled == True
```

### Comparing `codeinsight_sdk-0.0.8/tests/test_experimental.py` & `codeinsight_sdk-0.0.9/tests/test_experimental.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pytest
 import logging
 
 import requests_mock
 
 
 from codeinsight_sdk import CodeInsightClient
-from codeinsight_sdk.exceptions import CodeInsightError
 
 logger = logging.getLogger(__name__)
 
 ## CHANGE ME ##
 TEST_URL = "https://api.revenera.com"
 TEST_API_TOKEN = "your_api_token"
 
+
 class TestExperimental:
     @pytest.fixture
     def client(self):
         return CodeInsightClient(TEST_URL, TEST_API_TOKEN, experimental=True)
-    
+
     def test_experimental_enabled(self, client):
         assert client.experimental_enabled == True
-    
+
     def test_get_project_vulnerabilities(self, client):
         project_id = 1
         total_pages = 4
         total_records = total_pages * 2
         response_header = {"content-type": "application/json"}
         response_header["current-page"] = "1"
         response_header["number-of-pages"] = str(total_pages)
@@ -82,15 +82,25 @@
             "vulnerabilityId":123457,
             "vulnerabilityName":"CVE-987-65432",
             "vulnerabilityDescription":"Insecure library 2! Watch out.",
             "vulnerabilityCvssV3Score": 9,
             "vulnerabilityCvssV3Severity":"CRITICAL"} ] }
         """
         with requests_mock.Mocker() as m:
-            m.get(f"{TEST_URL}/codeinsight/api/projects/{project_id}/inventorySummary", 
-                  text=fake_response_json, headers=response_header)
-            m.get(f"{TEST_URL}/codeinsight/api/inventories/12346/vulnerabilities", 
-                  text=mock_resp_vuln, headers=response_header)
-            vulnerable_items = client.experimental.get_project_vulnerabilities(project_id)
+            m.get(
+                f"{TEST_URL}/codeinsight/api/projects/{project_id}/inventorySummary",
+                text=fake_response_json,
+                headers=response_header,
+            )
+            m.get(
+                f"{TEST_URL}/codeinsight/api/inventories/12346/vulnerabilities",
+                text=mock_resp_vuln,
+                headers=response_header,
+            )
+            vulnerable_items = client.experimental.get_project_vulnerabilities(
+                project_id
+            )
         assert len(vulnerable_items) > 0
         assert vulnerable_items[0].vulnerabilities is not None
-        assert vulnerable_items[0].vulnerabilities[1].vulnerabilityName == "CVE-987-65432"
+        assert (
+            vulnerable_items[0].vulnerabilities[1].vulnerabilityName == "CVE-987-65432"
+        )
```

### Comparing `codeinsight_sdk-0.0.8/tests/test_models.py` & `codeinsight_sdk-0.0.9/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import pytest
 
 from codeinsight_sdk.models import Project, Report
 
+
 class TestProject(object):
     @pytest.fixture
     def project(self):
         return Project(id=1, name="Test")
-    
+
     def test_project(self, project):
         assert project.id == 1
         assert project.name == "Test"
         assert isinstance(project, Project)
-    
+
+
 class TestReport(object):
     @pytest.fixture
     def report(self):
-        return Report(id=1,
-                        name="Test",
-                        path="path/to/report",
-                        default=True,
-                        enabled=True,
-                        enableProjectPicker=True,
-                        order=1,
-                        createdDateTime="Today",
-                        updatedDateTime="Tomorrow")
-    
+        return Report(
+            id=1,
+            name="Test",
+            path="path/to/report",
+            default=True,
+            enabled=True,
+            enableProjectPicker=True,
+            order=1,
+            createdDateTime="Today",
+            updatedDateTime="Tomorrow",
+        )
+
     def test_report(self, report):
         assert report.id == 1
         assert report.enabled == True
         assert isinstance(report, Report)
```

### Comparing `codeinsight_sdk-0.0.8/tests/test_not_implemented.py` & `codeinsight_sdk-0.0.9/tests/test_not_implemented.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
 
 from codeinsight_sdk import CodeInsightClient
 
-class TestNotImplemented(object):
 
+class TestNotImplemented(object):
     @pytest.fixture
     def client(self):
-        return CodeInsightClient("","")
+        return CodeInsightClient("", "")
 
-    ## Coming soon features ##    
+    ## Coming soon features ##
     def test_vulnerabilities(self, client):
         with pytest.raises(NotImplementedError):
             client.vulnerabilites()
-    
+
     def test_users(self, client):
         with pytest.raises(NotImplementedError):
             client.users()
-    
+
     def test_licenses(self, client):
         with pytest.raises(NotImplementedError):
             client.licenses()
 
     def test_tasks(self, client):
         with pytest.raises(NotImplementedError):
             client.tasks()
@@ -31,8 +31,8 @@
 
     def test_files(self, client):
         with pytest.raises(NotImplementedError):
             client.files()
 
     def test_folders(self, client):
         with pytest.raises(NotImplementedError):
-            client.folders()
+            client.folders()
```

### Comparing `codeinsight_sdk-0.0.8/PKG-INFO` & `codeinsight_sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeinsight-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python client for the Revenera Code Insight
 Home-page: https://github.com/zkarpinski/codeinsight-sdk-python
 License: Apache-2.0
 Keywords: revenera,api,flexera,code insight,sdk
 Author: Zachary Karpinski
 Author-email: 1206496+zkarpinski@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

