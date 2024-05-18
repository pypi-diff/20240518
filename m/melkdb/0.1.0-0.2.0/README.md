# Comparing `tmp/melkdb-0.1.0.tar.gz` & `tmp/melkdb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melkdb-0.1.0.tar", last modified: Mon Mar 25 02:53:42 2024, max compression
+gzip compressed data, was "melkdb-0.2.0.tar", last modified: Sat May 18 20:11:36 2024, max compression
```

## Comparing `melkdb-0.1.0.tar` & `melkdb-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jaedsonpys  (1000) jaedsonpys  (1000)        0 2024-03-25 02:53:42.666045 melkdb-0.1.0/
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     1070 2024-03-24 14:34:19.000000 melkdb-0.1.0/LICENSE
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     3681 2024-03-25 02:53:42.666045 melkdb-0.1.0/PKG-INFO
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2721 2024-03-24 18:44:05.000000 melkdb-0.1.0/README.md
-drwxrwxr-x   0 jaedsonpys  (1000) jaedsonpys  (1000)        0 2024-03-25 02:53:42.662045 melkdb-0.1.0/melkdb/
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       64 2024-03-24 18:32:18.000000 melkdb-0.1.0/melkdb/__init__.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       22 2024-03-23 03:41:46.000000 melkdb-0.1.0/melkdb/__version__.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     1820 2024-03-24 15:21:39.000000 melkdb-0.1.0/melkdb/_block.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2698 2024-03-24 15:28:32.000000 melkdb-0.1.0/melkdb/_item.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2330 2024-03-23 22:41:56.000000 melkdb-0.1.0/melkdb/crypto.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)      965 2024-03-24 18:55:51.000000 melkdb-0.1.0/melkdb/exceptions.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     5611 2024-03-24 18:58:17.000000 melkdb-0.1.0/melkdb/melkdb.py
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)      252 2024-03-23 23:07:10.000000 melkdb-0.1.0/melkdb/utils.py
-drwxrwxr-x   0 jaedsonpys  (1000) jaedsonpys  (1000)        0 2024-03-25 02:53:42.662045 melkdb-0.1.0/melkdb.egg-info/
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     3681 2024-03-25 02:53:42.000000 melkdb-0.1.0/melkdb.egg-info/PKG-INFO
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)      320 2024-03-25 02:53:42.000000 melkdb-0.1.0/melkdb.egg-info/SOURCES.txt
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)        1 2024-03-25 02:53:42.000000 melkdb-0.1.0/melkdb.egg-info/dependency_links.txt
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       19 2024-03-25 02:53:42.000000 melkdb-0.1.0/melkdb.egg-info/requires.txt
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)        7 2024-03-25 02:53:42.000000 melkdb-0.1.0/melkdb.egg-info/top_level.txt
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       38 2024-03-25 02:53:42.670045 melkdb-0.1.0/setup.cfg
--rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     1340 2024-03-25 02:52:16.000000 melkdb-0.1.0/setup.py
+drwxrwxr-x   0 jaedsonpys  (1000) jaedsonpys  (1000)        0 2024-05-18 20:11:36.438850 melkdb-0.2.0/
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     1070 2024-03-24 14:34:19.000000 melkdb-0.2.0/LICENSE
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     3532 2024-05-18 20:11:36.434851 melkdb-0.2.0/PKG-INFO
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2572 2024-05-18 20:11:09.000000 melkdb-0.2.0/README.md
+drwxrwxr-x   0 jaedsonpys  (1000) jaedsonpys  (1000)        0 2024-05-18 20:11:36.434851 melkdb-0.2.0/melkdb/
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       64 2024-03-24 18:32:18.000000 melkdb-0.2.0/melkdb/__init__.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       22 2024-05-18 19:59:45.000000 melkdb-0.2.0/melkdb/__version__.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2649 2024-05-18 19:28:23.000000 melkdb-0.2.0/melkdb/_block.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2698 2024-03-24 15:28:32.000000 melkdb-0.2.0/melkdb/_item.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     2330 2024-03-23 22:41:56.000000 melkdb-0.2.0/melkdb/crypto.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     1199 2024-05-18 20:06:48.000000 melkdb-0.2.0/melkdb/exceptions.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     7162 2024-05-18 20:07:18.000000 melkdb-0.2.0/melkdb/melkdb.py
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)      247 2024-05-18 16:15:08.000000 melkdb-0.2.0/melkdb/utils.py
+drwxrwxr-x   0 jaedsonpys  (1000) jaedsonpys  (1000)        0 2024-05-18 20:11:36.434851 melkdb-0.2.0/melkdb.egg-info/
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     3532 2024-05-18 20:11:36.000000 melkdb-0.2.0/melkdb.egg-info/PKG-INFO
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)      320 2024-05-18 20:11:36.000000 melkdb-0.2.0/melkdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)        1 2024-05-18 20:11:36.000000 melkdb-0.2.0/melkdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       19 2024-05-18 20:11:36.000000 melkdb-0.2.0/melkdb.egg-info/requires.txt
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)        7 2024-05-18 20:11:36.000000 melkdb-0.2.0/melkdb.egg-info/top_level.txt
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)       38 2024-05-18 20:11:36.438850 melkdb-0.2.0/setup.cfg
+-rw-rw-r--   0 jaedsonpys  (1000) jaedsonpys  (1000)     1340 2024-03-25 02:52:16.000000 melkdb-0.2.0/setup.py
```

### Comparing `melkdb-0.1.0/LICENSE` & `melkdb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `melkdb-0.1.0/PKG-INFO` & `melkdb-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melkdb
-Version: 0.1.0
+Version: 0.2.0
 Summary: MelkDB: A faster key-value database
 Home-page: https://github.com/jaedsonpys/melkdb
 Author: Jaedson Silva
 Author-email: jaedson.dev@proton.me
 License: MIT License
 Project-URL: License, https://github.com/jaedsonpys/melkdb/blob/master/LICENSE
 Project-URL: Documentation, https://github.com/jaedsonpys/melkdb/tree/master/docs
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Database Engines/Servers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **MelkDB**: Um banco de dados veloz e otimizado
 
-MelkDB é um banco de dados modelo key-value desenvolvido totalmente em Python. Com seu funcionamento bem documentado, O MelkDB é fácil de usar e pode ser instalado facilmente em sistemas operacionais baseados em Linux e no Windows.
+MelkDB é um banco de dados baseado em diretório desenvolvido totalmente em Python. Com seu funcionamento bem documentado, O MelkDB é fácil de usar e pode ser instalado facilmente em sistemas operacionais baseados em Linux e no Windows.
 
 1. **Obtenha os dados rapidamente**: Desenvolvido para ser extremamente veloz na escrita e leitura de dados, o MelkDB possui um método eficiente para realizar a busca de items, além de ter um código bem otimizado.
 2. **Mantenha seus dados seguros**: O MelkDB oferece a opção de criptografia de dados usando AES-256, protegendo seus dados e mantendo a velocidade ao adicionar e obter items.
 3. **Baixo consumo de memória**: Apenas os dados solicitados pelo usuário são carregados na memória, evitando o alto consumo de memória ao realizar operações no banco de dados. 
 
 ## ⚡ A velocidade do MelkDB
 
@@ -50,27 +50,19 @@
 ```
 
 Finalizando a instalação, o banco de dados MelkDB já está pronto para ser utilizado. Veja abaixo um simples exemplo de uso:
 
 ```python
 from melkdb import MelkDB
 
-db = MelkDB('cache')
+db = MelkDB('users')
 
-# adicionando um item
-db.add("latest_news", "Conteúdo das últimas notícias")
-
-# atualizando um item
-db.update("latest_news", "MelkDB é lançado oficialmente")
-
-# obtendo um item
-print(db.get("latest_news"))
-
-# deletando um item
-db.delete("latest_news")
+db.add('users/melk/name', 'Melk')
+db.add('users/melk/age', 18)
+db.add('users/melk/isTheBestCat', True)
 ```
 
 Veja a [documentação completa](https://github.com/jaedsonpys/melkdb/tree/master/docs) para aprender mais sobre o funcionamento e métodos disponíveis para uso do MelkDB.
 
 ## Licença de uso
 
 Este projeto utiliza a **licença MIT**. Por favor, considere [ler o documento LICENSE](https://github.com/jaedsonpys/melkdb/blob/master/LICENSE) para obter mais informações sobre o uso adequado deste projeto!
```

### Comparing `melkdb-0.1.0/README.md` & `melkdb-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **MelkDB**: Um banco de dados veloz e otimizado
 
-MelkDB é um banco de dados modelo key-value desenvolvido totalmente em Python. Com seu funcionamento bem documentado, O MelkDB é fácil de usar e pode ser instalado facilmente em sistemas operacionais baseados em Linux e no Windows.
+MelkDB é um banco de dados baseado em diretório desenvolvido totalmente em Python. Com seu funcionamento bem documentado, O MelkDB é fácil de usar e pode ser instalado facilmente em sistemas operacionais baseados em Linux e no Windows.
 
 1. **Obtenha os dados rapidamente**: Desenvolvido para ser extremamente veloz na escrita e leitura de dados, o MelkDB possui um método eficiente para realizar a busca de items, além de ter um código bem otimizado.
 2. **Mantenha seus dados seguros**: O MelkDB oferece a opção de criptografia de dados usando AES-256, protegendo seus dados e mantendo a velocidade ao adicionar e obter items.
 3. **Baixo consumo de memória**: Apenas os dados solicitados pelo usuário são carregados na memória, evitando o alto consumo de memória ao realizar operações no banco de dados. 
 
 ## ⚡ A velocidade do MelkDB
 
@@ -26,27 +26,19 @@
 ```
 
 Finalizando a instalação, o banco de dados MelkDB já está pronto para ser utilizado. Veja abaixo um simples exemplo de uso:
 
 ```python
 from melkdb import MelkDB
 
-db = MelkDB('cache')
+db = MelkDB('users')
 
-# adicionando um item
-db.add("latest_news", "Conteúdo das últimas notícias")
-
-# atualizando um item
-db.update("latest_news", "MelkDB é lançado oficialmente")
-
-# obtendo um item
-print(db.get("latest_news"))
-
-# deletando um item
-db.delete("latest_news")
+db.add('users/melk/name', 'Melk')
+db.add('users/melk/age', 18)
+db.add('users/melk/isTheBestCat', True)
 ```
 
 Veja a [documentação completa](https://github.com/jaedsonpys/melkdb/tree/master/docs) para aprender mais sobre o funcionamento e métodos disponíveis para uso do MelkDB.
 
 ## Licença de uso
 
 Este projeto utiliza a **licença MIT**. Por favor, considere [ler o documento LICENSE](https://github.com/jaedsonpys/melkdb/blob/master/LICENSE) para obter mais informações sobre o uso adequado deste projeto!
```

### Comparing `melkdb-0.1.0/melkdb/_item.py` & `melkdb-0.2.0/melkdb/_item.py`

 * *Files identical despite different names*

### Comparing `melkdb-0.1.0/melkdb/crypto.py` & `melkdb-0.2.0/melkdb/crypto.py`

 * *Files identical despite different names*

### Comparing `melkdb-0.1.0/melkdb/exceptions.py` & `melkdb-0.2.0/melkdb/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,7 +32,17 @@
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class ItemNotExistsError(Exception):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
+
+
+class KeyIsATreeError(Exception):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
+
+
+class ItemIsNotATreeError(Exception):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
```

### Comparing `melkdb-0.1.0/melkdb/melkdb.py` & `melkdb-0.2.0/melkdb/melkdb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import json
+import shutil
 
 from typing import Union
 from pathlib import Path
 
 from .__version__ import __version__
 from .crypto import Cryptography
 from .exceptions import *
@@ -74,14 +75,36 @@
             current_major_v = __version__.split('.')[0]
             db_major_v = db_version.split('.')[0]
 
             if current_major_v != db_major_v:
                 raise IncompatibleDatabaseError(f'{repr(name)} created with {db_major_v}.x.x'
                                                  'MelkDB version')
 
+    def _add_tree(self, key_parts: list, value: Union[str, int, float, bool]) -> None:
+        key_parts_len = len(key_parts)
+        sub_block_path = None
+
+        for index, kp in enumerate(key_parts):
+            block = self._block.make_path(kp, previous_path=sub_block_path)
+
+            if index == (key_parts_len - 1):
+                data_path = os.path.join(block, kp)
+            else:
+                sub_block_path = os.path.join(block, kp)
+
+                if os.path.isfile(sub_block_path):
+                    raise ItemIsNotATreeError(f'Item {repr(kp)} is not a tree')
+
+                if not os.path.isdir(sub_block_path):
+                    os.mkdir(sub_block_path)
+
+        with open(data_path, 'wb') as f:
+            item = self._item.encode(value)
+            f.write(item)
+
     def add(self, key: str, value: Union[str, int, float, bool]) -> None:
         """Add a item to database.
 
         :param key: Item key
         :type key: str
         :param value: Item value
         :type value: Union[str, int, float, bool]
@@ -91,20 +114,25 @@
 
         if not isinstance(key, str):
             raise KeyIsNotAStringError('The key must be a string')
 
         if not utils.key_is_valid(key):
             raise InvalidCharInKeyError(f'Key {repr(key)} is not valid')
 
-        block_path = self._block.make_path(key)
-        data_path = os.path.join(block_path, key)
-        item = self._item.encode(value)
+        key_parts = [p for p in key.split('/') if p]
 
-        with open(data_path, 'wb') as f:
-            f.write(item)
+        if len(key_parts) > 1:
+            self._add_tree(key_parts, value)
+        else:
+            block_path = self._block.make_path(key)
+            data_path = os.path.join(block_path, key)
+            item = self._item.encode(value)
+
+            with open(data_path, 'wb') as f:
+                f.write(item)
 
     def get(self, key: str) -> Union[None, str, int, float, bool]:
         """Get a item from database
 
         :param key: Item key
         :type key: str
         :raises KeyIsNotAStringError: If key is not a string
@@ -115,22 +143,29 @@
 
         if not isinstance(key, str):
             raise KeyIsNotAStringError('The key must be a string')
         
         if not utils.key_is_valid(key):
             raise InvalidCharInKeyError(f'Key {repr(key)} is not valid')
 
-        key_path = self._block.get_path(key)
-        data_file_path = os.path.join(key_path, key)
+        key_parts = [p for p in key.split('/') if p]
+
+        if len(key_parts) > 1:
+            data_file_path = self._block.get_tree_path(key_parts)
+        else:
+            key_path = self._block.get_path(key)
+            data_file_path = os.path.join(key_path, key)
 
         if os.path.isfile(data_file_path):
             with open(data_file_path, 'rb') as f:
                 value = self._item.decode(f)
 
             return value
+        elif os.path.isdir(data_file_path):
+            raise KeyIsATreeError(f'you can\'t get the full {repr(key)} tree')
 
     def delete(self, key: str) -> None:
         """Delete a item from database
 
         A exception must be raised if item
         not exists in database.
 
@@ -143,19 +178,26 @@
         
         if not isinstance(key, str):
             raise KeyIsNotAStringError('The key must be a string')
         
         if not utils.key_is_valid(key):
             raise InvalidCharInKeyError(f'Key {repr(key)} is not valid')
 
-        key_path = self._block.get_path(key)
-        data_file_path = os.path.join(key_path, key)
+        key_parts = [p for p in key.split('/') if p]
+
+        if len(key_parts) > 1:
+            data_file_path = self._block.get_tree_path(key_parts)
+        else:
+            key_path = self._block.get_path(key)
+            data_file_path = os.path.join(key_path, key)
 
         if os.path.isfile(data_file_path):
             os.remove(data_file_path)
+        elif os.path.isdir(data_file_path):
+            shutil.rmtree(data_file_path, ignore_errors=True)
         else:
             raise ItemNotExistsError(f'Item {repr(key)} not exists')
 
     def update(self, key: str, value: Union[str, int, float, bool]) -> None:
         """Update a item in database.
 
         This method is just a shortcut to use
```

### Comparing `melkdb-0.1.0/melkdb.egg-info/PKG-INFO` & `melkdb-0.2.0/melkdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melkdb
-Version: 0.1.0
+Version: 0.2.0
 Summary: MelkDB: A faster key-value database
 Home-page: https://github.com/jaedsonpys/melkdb
 Author: Jaedson Silva
 Author-email: jaedson.dev@proton.me
 License: MIT License
 Project-URL: License, https://github.com/jaedsonpys/melkdb/blob/master/LICENSE
 Project-URL: Documentation, https://github.com/jaedsonpys/melkdb/tree/master/docs
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Database Engines/Servers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **MelkDB**: Um banco de dados veloz e otimizado
 
-MelkDB é um banco de dados modelo key-value desenvolvido totalmente em Python. Com seu funcionamento bem documentado, O MelkDB é fácil de usar e pode ser instalado facilmente em sistemas operacionais baseados em Linux e no Windows.
+MelkDB é um banco de dados baseado em diretório desenvolvido totalmente em Python. Com seu funcionamento bem documentado, O MelkDB é fácil de usar e pode ser instalado facilmente em sistemas operacionais baseados em Linux e no Windows.
 
 1. **Obtenha os dados rapidamente**: Desenvolvido para ser extremamente veloz na escrita e leitura de dados, o MelkDB possui um método eficiente para realizar a busca de items, além de ter um código bem otimizado.
 2. **Mantenha seus dados seguros**: O MelkDB oferece a opção de criptografia de dados usando AES-256, protegendo seus dados e mantendo a velocidade ao adicionar e obter items.
 3. **Baixo consumo de memória**: Apenas os dados solicitados pelo usuário são carregados na memória, evitando o alto consumo de memória ao realizar operações no banco de dados. 
 
 ## ⚡ A velocidade do MelkDB
 
@@ -50,27 +50,19 @@
 ```
 
 Finalizando a instalação, o banco de dados MelkDB já está pronto para ser utilizado. Veja abaixo um simples exemplo de uso:
 
 ```python
 from melkdb import MelkDB
 
-db = MelkDB('cache')
+db = MelkDB('users')
 
-# adicionando um item
-db.add("latest_news", "Conteúdo das últimas notícias")
-
-# atualizando um item
-db.update("latest_news", "MelkDB é lançado oficialmente")
-
-# obtendo um item
-print(db.get("latest_news"))
-
-# deletando um item
-db.delete("latest_news")
+db.add('users/melk/name', 'Melk')
+db.add('users/melk/age', 18)
+db.add('users/melk/isTheBestCat', True)
 ```
 
 Veja a [documentação completa](https://github.com/jaedsonpys/melkdb/tree/master/docs) para aprender mais sobre o funcionamento e métodos disponíveis para uso do MelkDB.
 
 ## Licença de uso
 
 Este projeto utiliza a **licença MIT**. Por favor, considere [ler o documento LICENSE](https://github.com/jaedsonpys/melkdb/blob/master/LICENSE) para obter mais informações sobre o uso adequado deste projeto!
```

### Comparing `melkdb-0.1.0/setup.py` & `melkdb-0.2.0/setup.py`

 * *Files identical despite different names*

