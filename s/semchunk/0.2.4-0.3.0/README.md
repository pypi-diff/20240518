# Comparing `tmp/semchunk-0.2.4.tar.gz` & `tmp/semchunk-0.3.0.tar.gz`

## Comparing `semchunk-0.2.4.tar` & `semchunk-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 semchunk-0.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 semchunk-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 semchunk-0.2.4/src/semchunk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.2.4/src/semchunk/py.typed
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 semchunk-0.2.4/src/semchunk/semchunk.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 semchunk-0.2.4/tests/bench.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 semchunk-0.2.4/tests/test_semchunk.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-0.2.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.2.4/LICENCE
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 semchunk-0.2.4/README.md
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 semchunk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 semchunk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 semchunk-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 semchunk-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 semchunk-0.3.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 semchunk-0.3.0/src/semchunk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.3.0/src/semchunk/py.typed
+-rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 semchunk-0.3.0/src/semchunk/semchunk.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 semchunk-0.3.0/tests/bench.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 semchunk-0.3.0/tests/test_semchunk.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.3.0/LICENCE
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 semchunk-0.3.0/README.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 semchunk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 semchunk-0.3.0/PKG-INFO
```

### Comparing `semchunk-0.2.4/CHANGELOG.md` & `semchunk-0.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Changelog 🔄
 All notable changes to `semchunk` will be documented here. This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.0] - 2024-05-18
