# Comparing `tmp/asknews-0.6.2-py3-none-any.whl.zip` & `tmp/asknews-0.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 23535 bytes, number of entries: 24
+Zip file size: 23616 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4569 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     8720 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
--rw-r--r--  2.0 unx    13204 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
--rw-r--r--  2.0 unx    10988 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
+-rw-r--r--  2.0 unx    13251 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
+-rw-r--r--  2.0 unx    11113 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    16134 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
 -rw-r--r--  2.0 unx     3805 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     4530 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
--rw-r--r--  2.0 unx      588 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
+-rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
 -rw-r--r--  2.0 unx     6643 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1451 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6339 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5396 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.2.dist-info/RECORD
-24 files, 93825 bytes uncompressed, 20501 bytes compressed:  78.1%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.3.dist-info/RECORD
+24 files, 94005 bytes uncompressed, 20582 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.6.2.dist-info/LICENSE
+Filename: asknews-0.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.6.2.dist-info/METADATA
+Filename: asknews-0.6.3.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.6.2.dist-info/WHEEL
+Filename: asknews-0.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.6.2.dist-info/RECORD
+Filename: asknews-0.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/api/news.py

```diff
@@ -82,16 +82,16 @@
             meaning that the search will only look through the most recent news
             (48 hours)
         :type historical: bool
         :param method: Method to use for searching. 'nl' means Natural Language, which
             is a string that can be any phrase, keyword, question, or paragraph that
             will be used for semantic search on the news. 'kw' means Keyword, which can
             also be any keyword(s), phrase, or paragraph, however the search is a direct
-            keyword search on the database.
-        :type method: Literal["nl", "kw"]
+            keyword search on the database. 'both' uses a hybrid approach.
+        :type method: Literal["nl", "kw", "both"]
         :param similarity_score_threshold: Similarity score threshold, defaults to 0.5
         :type similarity_score_threshold: float
         :param offset: Offset for pagination
         :type offset: int
         :param categories: Categories of news to filter on, defaults to ["All"]
         :type categories: Optional[List[
             Literal[
@@ -186,15 +186,15 @@
         self,
         query: str,
         n_articles: int = 10,
         start_timestamp: Optional[int] = None,
         end_timestamp: Optional[int] = None,
         return_type: Literal["string", "dicts", "both"] = "dicts",
         historical: bool = False,
-        method: Literal["nl", "kw"] = "nl",
+        method: Literal["nl", "kw", "both"] = "nl",
         similarity_score_threshold: float = 0.5,
         offset: int = 0,
         categories: Optional[
             List[
                 Literal[
                     "All",
                     "Business",
```

## asknews_sdk/api/stories.py

```diff
@@ -56,14 +56,15 @@
         limit: int = 50,
         expand_updates: bool = False,
         max_updates: int = 11,
         max_articles: int = 5,
         reddit: int = 0,
         method: Literal["nl", "kw", "both"] = "kw",
         obj_type: Optional[List[Literal["story", "story_update"]]] = None,
+        provocative: Literal["unknown", "low", "medium", "high", "all"] = "all",
     ) -> StoriesResponse:
         """
         Get the news stories.
 
         https://docs.asknews.app/en/reference#get-/v1/stories
 
         :param query: The query.
@@ -113,14 +114,15 @@
                 "obj_type": obj_type if obj_type is not None else ["story"],
                 "reddit": reddit,
                 "limit": limit,
                 "expand_updates": expand_updates,
                 "max_updates": max_updates,
                 "max_articles": max_articles,
                 "uuids": uuids,
+                "provocative": provocative,
             },
             accept=[(StoriesResponse.__content_type__, 1.0)],
         )
 
         return StoriesResponse.model_validate(response.content)
 
     def get_story(
```

## asknews_sdk/dto/sentiment.py

```diff
@@ -6,15 +6,15 @@
 from typing_extensions import Annotated
 
 from asknews_sdk.dto.base import BaseSchema
 
 
 class FinanceResponseTimeSeriesData(BaseModel):
     datetime: Annotated[AwareDatetime, Field(title="Datetime")]
-    value: Annotated[int, Field(title="Value")]
+    value: Annotated[int | float, Field(title="Value")]
 
 
 class FinanceResponseTimeSeries(BaseModel):
     timeseries: Annotated[
         List[FinanceResponseTimeSeriesData], Field(title="Timeseriesdata")
     ]
```

