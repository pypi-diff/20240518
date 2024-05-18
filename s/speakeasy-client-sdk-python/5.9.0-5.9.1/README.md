# Comparing `tmp/speakeasy-client-sdk-python-5.9.0.tar.gz` & `tmp/speakeasy-client-sdk-python-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.9.0.tar", last modified: Thu May 16 00:12:44 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.9.1.tar", last modified: Sat May 18 00:15:32 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.9.0.tar` & `speakeasy-client-sdk-python-5.9.1.tar`

### file list

```diff
@@ -1,138 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.654952 speakeasy-client-sdk-python-5.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-16 00:12:44.654952 speakeasy-client-sdk-python-5.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:12:44.654952 speakeasy-client-sdk-python-5.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.634952 speakeasy-client-sdk-python-5.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.638952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.638952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.638952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.638952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.638952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.646952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getchangesreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getlintingreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getrevisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/posttags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/searchworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/uploadreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.654952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/addtags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/featureflag.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/getnamespacesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/getrevisionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/gettagsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/preflightrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/preflighttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/v2descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28973 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.654952 speakeasy-client-sdk-python-5.9.0/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-16 00:12:34.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:12:44.654952 speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-16 00:12:44.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-16 00:12:44.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:12:44.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 00:12:44.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 00:12:44.000000 speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.984112 speakeasy-client-sdk-python-5.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    23387 2024-05-18 00:15:32.984112 speakeasy-client-sdk-python-5.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:15:32.984112 speakeasy-client-sdk-python-5.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.960113 speakeasy-client-sdk-python-5.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.964113 speakeasy-client-sdk-python-5.9.1/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.964113 speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.964113 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.964113 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.964113 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.972113 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getchangesreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getlintingreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getorganizationusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/githubcheckaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/githubconfiguretarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/githubtriggeraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/posttags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/searchworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/uploadreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.980112 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/addtags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/featureflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/getnamespacesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/getrevisionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/gettagsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/githubconfiguretargetrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/githubtriggeractionrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/organizationusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/organizationusageresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/preflightrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/preflighttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/v2descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28973 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.980112 speakeasy-client-sdk-python-5.9.1/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-18 00:15:23.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:15:32.980112 speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23387 2024-05-18 00:15:32.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-18 00:15:32.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:15:32.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 00:15:32.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 00:15:32.000000 speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.9.0/PKG-INFO` & `speakeasy-client-sdk-python-5.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.9.0
+Version: 5.9.1
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -98,16 +98,23 @@
         
         ### [requests](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md)
         
         * [generate_request_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
         * [get_request_from_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
         * [query_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
         
+        ### [github](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md)
+        
+        * [github_check_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md#github_check_access)
+        * [github_configure_target](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md#github_configure_target)
+        * [github_trigger_action](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md#github_trigger_action)
+        
         ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md)
         
+        * [get_organization_usage](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organization_usage) - Get billing usage summary for a particular organization
         * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
         
         ### [reports](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md)
         
         * [get_changes_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_changes_report_signed_url) - Get the signed access url for the change reports for a particular document.
         * [get_linting_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_linting_report_signed_url) - Get the signed access url for the linting reports for a particular document.
         * [upload_report](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#upload_report) - Upload a report.
```