+### Added
+- Introduced the `chunkerify()` function, which constructs a chunker from a tokenizer or token counter that can be reused and can also chunk multiple texts in a single call. The resulting chunker speeds up chunking by 40.4% thanks, in large part, to a token counter that avoid having to count the number of tokens in a text when the number of characters in the text exceed a certain threshold, courtesy of [@R0bk](https://github.com/R0bk) ([#3](https://github.com/umarbutler/semchunk/pull/3)) ([337a186](https://github.com/umarbutler/semchunk/pull/3/commits/337a18615f991076b076262288b0408cb162b48c)).
+
 ## [0.2.4] - 2024-05-13
 ### Changed
-- Improved chunking performance with larger chunk sizes by switching from linear to binary search for the identification of optimal chunk boundaries, courtesy of [@R0bk](https://github.com/R0bk) ([#3](https://github.com/umarbutler/semchunk/pull/3)) ([1e3ddb9](https://github.com/umarbutler/semchunk/pull/3/commits/1e3ddb91698f072da1d8a7d809a66467e1d31ff8)).
+- Improved chunking performance with larger chunk sizes by switching from linear to binary search for the identification of optimal chunk boundaries, courtesy of [@R0bk](https://github.com/R0bk) ([#3](https://github.com/umarbutler/semchunk/pull/3)) ([337a186](https://github.com/umarbutler/semchunk/pull/3/commits/337a18615f991076b076262288b0408cb162b48c)).
 
 ## [0.2.3] - 2024-03-11
 ### Fixed
 - Ensured that memoization does not overwrite `chunk()`'s function signature.
 
 ## [0.2.2] - 2024-02-05
 ### Fixed
@@ -40,14 +44,15 @@
 - Improved chunking performance.
 - improved test coverage.
 
 ## [0.1.0] - 2023-11-05
 ### Added
 - Added the `chunk()` function, which splits text into semantically meaningful chunks of a specified size as determined by a provided token counter.
 
+[0.3.0]: https://github.com/umarbutler/semchunk/compare/v0.2.4...v0.3.0
 [0.2.4]: https://github.com/umarbutler/semchunk/compare/v0.2.3...v0.2.4
 [0.2.3]: https://github.com/umarbutler/semchunk/compare/v0.2.2...v0.2.3
 [0.2.2]: https://github.com/umarbutler/semchunk/compare/v0.2.1...v0.2.2
 [0.2.1]: https://github.com/umarbutler/semchunk/compare/v0.2.0...v0.2.1
 [0.2.0]: https://github.com/umarbutler/semchunk/compare/v0.1.2...v0.2.0
 [0.1.2]: https://github.com/umarbutler/semchunk/compare/v0.1.1...v0.1.2
 [0.1.1]: https://github.com/umarbutler/semchunk/compare/v0.1.0...v0.1.1
```

### Comparing `semchunk-0.2.4/.github/workflows/ci.yml` & `semchunk-0.3.0/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     - name: Install test dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest
         python -m pip install pytest-cov
         python -m pip install tiktoken
         python -m pip install nltk
+        python -m pip install transformers
 
     - name: Install semchunk
       run: |
         python -m pip install .
 
     - name: Test with pytest
       run: |
```

### Comparing `semchunk-0.2.4/tests/bench.py` & `semchunk-0.3.0/tests/bench.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,45 @@
-import semchunk
-from semantic_text_splitter import TextSplitter
-import test_semchunk
 import time
 
-chunk_size = 512
-semantic_text_splitter_chunker = TextSplitter.from_tiktoken_model('gpt-4', chunk_size)
+import semchunk
 
-def bench_semchunk(text: str) -> None:
-    semchunk.chunk(text, chunk_size=chunk_size, token_counter=test_semchunk._token_counter)
+import nltk
+import tiktoken
 
-def bench_semantic_text_splitter(text: str) -> None:
-    semantic_text_splitter_chunker.chunks(text)
+from semantic_text_splitter import TextSplitter
 
-libraries = {
-    'semchunk': bench_semchunk,
-    'semantic_text_splitter': bench_semantic_text_splitter,
-}
+# BEGIN CONFIG #
+CHUNK_SIZE = 512
+# END CONFIG #
 
 def bench() -> dict[str, float]:
+    # Initialise the chunkers.
+    semchunk_chunker = semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'), CHUNK_SIZE)
+    semantic_text_splitter_chunker = TextSplitter.from_tiktoken_model('gpt-4', CHUNK_SIZE)
+
+    def bench_semchunk(text: str) -> None:
+        semchunk_chunker(text)
+
+    def bench_semantic_text_splitter(text: str) -> None:
+        semantic_text_splitter_chunker.chunks(text)
+
+    libraries = {
+        'semchunk': bench_semchunk,
+        #'semantic_text_splitter': bench_semantic_text_splitter,
+    }
+
+    # Download the Gutenberg corpus.
+    nltk.download('gutenberg')
+    gutenberg = nltk.corpus.gutenberg
+    
+    # Benchmark the libraries.
     benchmarks = dict.fromkeys(libraries.keys(), 0)
     
-    for fileid in test_semchunk.gutenberg.fileids():
-        sample = test_semchunk.gutenberg.raw(fileid)
+    for fileid in gutenberg.fileids():
+        sample = gutenberg.raw(fileid)
         for library, function in libraries.items():
             start = time.time()
             function(sample)
             benchmarks[library] += time.time() - start
     
     return benchmarks
```

### Comparing `semchunk-0.2.4/LICENCE` & `semchunk-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `semchunk-0.2.4/pyproject.toml` & `semchunk-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "semchunk"
-version = "0.2.4"
+version = "0.3.0"
 authors = [
   {name="Umar Butler", email="umar@umar.au"},
 ]
 description = "A fast and lightweight pure Python library for splitting text into semantically meaningful chunks."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
@@ -31,14 +31,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: General",
     "Topic :: Utilities",
     "Typing :: Typed"
```

### Comparing `semchunk-0.2.4/PKG-INFO` & `semchunk-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: semchunk
-Version: 0.2.4
+Version: 0.3.0
 Summary: A fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 Project-URL: Homepage, https://github.com/umarbutler/semchunk
 Project-URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues
 Project-URL: Source, https://github.com/umarbutler/semchunk
 Author-email: Umar Butler <umar@umar.au>
 License: MIT
@@ -16,14 +16,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
@@ -31,46 +32,83 @@
 Description-Content-Type: text/markdown
 
 # semchunk
 <a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <!-- <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a> -->
 
 `semchunk` is a fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 
-Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 80% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
+Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 90% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
 
 ## Installation 📦
 `semchunk` may be installed with `pip`:
 ```bash
 pip install semchunk
 ```
 
 ## Usage 👩‍💻
 The code snippet below demonstrates how text can be chunked with `semchunk`:
 ```python
->>> import semchunk
->>> import tiktoken # `tiktoken` is not required but is used here to quickly count tokens.
->>> text = 'The quick brown fox jumps over the lazy dog.'
->>> chunk_size = 2 # A low chunk size is used here for demo purposes.
->>> encoder = tiktoken.encoding_for_model('gpt-4')
->>> token_counter = lambda text: len(encoder.encode(text)) # `token_counter` may be swapped out for any function capable of counting tokens.
->>> semchunk.chunk(text, chunk_size=chunk_size, token_counter=token_counter)
-['The quick', 'brown fox', 'jumps over', 'the lazy', 'dog.']
+import semchunk
+from transformers import AutoTokenizer # Neither `transformers` nor `tiktoken` are required,
+import tiktoken                        # they are here for demonstration purposes.
+
+chunk_size = 2 # A low chunk size is used here for demonstration purposes.
+text = 'The quick brown fox jumps over the lazy dog.'
+
+# As you can see below, `semchunk.chunkerify` will accept the names of all OpenAI models, OpenAI
+# `tiktoken` encodings and Hugging Face models (in that order of precedence), along with custom
+# tokenizers that have an `encode()` method (such as `tiktoken`, `transformers` and `tokenizers`
+# tokenizers) and finally any function that can take a text and return the number of tokens in it.
+chunker = semchunk.chunkerify('umarbutler/emubert', chunk_size) or \
+          semchunk.chunkerify('gpt-4', chunk_size) or \
+          semchunk.chunkerify('cl100k_base', chunk_size) or \
+          semchunk.chunkerify(AutoTokenizer.from_pretrained('umarbutler/emubert'), chunk_size) or \
+          semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'), chunk_size) or \
+          semchunk.chunkerify(lambda text: len(text.split()), chunk_size)
+
+# The resulting `chunker` can take and chunk a single text or a list of texts, returning a list of
+# chunks or a list of lists of chunks, respectively.
+assert chunker(text) == ['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']
+assert chunker([text]) == [['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']]
 ```
 
+### Chunkerify
+```python
+def chunkerify(
+    tokenizer_or_token_counter: str | tiktoken.Encoding | transformers.PreTrainedTokenizer | \
+                                tokenizers.Tokenizer | Callable[[str], int],
+    chunk_size: int = None,
+    max_token_chars: int = None,
+    memoize: bool = True,
+) -> Callable[[str | Sequence[str]], list[str] | list[list[str]]]:
+```
+
+`chunkerify()` constructs a chunker that splits one or more texts into semantically meaningful chunks of a specified size as determined by the provided tokenizer or token counter.
+
+`tokenizer_or_token_counter` is either: the name of a `tiktoken` or `transformers` tokenizer (with priority given to the former); a tokenizer that possesses an `encode` attribute (eg, a `tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that returns the number of tokens in a input.
+
+`chunk_size` is the maximum number of tokens a chunk may contain. It defaults to `None` in which case it will be set to the same value as the tokenizer's `model_max_length` attribute (deducted by the number of tokens returned by attempting to tokenize an empty string) if possible otherwise a `ValueError` will be raised.
+
+`max_token_chars` is the maximum numbers of characters a token may contain. It is used to significantly speed up the token counting of long inputs. It defaults to `None` in which case it will either not be used or will, if possible, be set to the numbers of characters in the longest token in the tokenizer's vocabulary as determined by the `token_byte_values` or `get_vocab` methods.
+
+`memoize` flags whether to memoise the token counter. It defaults to `True`.
+
+This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts.
+
 ### Chunk
 ```python
 def chunk(
     text: str,
     chunk_size: int,
-    token_counter: callable,
-    memoize: bool=True
+    token_counter: Callable,
+    memoize: bool = True,
 ) -> list[str]
 ```
 
-`chunk()` splits text into semantically meaningful chunks of a specified size as determined by the provided token counter.
+`chunk()` splits a text into semantically meaningful chunks of a specified size as determined by the provided token counter.
 
 `text` is the text to be chunked.
 
 `chunk_size` is the maximum number of tokens a chunk may contain.
 
 `token_counter` is a callable that takes a string and returns the number of tokens in it.
 
@@ -94,13 +132,13 @@
 1. Sentence interrupters (`:`, `—` and `…`);
 1. Word joiners (`/`, `\`, `–`, `&` and `-`); and
 1. All other characters.
 
 `semchunk` also relies on memoization to cache the results of token counters and the `chunk()` function, thereby improving performance.
 
 ## Benchmarks 📊
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it takes `semchunk` 14.11s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 2 minutes and 56.1 seconds to chunk the same texts into 512-token-long chunks — a difference of 87.84%.
+On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes `semchunk` 8.34s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same texts into 512-token-long chunks — a difference of 92.84%.
 
 The code used to benchmark `semchunk` and `semantic-text-splitter` is available [here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py).
 
 ## Licence 📄
 This library is licensed under the [MIT License](https://github.com/umarbutler/semchunk/blob/main/LICENCE).
```

#### html2text {}

```diff
@@ -1,55 +1,94 @@
-Metadata-Version: 2.3 Name: semchunk Version: 0.2.4 Summary: A fast and
+Metadata-Version: 2.3 Name: semchunk Version: 0.3.0 Summary: A fast and
 lightweight pure Python library for splitting text into semantically meaningful
 chunks. Project-URL: Homepage, https://github.com/umarbutler/semchunk Project-
 URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues Project-URL:
 Source, https://github.com/umarbutler/semchunk Author-email: Umar Butler
 umar.au> License: MIT License-File: LICENCE Keywords:
 chunk,chunker,chunking,chunks,nlp,split,splits,splitter,splitting,text
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
-:: General Classifier: Topic :: Utilities Classifier: Typing :: Typed Requires-
-Python: >=3.9 Description-Content-Type: text/markdown # semchunk _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/
-_s_t_a_t_u_s_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/
-_c_/_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and lightweight pure Python
+Language :: Python :: 3.13 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Text Processing :: General Classifier:
+Topic :: Utilities Classifier: Typing :: Typed Requires-Python: >=3.9
+Description-Content-Type: text/markdown # semchunk _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_p_y_p_i_/_v_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/
+_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/_c_/
+_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and lightweight pure Python
 library for splitting text into semantically meaningful chunks. Owing to its
 complex yet highly efficient chunking algorithm, `semchunk` is both more
 semantically accurate than
 [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://
 python.langchain.com/docs/modules/data_connection/document_transformers/
 text_splitters/recursive_text_splitter) (see [How It Works ð](https://
-github.com/umarbutler/semchunk#how-it-works-)) and is also over 80% faster than
+github.com/umarbutler/semchunk#how-it-works-)) and is also over 90% faster than
 [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/)
 (see the [Benchmarks ð](https://github.com/umarbutler/semchunk#benchmarks-
 )). ## Installation ð¦ `semchunk` may be installed with `pip`: ```bash pip
 install semchunk ``` ## Usage ð©âð» The code snippet below demonstrates
-how text can be chunked with `semchunk`: ```python >>> import semchunk >>>
-import tiktoken # `tiktoken` is not required but is used here to quickly count
-tokens. >>> text = 'The quick brown fox jumps over the lazy dog.' >>>
-chunk_size = 2 # A low chunk size is used here for demo purposes. >>> encoder =
-tiktoken.encoding_for_model('gpt-4') >>> token_counter = lambda text: len
-(encoder.encode(text)) # `token_counter` may be swapped out for any function
-capable of counting tokens. >>> semchunk.chunk(text, chunk_size=chunk_size,
-token_counter=token_counter) ['The quick', 'brown fox', 'jumps over', 'the
-lazy', 'dog.'] ``` ### Chunk ```python def chunk( text: str, chunk_size: int,
-token_counter: callable, memoize: bool=True ) -> list[str] ``` `chunk()` splits
-text into semantically meaningful chunks of a specified size as determined by
-the provided token counter. `text` is the text to be chunked. `chunk_size` is
-the maximum number of tokens a chunk may contain. `token_counter` is a callable
+how text can be chunked with `semchunk`: ```python import semchunk from
+transformers import AutoTokenizer # Neither `transformers` nor `tiktoken` are
+required, import tiktoken # they are here for demonstration purposes.
+chunk_size = 2 # A low chunk size is used here for demonstration purposes. text
+= 'The quick brown fox jumps over the lazy dog.' # As you can see below,
+`semchunk.chunkerify` will accept the names of all OpenAI models, OpenAI #
+`tiktoken` encodings and Hugging Face models (in that order of precedence),
+along with custom # tokenizers that have an `encode()` method (such as
+`tiktoken`, `transformers` and `tokenizers` # tokenizers) and finally any
+function that can take a text and return the number of tokens in it. chunker =
+semchunk.chunkerify('umarbutler/emubert', chunk_size) or \ semchunk.chunkerify
+('gpt-4', chunk_size) or \ semchunk.chunkerify('cl100k_base', chunk_size) or \
+semchunk.chunkerify(AutoTokenizer.from_pretrained('umarbutler/emubert'),
+chunk_size) or \ semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'),
+chunk_size) or \ semchunk.chunkerify(lambda text: len(text.split()),
+chunk_size) # The resulting `chunker` can take and chunk a single text or a
+list of texts, returning a list of # chunks or a list of lists of chunks,
+respectively. assert chunker(text) == ['The quick', 'brown', 'fox', 'jumps',
+'over the', 'lazy', 'dog.'] assert chunker([text]) == [['The quick', 'brown',
+'fox', 'jumps', 'over the', 'lazy', 'dog.']] ``` ### Chunkerify ```python def
+chunkerify( tokenizer_or_token_counter: str | tiktoken.Encoding |
+transformers.PreTrainedTokenizer | \ tokenizers.Tokenizer | Callable[[str],
+int], chunk_size: int = None, max_token_chars: int = None, memoize: bool =
+True, ) -> Callable[[str | Sequence[str]], list[str] | list[list[str]]]: ```
+`chunkerify()` constructs a chunker that splits one or more texts into
+semantically meaningful chunks of a specified size as determined by the
+provided tokenizer or token counter. `tokenizer_or_token_counter` is either:
+the name of a `tiktoken` or `transformers` tokenizer (with priority given to
+the former); a tokenizer that possesses an `encode` attribute (eg, a
+`tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that
+returns the number of tokens in a input. `chunk_size` is the maximum number of
+tokens a chunk may contain. It defaults to `None` in which case it will be set
+to the same value as the tokenizer's `model_max_length` attribute (deducted by
+the number of tokens returned by attempting to tokenize an empty string) if
+possible otherwise a `ValueError` will be raised. `max_token_chars` is the
+maximum numbers of characters a token may contain. It is used to significantly
+speed up the token counting of long inputs. It defaults to `None` in which case
+it will either not be used or will, if possible, be set to the numbers of
+characters in the longest token in the tokenizer's vocabulary as determined by
+the `token_byte_values` or `get_vocab` methods. `memoize` flags whether to
+memoise the token counter. It defaults to `True`. This function returns a
+callable that takes either a single text or a sequence of texts and returns, if
+a single text has been provided, a list of chunks up to `chunk_size`-tokens-
+long with any whitespace used to split the text removed, or, if multiple texts
+have been provided, a list of lists of chunks, with each inner list
+corresponding to the chunks of one of the provided input texts. ### Chunk
+```python def chunk( text: str, chunk_size: int, token_counter: Callable,
+memoize: bool = True, ) -> list[str] ``` `chunk()` splits a text into
+semantically meaningful chunks of a specified size as determined by the
+provided token counter. `text` is the text to be chunked. `chunk_size` is the
+maximum number of tokens a chunk may contain. `token_counter` is a callable
 that takes a string and returns the number of tokens in it. `memoize` flags
 whether to memoise the token counter. It defaults to `True`. This function
 returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace
 used to split the text removed. ## How It Works ð `semchunk` works by
 recursively splitting texts until all resulting chunks are equal to or less
 than a specified chunk size. In particular, it: 1. Splits text using the most
 semantically meaningful splitter possible; 1. Recursively splits the resulting
@@ -64,18 +103,18 @@
 sequence of tabs; 1. The largest sequence of whitespace characters (as defined
 by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
 `*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
 `â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
 1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
 `semchunk` also relies on memoization to cache the results of token counters
 and the `chunk()` function, thereby improving performance. ## Benchmarks ð
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it
-takes `semchunk` 14.11s seconds to split every sample in [NLTK's Gutenberg
+On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it
+takes `semchunk` 8.34s seconds to split every sample in [NLTK's Gutenberg
 Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
 token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
-(https://pypi.org/project/semantic-text-splitter/) 2 minutes and 56.1 seconds
-to chunk the same texts into 512-token-long chunks â a difference of 87.84%.
-The code used to benchmark `semchunk` and `semantic-text-splitter` is available
-[here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py). ##
-Licence ð This library is licensed under the [MIT License](https://
-github.com/umarbutler/semchunk/blob/main/LICENCE).
+(https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the
+same texts into 512-token-long chunks â a difference of 92.84%. The code used
+to benchmark `semchunk` and `semantic-text-splitter` is available [here](https:
+//github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð
+This library is licensed under the [MIT License](https://github.com/umarbutler/
+semchunk/blob/main/LICENCE).
```