## Comparing `asknews-0.6.2.dist-info/LICENSE` & `asknews-0.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.6.2.dist-info/METADATA` & `asknews-0.6.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python SDK for AskNews
 Home-page: https://github.com/emergentmethods/asknews-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.6.2.dist-info/RECORD` & `asknews-0.6.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 asknews_sdk/__init__.py,sha256=TSiiLJIi3INZrbhvrqaXBSAG4MuX5e-Hz7VQstvTOWM,262
 asknews_sdk/api/__init__.py,sha256=1pNfLO6CSeU2bapA-l_oyUQhW2bgavSQUdQcWqjzwno,415
 asknews_sdk/api/analytics.py,sha256=XrH5U5GYXJ5RRTQNVkWYnL-HOD-6yLm6HmNNVWKczxQ,4569
 asknews_sdk/api/base.py,sha256=6w20VMcj9wuMIZLSy_ajbGbMs-cHWbyN7easFpNb8Cg,203
 asknews_sdk/api/chat.py,sha256=7EbwsFKwwmT8Q-7HanDaWrNO8p1bBt565uBHpAH91ao,8720
-asknews_sdk/api/news.py,sha256=G-YKgFrXgRRNEmy0YaYVUfVrYbcQVRsQl5B1tPn5NNk,13204
-asknews_sdk/api/stories.py,sha256=GG_1lJ4S5EoSPO6HRJQIFWXZWSsu54WXKgqufBXz_TU,10988
+asknews_sdk/api/news.py,sha256=rZN3HyD5-KBt_dQ9KjluVN3vMUq43EpU_7EgpnYa8v4,13251
+asknews_sdk/api/stories.py,sha256=hRox9EzQfaXyaYHnj-rASBludwpRRxhb2Re6-mhvFFw,11113
 asknews_sdk/client.py,sha256=A7irft6UAXEIA8OTC2-EOfp7HSREiT09WAZ7g53iAVM,16134
 asknews_sdk/dto/__init__.py,sha256=dECq34FclMMDeF8Fq62TTngjillmysK8yht2DTOdqHM,677
 asknews_sdk/dto/base.py,sha256=F5rtwwAcuDbCYY1MF0i06IbasIVhZTWzHWoMp4t7f-Y,3805
 asknews_sdk/dto/chat.py,sha256=U76lXLM27LXAxGeMFzbBp9rr5Wi5epXr3H6-2jyZhfc,4530
 asknews_sdk/dto/error.py,sha256=fAJutRBtFzSLcJuZYgTDZtv7-T3p6WBGqk3ky3K481c,674
 asknews_sdk/dto/news.py,sha256=aq9H-lU3LOPbTgPXT_j_7HlCHx-y1aNdPuwD9a6icVo,1296
-asknews_sdk/dto/sentiment.py,sha256=ZK0ArKptbbu7WScZWxavZrONDb5l2o9jlPdrCBF5epg,588
+asknews_sdk/dto/sentiment.py,sha256=8UhtmYw9jxwcZ1aw9300g-UE0WEIdo5JmgWbPLR-58w,596
 asknews_sdk/dto/stories.py,sha256=H0TTy1t52NOkTP4mLB1bcDgibPh76_bDhOWV7UCtVw8,6643
 asknews_sdk/errors.py,sha256=2J6fihHeAL1ny7bdGAoEOazaRibosU3N4IFDBlO9vHk,1451
 asknews_sdk/sdk.py,sha256=EMQeZLuPeAWlV8yLbiefY_C7UuG-1pFDp7GwKJ0rsn4,6339
 asknews_sdk/security.py,sha256=mXVyc4_5KE2j-t5fS3IKewUfmCJZLCPbfcXMJJpLzIk,5396
 asknews_sdk/utils.py,sha256=tM7ga0MZGDA4YheH4dyZ6xxVVexMkzTMz0f6ttP6pwU,1614
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.6.2.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.6.2.dist-info/METADATA,sha256=jx-ASxXi2jtlvWiTSqrr35bui93SfayAfkbrNXnfZ3Y,3233
-asknews-0.6.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.6.2.dist-info/RECORD,,
+asknews-0.6.3.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.6.3.dist-info/METADATA,sha256=6l5kdClZgTPLLT_OJskZCbRtrhwp00oDt4FdcVGxYK4,3233
+asknews-0.6.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.6.3.dist-info/RECORD,,
```

