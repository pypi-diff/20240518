# Comparing `tmp/iam_actions-1.2.20240516.tar.gz` & `tmp/iam_actions-1.2.20240517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240516.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240517.tar", max compression
```

## Comparing `iam_actions-1.2.20240516.tar` & `iam_actions-1.2.20240517.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/README.md
--rw-r--r--   0        0        0      228 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/__init__.py
--rw-r--r--   0        0        0  4834343 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/services.py
--rw-r--r--   0        0        0   628769 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/policies.json
--rw-r--r--   0        0        0   209690 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   610102 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-16 02:23:31.766452 iam_actions-1.2.20240516/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240516/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240516/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/README.md
+-rw-r--r--   0        0        0      228 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4837373 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   629260 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/policies.json
+-rw-r--r--   0        0        0   209717 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   610645 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-17 02:22:26.235777 iam_actions-1.2.20240517/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240517/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240517/PKG-INFO
```

### Comparing `iam_actions-1.2.20240516/LICENSE` & `iam_actions-1.2.20240517/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/README.md` & `iam_actions-1.2.20240517/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/actions.json` & `iam_actions-1.2.20240517/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997235315615153%*

 * *Differences: {"'grafana'": "{'UntagResource': {'condition_keys': {delete: [0]}}, "*

 * *              "'CreateWorkspaceServiceAccount': {'access_level': 'Write', 'description': 'Grants "*

 * *              "permission to create service accounts for a workspace', 'resources': "*

 * *              "['workspace']}, 'DeleteWorkspaceServiceAccount': {'access_level': 'Write', "*

 * *              "'description': 'Grants permission to delete service accounts for a workspace', "*

 * *              "'resources': ['workspace']}, 'ListWorkspaceServiceAcco […]*

```diff
@@ -78319,28 +78319,32 @@
             "description": "Grants permission to create API keys for a workspace",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
         "CreateWorkspaceServiceAccount": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateWorkspaceServiceAccount",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create service accounts for a workspace",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "CreateWorkspaceServiceAccountToken": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateWorkspaceServiceAccountToken",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create service account tokens for a workspace",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "DeleteWorkspace": {
             "access_level": "Write",
             "action": "DeleteWorkspace",
             "condition_keys": [],
             "description": "Grants permission to delete a workspace",
             "orphan": false,
@@ -78355,28 +78359,32 @@
             "description": "Grants permission to delete API keys from a workspace",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
         "DeleteWorkspaceServiceAccount": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteWorkspaceServiceAccount",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete service accounts for a workspace",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "DeleteWorkspaceServiceAccountToken": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteWorkspaceServiceAccountToken",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete service account tokens for a workspace",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "DescribeWorkspace": {
             "access_level": "Read",
             "action": "DescribeWorkspace",
             "condition_keys": [],
             "description": "Grants permission to describe a workspace",
             "orphan": false,
@@ -78441,28 +78449,32 @@
             "description": "Grants permission to list all available supported Grafana versions. Optionally, include a workspace to list the versions to which it can be upgraded",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
         "ListWorkspaceServiceAccountTokens": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListWorkspaceServiceAccountTokens",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list service account tokens for a workspace",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "ListWorkspaceServiceAccounts": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListWorkspaceServiceAccounts",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list service accounts for a workspace",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "ListWorkspaces": {
             "access_level": "Read",
             "action": "ListWorkspaces",
             "condition_keys": [],
             "description": "Grants permission to list workspaces",
             "orphan": false,
@@ -78481,15 +78493,14 @@
                 "workspace"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
-                "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags from a workspace",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
@@ -109214,14 +109225,22 @@
             "access_level": "Undocumented",
             "action": "GetDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetDICOMInstance": {
+            "access_level": "Undocumented",
+            "action": "GetDICOMInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetDatastore": {
             "access_level": "Undocumented",
             "action": "GetDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -125596,14 +125615,22 @@
             "access_level": "Read",
             "action": "DescribeIpRestriction",
             "condition_keys": [],
             "description": "Grants permission to describe the IP restrictions for QuickSight account",
             "orphan": false,
             "resources": []
         },
+        "DescribeKeyRegistration": {
+            "access_level": "Undocumented",
+            "action": "DescribeKeyRegistration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeNamespace": {
             "access_level": "Read",
             "action": "DescribeNamespace",
             "condition_keys": [],
             "description": "Grants permission to describe a QuickSight namespace",
             "orphan": false,
             "resources": [
@@ -126621,14 +126648,22 @@
             "access_level": "Write",
             "action": "UpdateIpRestriction",
             "condition_keys": [],
             "description": "Grants permission to update the IP restrictions for QuickSight account",
             "orphan": false,
             "resources": []
         },
+        "UpdateKeyRegistration": {
+            "access_level": "Undocumented",
+            "action": "UpdateKeyRegistration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdatePublicSharingSettings": {
             "access_level": "Write",
             "action": "UpdatePublicSharingSettings",
             "condition_keys": [],
             "description": "Grants permission to enable or disable public sharing on an account",
             "orphan": false,
             "resources": []
@@ -164811,14 +164846,64 @@
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
+    "user-subscriptions": {
+        "CreateClaim": {
+            "access_level": "Undocumented",
+            "action": "CreateClaim",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteClaim": {
+            "access_level": "Undocumented",
+            "action": "DeleteClaim",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListApplicationClaims": {
+            "access_level": "Undocumented",
+            "action": "ListApplicationClaims",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListClaims": {
+            "access_level": "Undocumented",
+            "action": "ListClaims",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListUserSubscriptions": {
+            "access_level": "Undocumented",
+            "action": "ListUserSubscriptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateClaim": {
+            "access_level": "Undocumented",
+            "action": "UpdateClaim",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "vendor-insights": {
         "ActivateSecurityProfile": {
             "access_level": "Write",
             "action": "ActivateSecurityProfile",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -169295,14 +169380,22 @@
             "access_level": "Undocumented",
             "action": "CreateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "CreateContentAssociation": {
+            "access_level": "Undocumented",
+            "action": "CreateContentAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateKnowledgeBase": {
             "access_level": "Undocumented",
             "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -169343,14 +169436,22 @@
             "access_level": "Undocumented",
             "action": "DeleteContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "DeleteContentAssociation": {
+            "access_level": "Undocumented",
+            "action": "DeleteContentAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteImportJob": {
             "access_level": "Undocumented",
             "action": "DeleteImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -169391,14 +169492,22 @@
             "access_level": "Undocumented",
             "action": "GetContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetContentAssociation": {
+            "access_level": "Undocumented",
+            "action": "GetContentAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetContentSummary": {
             "access_level": "Undocumented",
             "action": "GetContentSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -169455,14 +169564,22 @@
             "access_level": "Undocumented",
             "action": "ListAssistants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListContentAssociations": {
+            "access_level": "Undocumented",
+            "action": "ListContentAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListContents": {
             "access_level": "Undocumented",
             "action": "ListContents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20240516/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240517/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240517/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/generate/generate.py` & `iam_actions-1.2.20240517/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240517/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240517/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/generate/services.py` & `iam_actions-1.2.20240517/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240516/iam_actions/policies.json` & `iam_actions-1.2.20240517/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997547761128445%*

 * *Differences: {"'serviceMap'": "{'Amazon Q in Connect': {'Actions': {insert: [(3, 'CreateContentAssociation'), "*

 * *                 "(10, 'DeleteContentAssociation'), (17, 'GetContentAssociation'), (26, "*

 * *                 "'ListContentAssociations')]}}, 'Amazon QuickSight': {'Actions': {insert: [(83, "*

 * *                 "'DescribeKeyRegistration'), (183, 'UpdateKeyRegistration')]}, 'conditionKeys': "*

 * *                 "{insert: [(7, 'quicksight:KmsKeyArns')]}}, 'AWS HealthImaging': {'Actions': "*

 * *                 "{insert: [( […]*

```diff
@@ -5180,14 +5180,15 @@
             "ARNRegex": "^arn:aws:medical-imaging:.+:.+:.+",
             "Actions": [
                 "CopyImageSet",
                 "CreateDatastore",
                 "DeleteDatastore",
                 "DeleteImageSet",
                 "GetDICOMImportJob",
+                "GetDICOMInstance",
                 "GetDatastore",
                 "GetImageFrame",
                 "GetImageSet",
                 "GetImageSetMetadata",
                 "ListDICOMImportJobs",
                 "ListDatastores",
                 "ListImageSetVersions",
@@ -10495,14 +10496,26 @@
             "StringPrefix": "notifications-contacts",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "AWS User Subscriptions": {
+            "Actions": [
+                "CreateClaim",
+                "DeleteClaim",
+                "ListApplicationClaims",
+                "ListClaims",
+                "ListUserSubscriptions",
+                "UpdateClaim"
+            ],
+            "HasResource": false,
+            "StringPrefix": "user-subscriptions"
+        },
         "AWS Verified Access": {
             "Actions": [
                 "AllowVerifiedAccess"
             ],
             "HasResource": false,
             "StringPrefix": "verified-access"
         },
@@ -18997,34 +19010,38 @@
         "Amazon Q in Connect": {
             "ARNFormat": "arn:aws:wisdom:${Region}:${Account}:${Resource}/${ResourceId}",
             "ARNRegex": "^arn:aws:wisdom:.+:.+:.+",
             "Actions": [
                 "CreateAssistant",
                 "CreateAssistantAssociation",
                 "CreateContent",
+                "CreateContentAssociation",
                 "CreateKnowledgeBase",
                 "CreateQuickResponse",
                 "CreateSession",
                 "DeleteAssistant",
                 "DeleteAssistantAssociation",
                 "DeleteContent",
+                "DeleteContentAssociation",
                 "DeleteImportJob",
                 "DeleteKnowledgeBase",
                 "DeleteQuickResponse",
                 "GetAssistant",
                 "GetAssistantAssociation",
                 "GetContent",
+                "GetContentAssociation",
                 "GetContentSummary",
                 "GetImportJob",
                 "GetKnowledgeBase",
                 "GetQuickResponse",
                 "GetRecommendations",
                 "GetSession",
                 "ListAssistantAssociations",
                 "ListAssistants",
+                "ListContentAssociations",
                 "ListContents",
                 "ListImportJobs",
                 "ListKnowledgeBases",
                 "ListQuickResponses",
                 "ListTagsForResource",
                 "NotifyRecommendationsReceived",
                 "PutFeedback",
@@ -19183,14 +19200,15 @@
                 "DescribeFolderPermissions",
                 "DescribeFolderResolvedPermissions",
                 "DescribeGroup",
                 "DescribeGroupMembership",
                 "DescribeIAMPolicyAssignment",
                 "DescribeIngestion",
                 "DescribeIpRestriction",
+                "DescribeKeyRegistration",
                 "DescribeNamespace",
                 "DescribeRefreshSchedule",
                 "DescribeRoleCustomPermission",
                 "DescribeTemplate",
                 "DescribeTemplateAlias",
                 "DescribeTemplatePermissions",
                 "DescribeTheme",
@@ -19282,14 +19300,15 @@
                 "UpdateEmailCustomizationTemplate",
                 "UpdateFolder",
                 "UpdateFolderPermissions",
                 "UpdateGroup",
                 "UpdateIAMPolicyAssignment",
                 "UpdateIdentityPropagationConfig",
                 "UpdateIpRestriction",
+                "UpdateKeyRegistration",
                 "UpdatePublicSharingSettings",
                 "UpdateRefreshSchedule",
                 "UpdateResourcePermissions",
                 "UpdateRoleCustomPermission",
                 "UpdateSPICECapacityConfiguration",
                 "UpdateTemplate",
                 "UpdateTemplateAlias",
@@ -19309,14 +19328,15 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "quicksight:AllowedEmbeddingDomains",
                 "quicksight:DirectoryType",
                 "quicksight:Edition",
                 "quicksight:IamArn",
+                "quicksight:KmsKeyArns",
                 "quicksight:SessionName",
                 "quicksight:UserName"
             ]
         },
         "Amazon RDS": {
             "ARNFormat": "arn:aws:rds:${Region}:${Account}:${RelativeId}",
             "ARNRegex": "^arn:aws:rds:.+",
```

### Comparing `iam_actions-1.2.20240516/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240517/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974619289340102%*

 * *Differences: {"'user-subscriptions'": 'OrderedDict()'}*

```diff
@@ -6720,14 +6720,15 @@
     "trustedadvisor": {
         "checks": {
             "arn_pattern": "arn:*:trustedadvisor:*:*:checks/*/*",
             "condition_keys": null
         }
     },
     "ts": {},
+    "user-subscriptions": {},
     "vendor-insights": {
         "DataSource": {
             "arn_pattern": "arn:*:vendor-insights:::data-source:*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         },
         "SecurityProfile": {
             "arn_pattern": "arn:*:vendor-insights:::security-profile:*",
```

### Comparing `iam_actions-1.2.20240516/iam_actions/services.json` & `iam_actions-1.2.20240517/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974357299109636%*

 * *Differences: {"'medical-imaging'": "{'Actions': {insert: [(5, 'GetDICOMInstance')]}}",*

 * * "'quicksight'": "{'Actions': {insert: [(83, 'DescribeKeyRegistration'), (183, "*

 * *                 "'UpdateKeyRegistration')]}, 'ConditionKeys': {insert: [(7, "*

 * *                 "'quicksight:KmsKeyArns')]}}",*

 * * "'user-subscriptions'": "OrderedDict([('Actions', ['CreateClaim', 'DeleteClaim', "*

 * *                         "'ListApplicationClaims', 'ListClaims', 'ListUserSubscriptions', "*

 * *                         "'UpdateClaim']), ('ServiceNa […]*

```diff
@@ -15186,14 +15186,15 @@
         ],
         "Actions": [
             "CopyImageSet",
             "CreateDatastore",
             "DeleteDatastore",
             "DeleteImageSet",
             "GetDICOMImportJob",
+            "GetDICOMInstance",
             "GetDatastore",
             "GetImageFrame",
             "GetImageSet",
             "GetImageSetMetadata",
             "ListDICOMImportJobs",
             "ListDatastores",
             "ListImageSetVersions",
@@ -17658,14 +17659,15 @@
             "DescribeFolderPermissions",
             "DescribeFolderResolvedPermissions",
             "DescribeGroup",
             "DescribeGroupMembership",
             "DescribeIAMPolicyAssignment",
             "DescribeIngestion",
             "DescribeIpRestriction",
+            "DescribeKeyRegistration",
             "DescribeNamespace",
             "DescribeRefreshSchedule",
             "DescribeRoleCustomPermission",
             "DescribeTemplate",
             "DescribeTemplateAlias",
             "DescribeTemplatePermissions",
             "DescribeTheme",
@@ -17757,14 +17759,15 @@
             "UpdateEmailCustomizationTemplate",
             "UpdateFolder",
             "UpdateFolderPermissions",
             "UpdateGroup",
             "UpdateIAMPolicyAssignment",
             "UpdateIdentityPropagationConfig",
             "UpdateIpRestriction",
+            "UpdateKeyRegistration",
             "UpdatePublicSharingSettings",
             "UpdateRefreshSchedule",
             "UpdateResourcePermissions",
             "UpdateRoleCustomPermission",
             "UpdateSPICECapacityConfiguration",
             "UpdateTemplate",
             "UpdateTemplateAlias",
@@ -17782,14 +17785,15 @@
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "quicksight:AllowedEmbeddingDomains",
             "quicksight:DirectoryType",
             "quicksight:Edition",
             "quicksight:IamArn",
+            "quicksight:KmsKeyArns",
             "quicksight:SessionName",
             "quicksight:UserName"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon QuickSight"
         ]
@@ -23218,14 +23222,31 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Diagnostic tools"
         ]
     },
+    "user-subscriptions": {
+        "ARNFormats": [],
+        "ARNRegexes": [],
+        "Actions": [
+            "CreateClaim",
+            "DeleteClaim",
+            "ListApplicationClaims",
+            "ListClaims",
+            "ListUserSubscriptions",
+            "UpdateClaim"
+        ],
+        "ConditionKeys": [],
+        "HasResource": false,
+        "ServiceNames": [
+            "AWS User Subscriptions"
+        ]
+    },
     "vendor-insights": {
         "ARNFormats": [
             "arn:aws:vendor-insights:::${ResourceType}:${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:vendor-insights:.+"
         ],
@@ -23880,34 +23901,38 @@
         "ARNRegexes": [
             "^arn:aws:wisdom:.+:.+:.+"
         ],
         "Actions": [
             "CreateAssistant",
             "CreateAssistantAssociation",
             "CreateContent",
+            "CreateContentAssociation",
             "CreateKnowledgeBase",
             "CreateQuickResponse",
             "CreateSession",
             "DeleteAssistant",
             "DeleteAssistantAssociation",
             "DeleteContent",
+            "DeleteContentAssociation",
             "DeleteImportJob",
             "DeleteKnowledgeBase",
             "DeleteQuickResponse",
             "GetAssistant",
             "GetAssistantAssociation",
             "GetContent",
+            "GetContentAssociation",
             "GetContentSummary",
             "GetImportJob",
             "GetKnowledgeBase",
             "GetQuickResponse",
             "GetRecommendations",
             "GetSession",
             "ListAssistantAssociations",
             "ListAssistants",
+            "ListContentAssociations",
             "ListContents",
             "ListImportJobs",
             "ListKnowledgeBases",
             "ListQuickResponses",
             "ListTagsForResource",
             "NotifyRecommendationsReceived",
             "PutFeedback",
```

### Comparing `iam_actions-1.2.20240516/pyproject.toml` & `iam_actions-1.2.20240517/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240516"
+version = "1.2.20240517"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240516/setup.py` & `iam_actions-1.2.20240517/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240516',
+    'version': '1.2.20240517',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240516/PKG-INFO` & `iam_actions-1.2.20240517/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240516
+Version: 1.2.20240517
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

