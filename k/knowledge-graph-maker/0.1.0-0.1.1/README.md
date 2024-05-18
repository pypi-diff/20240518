# Comparing `tmp/knowledge_graph_maker-0.1.0.tar.gz` & `tmp/knowledge_graph_maker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge_graph_maker-0.1.0.tar", max compression
+gzip compressed data, was "knowledge_graph_maker-0.1.1.tar", max compression
```

## Comparing `knowledge_graph_maker-0.1.0.tar` & `knowledge_graph_maker-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-05-01 08:08:04.561957 knowledge_graph_maker-0.1.0/LICENSE
--rw-r--r--   0        0        0     6703 2024-05-18 05:36:37.493802 knowledge_graph_maker-0.1.0/README.md
--rw-r--r--   0        0        0      244 2024-05-18 05:36:37.494471 knowledge_graph_maker-0.1.0/knowledge_graph_maker/__init__.py
--rw-r--r--   0        0        0     6457 2024-05-18 05:36:37.494857 knowledge_graph_maker-0.1.0/knowledge_graph_maker/graph_maker.py
--rw-r--r--   0        0        0      257 2024-05-01 07:29:51.195238 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1768 2024-05-01 07:50:57.377849 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc
--rw-r--r--   0        0        0     1657 2024-05-18 05:36:37.495037 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc
--rw-r--r--   0        0        0     1822 2024-05-18 05:36:37.495201 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2024-05-18 07:21:08.395043 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc
--rw-r--r--   0        0        0     1715 2024-05-01 07:29:51.195530 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/groq_client.py
--rw-r--r--   0        0        0     1009 2024-05-18 05:36:37.495488 knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/openai_client.py
--rw-r--r--   0        0        0     3908 2024-05-01 07:29:51.193626 knowledge_graph_maker-0.1.0/knowledge_graph_maker/logger.py
--rw-r--r--   0        0        0     2093 2024-05-04 14:44:32.548460 knowledge_graph_maker-0.1.0/knowledge_graph_maker/neo4j_graph_model.py
--rw-r--r--   0        0        0      938 2024-05-04 14:44:32.548639 knowledge_graph_maker-0.1.0/knowledge_graph_maker/types.py
--rw-r--r--   0        0        0      694 2024-05-18 12:04:34.577827 knowledge_graph_maker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7843 1970-01-01 00:00:00.000000 knowledge_graph_maker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 08:08:04.561957 knowledge_graph_maker-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7551 2024-05-18 12:56:15.664626 knowledge_graph_maker-0.1.1/README.md
+-rw-r--r--   0        0        0      244 2024-05-18 05:36:37.494471 knowledge_graph_maker-0.1.1/knowledge_graph_maker/__init__.py
+-rw-r--r--   0        0        0     6457 2024-05-18 05:36:37.494857 knowledge_graph_maker-0.1.1/knowledge_graph_maker/graph_maker.py
+-rw-r--r--   0        0        0      257 2024-05-01 07:29:51.195238 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1768 2024-05-01 07:50:57.377849 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc
+-rw-r--r--   0        0        0     1657 2024-05-18 05:36:37.495037 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc
+-rw-r--r--   0        0        0     1822 2024-05-18 05:36:37.495201 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc
+-rw-r--r--   0        0        0     1818 2024-05-18 07:21:08.395043 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc
+-rw-r--r--   0        0        0     1715 2024-05-01 07:29:51.195530 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/groq_client.py
+-rw-r--r--   0        0        0     1009 2024-05-18 05:36:37.495488 knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/openai_client.py
+-rw-r--r--   0        0        0     3908 2024-05-01 07:29:51.193626 knowledge_graph_maker-0.1.1/knowledge_graph_maker/logger.py
+-rw-r--r--   0        0        0     2093 2024-05-04 14:44:32.548460 knowledge_graph_maker-0.1.1/knowledge_graph_maker/neo4j_graph_model.py
+-rw-r--r--   0        0        0      938 2024-05-04 14:44:32.548639 knowledge_graph_maker-0.1.1/knowledge_graph_maker/types.py
+-rw-r--r--   0        0        0      694 2024-05-18 12:58:43.759451 knowledge_graph_maker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8691 1970-01-01 00:00:00.000000 knowledge_graph_maker-0.1.1/PKG-INFO
```

### Comparing `knowledge_graph_maker-0.1.0/LICENSE` & `knowledge_graph_maker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/README.md` & `knowledge_graph_maker-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,54 @@
-# The Graph Maker
+# The Knowledge Graph Maker
 
 A Python tool that can convert any text into a graph of knowedge given an ontology.
 
 ![The Graph Maker](./assets/GraphMaker.png)
 _Image generated using Adobe Firefly and Photoshop_
 
 ## What is a knowledge graph?
 
 A knowledge graph, also known as a semantic network, represents a network of real-world entities—i.e. objects, events, situations, or concepts—and illustrates the relationship between them. This information is usually stored in a graph database and visualized as a graph structure, prompting the term knowledge “graph.”
 
 Source: https://www.ibm.com/topics/knowledge-graph
 