### Comparing `speakeasy-client-sdk-python-5.9.0/README.md` & `speakeasy-client-sdk-python-5.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,16 +91,23 @@
 
 ### [requests](docs/sdks/requests/README.md)
 
 * [generate_request_postman_collection](docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
 * [get_request_from_event_log](docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
 * [query_event_log](docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
 
+### [github](docs/sdks/github/README.md)
+
+* [github_check_access](docs/sdks/github/README.md#github_check_access)
+* [github_configure_target](docs/sdks/github/README.md#github_configure_target)
+* [github_trigger_action](docs/sdks/github/README.md#github_trigger_action)
+
 ### [organizations](docs/sdks/organizations/README.md)
 
+* [get_organization_usage](docs/sdks/organizations/README.md#get_organization_usage) - Get billing usage summary for a particular organization
 * [get_organizations](docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
 
 ### [reports](docs/sdks/reports/README.md)
 
 * [get_changes_report_signed_url](docs/sdks/reports/README.md#get_changes_report_signed_url) - Get the signed access url for the change reports for a particular document.
 * [get_linting_report_signed_url](docs/sdks/reports/README.md#get_linting_report_signed_url) - Get the signed access url for the linting reports for a particular document.
 * [upload_report](docs/sdks/reports/README.md#upload_report) - Upload a report.
```

### Comparing `speakeasy-client-sdk-python-5.9.0/setup.py` & `speakeasy-client-sdk-python-5.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.9.0',
+    version='5.9.1',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/artifacts.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/artifacts.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/auth.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/events.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,38 @@
 from .getblob import *
 from .getchangesreportsignedurl import *
 from .getembedaccesstoken import *
 from .getlintingreportsignedurl import *
 from .getmanifest import *
 from .getnamespaces import *
 from .getorganizations import *
+from .getorganizationusage import *
 from .getrequestfromeventlog import *
 from .getrevisions import *
 from .getschema import *
 from .getschemadiff import *
 from .getschemarevision import *
 from .getschemas import *
 from .gettags import *
 from .getuser import *
 from .getvalidembedaccesstokens import *
 from .getversionmetadata import *
 from .getworkspaceaccess import *
 from .getworkspaceeventsbytarget import *
 from .getworkspacetargets import *
+from .githubcheckaccess import *
+from .githubconfiguretarget import *
+from .githubtriggeraction import *
 from .insertversionmetadata import *
 from .posttags import *
 from .postworkspaceevents import *
 from .preflight import *
 from .queryeventlog import *
 from .registerschema import *
 from .revokeembedaccesstoken import *
 from .searchworkspaceevents import *
 from .uploadreport import *
 from .upsertapi import *
 from .upsertapiendpoint import *
 from .validateapikey import *
 
-__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetBlobRequest","GetBlobResponse","GetChangesReportSignedURLRequest","GetChangesReportSignedURLResponse","GetChangesReportSignedURLSignedAccess","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetLintingReportSignedURLRequest","GetLintingReportSignedURLResponse","GetLintingReportSignedURLSignedAccess","GetManifestRequest","GetManifestResponse","GetNamespacesResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetTagsRequest","GetTagsResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsByTargetGlobals","GetWorkspaceEventsByTargetRequest","GetWorkspaceEventsByTargetResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostTagsRequest","PostTagsResponse","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaFile","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","SearchWorkspaceEventsGlobals","SearchWorkspaceEventsRequest","SearchWorkspaceEventsResponse","UploadReportRequestBody","UploadReportResponse","UploadReportUploadedReport","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
+__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetBlobRequest","GetBlobResponse","GetChangesReportSignedURLRequest","GetChangesReportSignedURLResponse","GetChangesReportSignedURLSignedAccess","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetLintingReportSignedURLRequest","GetLintingReportSignedURLResponse","GetLintingReportSignedURLSignedAccess","GetManifestRequest","GetManifestResponse","GetNamespacesResponse","GetOrganizationUsageResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetTagsRequest","GetTagsResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsByTargetGlobals","GetWorkspaceEventsByTargetRequest","GetWorkspaceEventsByTargetResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","GithubCheckAccessRequest","GithubCheckAccessResponse","GithubConfigureTargetResponse","GithubTriggerActionResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostTagsRequest","PostTagsResponse","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaFile","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","SearchWorkspaceEventsGlobals","SearchWorkspaceEventsRequest","SearchWorkspaceEventsResponse","UploadReportRequestBody","UploadReportResponse","UploadReportUploadedReport","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
```

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getblob.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getblob.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getchangesreportsignedurl.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getchangesreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getlintingreportsignedurl.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getlintingreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getmanifest.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getnamespaces.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getnamespaces.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getrevisions.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getrevisions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/gettags.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getworkspaceeventsbytarget.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getworkspaceeventsbytarget.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/posttags.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/posttags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/preflight.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/preflight.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/searchworkspaceevents.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/searchworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/uploadreport.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/uploadreport.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,22 @@
 from .featureflag import *
 from .filter_ import *
 from .filters import *
 from .generateopenapispecdiff import *
 from .getnamespacesresponse import *
 from .getrevisionsresponse import *
 from .gettagsresponse import *
+from .githubconfiguretargetrequest import *
+from .githubtriggeractionrequest import *
 from .interactiontype import *
 from .manifest import *
 from .namespace import *
 from .organization import *
+from .organizationusage import *
+from .organizationusageresponse import *
 from .preflightrequest import *
 from .preflighttoken import *
 from .report import *
 from .requestmetadata import *
 from .revision import *
 from .schema import *
 from .schemadiff import *
@@ -36,8 +40,8 @@
 from .targetsdk import *
 from .unboundedrequest import *
 from .user import *
 from .v2descriptor import *
 from .versionmetadata import *
 from .versionmetadata_input import *
 
-__all__ = ["API","APIEndpoint","APIEndpointInput","APIInput","APIKeyDetails","AccessDetails","AccessToken","AccessTokenAccountType","AccessTokenUser","AccountType","AddTags","Annotations","BoundedRequest","Claims","CliEvent","EmbedAccessTokenResponse","EmbedToken","FeatureFlag","Filter","Filters","GenerateBumpType","GenerateOpenAPISpecDiff","GetNamespacesResponse","GetRevisionsResponse","GetTagsResponse","InteractionType","Level","Manifest","Namespace","OpenapiDiffBumpType","Organization","OrganizationAccountType","PreflightRequest","PreflightToken","Report","RequestMetadata","Revision","Schema","SchemaDiff","Security","Tag","TargetSDK","Type","UnboundedRequest","User","V2Descriptor","ValueChange","VersionMetadata","VersionMetadataInput","Workspaces"]
+__all__ = ["API","APIEndpoint","APIEndpointInput","APIInput","APIKeyDetails","AccessDetails","AccessToken","AccessTokenAccountType","AccessTokenUser","AccountType","AddTags","Annotations","BoundedRequest","Claims","CliEvent","EmbedAccessTokenResponse","EmbedToken","FeatureFlag","Filter","Filters","GenerateBumpType","GenerateOpenAPISpecDiff","GetNamespacesResponse","GetRevisionsResponse","GetTagsResponse","GithubConfigureTargetRequest","GithubTriggerActionRequest","InteractionType","Level","Manifest","Namespace","OpenapiDiffBumpType","Organization","OrganizationAccountType","OrganizationUsage","OrganizationUsageResponse","PreflightRequest","PreflightToken","Report","RequestMetadata","Revision","Schema","SchemaDiff","Security","Tag","TargetSDK","Type","UnboundedRequest","User","V2Descriptor","ValueChange","VersionMetadata","VersionMetadataInput","Workspaces"]
```

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/addtags.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/addtags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/annotations.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/annotations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/featureflag.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/featureflag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/getrevisionsresponse.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/getrevisionsresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/manifest.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/manifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/namespace.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/namespace.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/preflighttoken.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/preflighttoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/report.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/report.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/revision.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/revision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/tag.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/tag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/v2descriptor.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/v2descriptor.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/reports.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/reports.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests as requests_http
 from .apiendpoints import APIEndpoints
 from .apis import Apis
 from .artifacts import Artifacts
 from .auth import Auth
 from .embeds import Embeds
 from .events import Events
+from .github import Github
 from .metadata import Metadata
 from .organizations import Organizations
 from .reports import Reports
 from .requests import Requests
 from .schemas import Schemas
 from .sdkconfiguration import SDKConfiguration
 from .utils.retries import RetryConfig
@@ -32,14 +33,15 @@
     schemas: Schemas
     r"""REST APIs for managing Schema entities"""
     artifacts: Artifacts
     auth: Auth
     r"""REST APIs for managing Authentication"""
     requests: Requests
     r"""REST APIs for retrieving request information"""
+    github: Github
     organizations: Organizations
     reports: Reports
     r"""REST APIs for managing reports"""
     embeds: Embeds
     r"""REST APIs for managing embeds"""
     events: Events
     r"""REST APIs for capturing event data"""
@@ -109,11 +111,12 @@
         self.apis = Apis(self.sdk_configuration)
         self.api_endpoints = APIEndpoints(self.sdk_configuration)
         self.metadata = Metadata(self.sdk_configuration)
         self.schemas = Schemas(self.sdk_configuration)
         self.artifacts = Artifacts(self.sdk_configuration)
         self.auth = Auth(self.sdk_configuration)
         self.requests = Requests(self.sdk_configuration)
+        self.github = Github(self.sdk_configuration)
         self.organizations = Organizations(self.sdk_configuration)
         self.reports = Reports(self.sdk_configuration)
         self.embeds = Embeds(self.sdk_configuration)
         self.events = Events(self.sdk_configuration)
```

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     language: str = 'python'
     openapi_doc_version: str = '0.4.0 .'
-    sdk_version: str = '5.9.0'
-    gen_version: str = '2.332.4'
-    user_agent: str = 'speakeasy-sdk/python 5.9.0 2.332.4 0.4.0 . speakeasy-client-sdk-python'
+    sdk_version: str = '5.9.1'
+    gen_version: str = '2.333.3'
+    user_agent: str = 'speakeasy-sdk/python 5.9.1 2.333.3 0.4.0 . speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.9.0
+Version: 5.9.1
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -98,16 +98,23 @@
         
         ### [requests](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md)
         
         * [generate_request_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
         * [get_request_from_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
         * [query_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
         
+        ### [github](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md)
+        
+        * [github_check_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md#github_check_access)
+        * [github_configure_target](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md#github_configure_target)
+        * [github_trigger_action](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/github/README.md#github_trigger_action)
+        
         ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md)
         
+        * [get_organization_usage](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organization_usage) - Get billing usage summary for a particular organization
         * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
         
         ### [reports](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md)
         
         * [get_changes_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_changes_report_signed_url) - Get the signed access url for the change reports for a particular document.
         * [get_linting_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_linting_report_signed_url) - Get the signed access url for the linting reports for a particular document.
         * [upload_report](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#upload_report) - Upload a report.
```

### Comparing `speakeasy-client-sdk-python-5.9.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.9.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/speakeasy/__init__.py
 src/speakeasy/apiendpoints.py
 src/speakeasy/apis.py
 src/speakeasy/artifacts.py
 src/speakeasy/auth.py
 src/speakeasy/embeds.py
 src/speakeasy/events.py
+src/speakeasy/github.py
 src/speakeasy/metadata.py
 src/speakeasy/organizations.py
 src/speakeasy/reports.py
 src/speakeasy/requests.py
 src/speakeasy/schemas.py
 src/speakeasy/sdk.py
 src/speakeasy/sdkconfiguration.py
@@ -46,27 +47,31 @@
 src/speakeasy/models/operations/getblob.py
 src/speakeasy/models/operations/getchangesreportsignedurl.py
 src/speakeasy/models/operations/getembedaccesstoken.py
 src/speakeasy/models/operations/getlintingreportsignedurl.py
 src/speakeasy/models/operations/getmanifest.py
 src/speakeasy/models/operations/getnamespaces.py
 src/speakeasy/models/operations/getorganizations.py
+src/speakeasy/models/operations/getorganizationusage.py
 src/speakeasy/models/operations/getrequestfromeventlog.py
 src/speakeasy/models/operations/getrevisions.py
 src/speakeasy/models/operations/getschema.py
 src/speakeasy/models/operations/getschemadiff.py
 src/speakeasy/models/operations/getschemarevision.py
 src/speakeasy/models/operations/getschemas.py
 src/speakeasy/models/operations/gettags.py
 src/speakeasy/models/operations/getuser.py
 src/speakeasy/models/operations/getvalidembedaccesstokens.py
 src/speakeasy/models/operations/getversionmetadata.py
 src/speakeasy/models/operations/getworkspaceaccess.py
 src/speakeasy/models/operations/getworkspaceeventsbytarget.py
 src/speakeasy/models/operations/getworkspacetargets.py
+src/speakeasy/models/operations/githubcheckaccess.py
+src/speakeasy/models/operations/githubconfiguretarget.py
+src/speakeasy/models/operations/githubtriggeraction.py
 src/speakeasy/models/operations/insertversionmetadata.py
 src/speakeasy/models/operations/posttags.py
 src/speakeasy/models/operations/postworkspaceevents.py
 src/speakeasy/models/operations/preflight.py
 src/speakeasy/models/operations/queryeventlog.py
 src/speakeasy/models/operations/registerschema.py
 src/speakeasy/models/operations/revokeembedaccesstoken.py
@@ -92,18 +97,22 @@
 src/speakeasy/models/shared/featureflag.py
 src/speakeasy/models/shared/filter_.py
 src/speakeasy/models/shared/filters.py
 src/speakeasy/models/shared/generateopenapispecdiff.py
 src/speakeasy/models/shared/getnamespacesresponse.py
 src/speakeasy/models/shared/getrevisionsresponse.py
 src/speakeasy/models/shared/gettagsresponse.py
+src/speakeasy/models/shared/githubconfiguretargetrequest.py
+src/speakeasy/models/shared/githubtriggeractionrequest.py
 src/speakeasy/models/shared/interactiontype.py
 src/speakeasy/models/shared/manifest.py
 src/speakeasy/models/shared/namespace.py
 src/speakeasy/models/shared/organization.py
+src/speakeasy/models/shared/organizationusage.py
+src/speakeasy/models/shared/organizationusageresponse.py
 src/speakeasy/models/shared/preflightrequest.py
 src/speakeasy/models/shared/preflighttoken.py
 src/speakeasy/models/shared/report.py
 src/speakeasy/models/shared/requestmetadata.py
 src/speakeasy/models/shared/revision.py
 src/speakeasy/models/shared/schema.py
 src/speakeasy/models/shared/schemadiff.py
```