-## Why Graph?
+## Why Knowledge Graph?
 
 KG can be used for a multitude of purposes. We can run graph algorithms and calculate centralities of any node, to understand how important a concept (node) is to this body of work. We can calculate communities to bunch the concepts together to better analyse the text. We can understand the connectedness between seemingly disconnected concepts.
 
 The best of all, we can achieve **Graph Retrieval Augmented Generation (GRAG)** and chat with our text in a much more profound way using Graph as a retriever. This is a new and improved version of **Retrieval Augmented Generation (RAG)** where we use a vectory db as a retriever to chat with our documents.
 
 ---
 
 ## This project
 
 This is a python library that can create knowledge graphs out of any text using a given ontology. The library creates the graph fairly consistently with a good resilience to the faulty response generated by the LLM.
 
-Here are the steps to create the knowledge graph.
-
-To set up this project, [you will need Poetry](https://python-poetry.org/docs/configuration/)
+Here is how to use the library
 
-```zsh
-# Create a local environment
-$ poetry config --local virtualenvs.in-project true
-# Install dependencies.
-$ poetry install
+```shell
+# Get the library
+$ pip install knowledge-graph-maker
+```
+
+Remember to set the following environment variables in your .env file
+
+```shell
+## If using GROQ Client
+GROQ_API_KEY="groq_api_key"
+## If using OpenAI Client
+OPENAI_API_KEY="openai_api_key"
+## If using Neo4j
+NEO4J_USERNAME="neo4j"
+NEO4J_PASSWORD="localneo4j"
+NEO4J_URI="bolt://localhost:7687"
 ```
 
+Here are the steps to create the knowledge graph.
+
 ### 1. Define the Ontology of your Graph
 
 The library understands the following schema for the Ontology. Behind the scene, ontology is a pydantic model.
 
 ```python
 ontology = Ontology(
     # labels of the entities to be extracted. Can be a string or an object, like the following.
@@ -77,29 +88,60 @@
     text: str
     metadata: dict
 ```
 
 The metadata we add to the document here is tagged to every relation that is extracted out of the document.
 We can add the context of the relation, for example the page number, chapter, the name of the article, etc. into the metadata. More often than not, Each node pairs have multiple relation with each other across multiple documents. The metadata helps contextualise these relationships.
 
-### 4. Run the Graph Maker.
+### 4. Select an LLM
+
+The knowledge graph maker provides a OpenAI and Groq LLM clients out of the box.
+
+```python
+
+## Groq models
+model = "mixtral-8x7b-32768"
+# model ="llama3-8b-8192"
+# model = "llama3-70b-8192"
+# model="gemma-7b-it"
+
+## Open AI models
+oai_model="gpt-3.5-turbo"
+
+## Use Groq
+# llm = GroqClient(model=model, temperature=0.1, top_p=0.5)
+## OR Use OpenAI
+llm = OpenAIClient(model=oai_model, temperature=0.1, top_p=0.5)
+
+```
+
+Optionally you can also code your own LLM Client as long as it follows the following abstract class
+
+```python
+class LLMClient(ABC):
+    @abstractmethod
+    def __init__(self, model: str, temperature: float, top_p: float):
+        pass
+
+    @abstractmethod
+    def generate(self, user_message: str, system_message: str) -> str:
+        "Generate and return the result text as string"
+        pass
+```
+
+### 5. Run the Graph Maker.
 
 The Graph Maker directly takes a list of documents and iterates over each of them to create one subgraph per document. The final output is the complete graph of all the documents.
 
 Here is the simple example code
 
 ```python
-from graph_maker import GraphMaker, Ontology, GroqClient
-from graph_maker import Document
+from knowledge_graph_maker import GraphMaker, Ontology, GroqClient
+from knowledge_graph_maker import Document
 
-## Select a groq supported model
-## model = "mixtral-8x7b-32768"
-model ="llama3-8b-8192"
-## model = "llama3-70b-8192"
-## model="gemma-7b-it" ## This is probably the fastest of all models, though a tad inaccurate.
 
 llm = GroqClient(model=model, temperature=0.1, top_p=0.5)
 graph_maker = GraphMaker(ontology=ontology, llm_client=llm, verbose=False)
 
 ## create a graph out of a list of Documents.
 graph = graph_maker.from_documents(
     list(docs),
@@ -124,20 +166,20 @@
     metadata: dict = {}
     order: Union[int, None] = None
 ```
 
 The Graph Makers runs each document through the model and parses the response into graph edges.
 I have tuned the prompts to a point where it is quite fault tolerant by now. Most JSON failures are automatically corrected. In case the JSON response fails to parse, it also tries to manually split the JSON string into multiple strings of edges and then tries to parse each one of them separately.
 
-### 5. Save to Neo4j (optional step)
+### 6. Save to Neo4j (optional step)
 
 We can save the model to Neo4j either to create an RAG application, run Network algorithms, or maybe just visualise the graph using the Bloom
 
 ```python
-from graph_maker import Neo4jGraphModel
+from knowledge_graph_maker import Neo4jGraphModel
 
 create_indices = False
 neo4j_graph = Neo4jGraphModel(edges=graph, create_indices=create_indices)
 
 neo4j_graph.save()
 
 ```
```

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/graph_maker.py` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/graph_maker.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/groq_client.py` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/groq_client.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/llm_clients/openai_client.py` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/llm_clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/logger.py` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/logger.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/neo4j_graph_model.py` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/neo4j_graph_model.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/knowledge_graph_maker/types.py` & `knowledge_graph_maker-0.1.1/knowledge_graph_maker/types.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.0/pyproject.toml` & `knowledge_graph_maker-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "knowledge-graph-maker"
-version = "0.1.0"
+version = "0.1.1"
 description = "Create knowledge graph out of any text using a given ontology"
 authors = ["Rahul Nayak <rahul.nyk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 langchain = "^0.0.335"
```

### Comparing `knowledge_graph_maker-0.1.0/PKG-INFO` & `knowledge_graph_maker-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge-graph-maker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create knowledge graph out of any text using a given ontology
 Author: Rahul Nayak
 Author-email: rahul.nyk@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -24,50 +24,61 @@
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: unstructured (>=0.10.30,<0.11.0)
 Requires-Dist: uuid (>=1.30,<2.0)
 Requires-Dist: yachalk (>=0.1.5,<0.2.0)
 Description-Content-Type: text/markdown
 
-# The Graph Maker
+# The Knowledge Graph Maker
 
 A Python tool that can convert any text into a graph of knowedge given an ontology.
 
 ![The Graph Maker](./assets/GraphMaker.png)
 _Image generated using Adobe Firefly and Photoshop_
 
 ## What is a knowledge graph?
 
 A knowledge graph, also known as a semantic network, represents a network of real-world entities—i.e. objects, events, situations, or concepts—and illustrates the relationship between them. This information is usually stored in a graph database and visualized as a graph structure, prompting the term knowledge “graph.”
 
 Source: https://www.ibm.com/topics/knowledge-graph
 
-## Why Graph?
+## Why Knowledge Graph?
 
 KG can be used for a multitude of purposes. We can run graph algorithms and calculate centralities of any node, to understand how important a concept (node) is to this body of work. We can calculate communities to bunch the concepts together to better analyse the text. We can understand the connectedness between seemingly disconnected concepts.
 
 The best of all, we can achieve **Graph Retrieval Augmented Generation (GRAG)** and chat with our text in a much more profound way using Graph as a retriever. This is a new and improved version of **Retrieval Augmented Generation (RAG)** where we use a vectory db as a retriever to chat with our documents.
 
 ---
 
 ## This project
 
 This is a python library that can create knowledge graphs out of any text using a given ontology. The library creates the graph fairly consistently with a good resilience to the faulty response generated by the LLM.
 
-Here are the steps to create the knowledge graph.
-
-To set up this project, [you will need Poetry](https://python-poetry.org/docs/configuration/)
+Here is how to use the library
 
-```zsh
-# Create a local environment
-$ poetry config --local virtualenvs.in-project true
-# Install dependencies.
-$ poetry install
+```shell
+# Get the library
+$ pip install knowledge-graph-maker
+```
+
+Remember to set the following environment variables in your .env file
+
+```shell
+## If using GROQ Client
+GROQ_API_KEY="groq_api_key"
+## If using OpenAI Client
+OPENAI_API_KEY="openai_api_key"
+## If using Neo4j
+NEO4J_USERNAME="neo4j"
+NEO4J_PASSWORD="localneo4j"
+NEO4J_URI="bolt://localhost:7687"
 ```
 
+Here are the steps to create the knowledge graph.
+
 ### 1. Define the Ontology of your Graph
 
 The library understands the following schema for the Ontology. Behind the scene, ontology is a pydantic model.
 
 ```python
 ontology = Ontology(
     # labels of the entities to be extracted. Can be a string or an object, like the following.
@@ -107,29 +118,60 @@
     text: str
     metadata: dict
 ```
 
 The metadata we add to the document here is tagged to every relation that is extracted out of the document.
 We can add the context of the relation, for example the page number, chapter, the name of the article, etc. into the metadata. More often than not, Each node pairs have multiple relation with each other across multiple documents. The metadata helps contextualise these relationships.
 
-### 4. Run the Graph Maker.
+### 4. Select an LLM
+
+The knowledge graph maker provides a OpenAI and Groq LLM clients out of the box.
+
+```python
+
+## Groq models
+model = "mixtral-8x7b-32768"
+# model ="llama3-8b-8192"
+# model = "llama3-70b-8192"
+# model="gemma-7b-it"
+
+## Open AI models
+oai_model="gpt-3.5-turbo"
+
+## Use Groq
+# llm = GroqClient(model=model, temperature=0.1, top_p=0.5)
+## OR Use OpenAI
+llm = OpenAIClient(model=oai_model, temperature=0.1, top_p=0.5)
+
+```
+
+Optionally you can also code your own LLM Client as long as it follows the following abstract class
+
+```python
+class LLMClient(ABC):
+    @abstractmethod
+    def __init__(self, model: str, temperature: float, top_p: float):
+        pass
+
+    @abstractmethod
+    def generate(self, user_message: str, system_message: str) -> str:
+        "Generate and return the result text as string"
+        pass
+```
+
+### 5. Run the Graph Maker.
 
 The Graph Maker directly takes a list of documents and iterates over each of them to create one subgraph per document. The final output is the complete graph of all the documents.
 
 Here is the simple example code
 
 ```python
-from graph_maker import GraphMaker, Ontology, GroqClient
-from graph_maker import Document
+from knowledge_graph_maker import GraphMaker, Ontology, GroqClient
+from knowledge_graph_maker import Document
 
-## Select a groq supported model
-## model = "mixtral-8x7b-32768"
-model ="llama3-8b-8192"
-## model = "llama3-70b-8192"
-## model="gemma-7b-it" ## This is probably the fastest of all models, though a tad inaccurate.
 
 llm = GroqClient(model=model, temperature=0.1, top_p=0.5)
 graph_maker = GraphMaker(ontology=ontology, llm_client=llm, verbose=False)
 
 ## create a graph out of a list of Documents.
 graph = graph_maker.from_documents(
     list(docs),
@@ -154,20 +196,20 @@
     metadata: dict = {}
     order: Union[int, None] = None
 ```
 
 The Graph Makers runs each document through the model and parses the response into graph edges.
 I have tuned the prompts to a point where it is quite fault tolerant by now. Most JSON failures are automatically corrected. In case the JSON response fails to parse, it also tries to manually split the JSON string into multiple strings of edges and then tries to parse each one of them separately.
 
-### 5. Save to Neo4j (optional step)
+### 6. Save to Neo4j (optional step)
 
 We can save the model to Neo4j either to create an RAG application, run Network algorithms, or maybe just visualise the graph using the Bloom
 
 ```python
-from graph_maker import Neo4jGraphModel
+from knowledge_graph_maker import Neo4jGraphModel
 
 create_indices = False
 neo4j_graph = Neo4jGraphModel(edges=graph, create_indices=create_indices)
 
 neo4j_graph.save()
 
 ```
```

