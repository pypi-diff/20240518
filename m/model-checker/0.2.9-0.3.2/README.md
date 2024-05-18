# Comparing `tmp/model_checker-0.2.9.tar.gz` & `tmp/model_checker-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.2.9.tar", last modified: Mon May  6 22:32:57 2024, max compression
+gzip compressed data, was "model_checker-0.3.2.tar", last modified: Sat May 18 15:07:14 2024, max compression
```

## Comparing `model_checker-0.2.9.tar` & `model_checker-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.401485 model_checker-0.2.9/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.9/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 22:32:57.401485 model_checker-0.2.9/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.9/README.md
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.401485 model_checker-0.2.9/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      456 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       67 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        4 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/top_level.txt
--rw-r--r--   0 benjamin  (1000) users      (100)      907 2024-05-06 22:32:22.000000 model_checker-0.2.9/pyproject.toml
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.400485 model_checker-0.2.9/scr/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.401485 model_checker-0.2.9/scr/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 21:38:54.000000 model_checker-0.2.9/scr/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    16026 2024-05-06 22:19:35.000000 model_checker-0.2.9/scr/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 22:19:35.000000 model_checker-0.2.9/scr/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-06 22:19:35.000000 model_checker-0.2.9/scr/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-06 21:11:53.000000 model_checker-0.2.9/scr/model_checker/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-06 22:32:06.000000 model_checker-0.2.9/scr/model_checker/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 22:32:57.401485 model_checker-0.2.9/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:07:14.707068 model_checker-0.3.2/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.2/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:07:14.706067 model_checker-0.3.2/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     4662 2024-05-12 17:17:50.000000 model_checker-0.3.2/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)      925 2024-05-18 15:06:54.000000 model_checker-0.3.2/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-18 15:07:14.707068 model_checker-0.3.2/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:07:14.705067 model_checker-0.3.2/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:07:14.706067 model_checker-0.3.2/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)       86 2024-05-08 21:34:17.000000 model_checker-0.3.2/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-18 15:02:56.000000 model_checker-0.3.2/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19680 2024-05-18 15:02:56.000000 model_checker-0.3.2/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    26125 2024-05-18 15:02:56.000000 model_checker-0.3.2/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.2/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.2/src/model_checker/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     1864 2024-05-08 20:49:46.000000 model_checker-0.3.2/src/model_checker/temp.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.2/src/model_checker/test.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:07:14.706067 model_checker-0.3.2/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:07:14.000000 model_checker-0.3.2/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      549 2024-05-18 15:07:14.000000 model_checker-0.3.2/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-18 15:07:14.000000 model_checker-0.3.2/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-18 15:07:14.000000 model_checker-0.3.2/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-18 15:07:14.000000 model_checker-0.3.2/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-18 15:07:14.000000 model_checker-0.3.2/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:07:14.706067 model_checker-0.3.2/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.2/test/test_examples.py
```

### Comparing `model_checker-0.2.9/LICENCE` & `model_checker-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.9/pyproject.toml` & `model_checker-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.2.9"
+version = "0.3.2"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-keywords = ["semantics", "Z3", "counterfactuals", "model checker", "theorem prover"]
+keywords = ["semantics", "Z3", "counterfactuals", "model checker", "theorem prover", "hyperintensionality"]
 dependencies = [
     "z3-solver",
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
 
 [project.scripts]
-model-checker = "model_checker.test_complete:main"
+model-checker = "model_checker.__main__:main"
```

### Comparing `model_checker-0.2.9/scr/model_checker/model_definitions.py` & `model_checker-0.3.2/src/model_checker/model_definitions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 '''
 file contains all definitions for defining the model structure
 '''
 
-import sys
 from z3 import (
     BitVecVal,
     simplify,
 )
 
-from syntax import Infix
-
 def summation(n, func, start = 0):
     '''summation of i ranging from start to n of func(i)
     used in find_all_bits'''
     if start == n:
         return func(start)
     return func(start) + summation(n,func,start+1)
 
-def find_null_bit(size):
-    '''finds the null bit'''
-    return [BitVecVal(0, size)]
+# unused
+# def find_null_bit(size):
+#     '''finds the null bit'''
+#     return [BitVecVal(0, size)]
 
 def find_all_bits(size):
     '''extract all bitvectors from the input model
     imported by model_structure'''
     all_bits = []
     max_bit_number = summation(
         size + 1, lambda x: 2**x
@@ -33,20 +31,20 @@
         if test_bit in all_bits:
         # break once bits start to repeat
             continue
         all_bits.append(test_bit)
     return all_bits
 
 
-def find_poss_bits(model,all_bits, possible):
+def find_poss_bits(z3_model, all_bits, possible):
     '''extract all possible bitvectors from all_bits given the model
     imported by model_structure'''
     poss_bits = []
     for bit in all_bits:
-        if model.evaluate(possible(bit)): # of type/sort BoolRef
+        if z3_model.evaluate(possible(bit)): # of type/sort BoolRef
             poss_bits.append(bit)
     return poss_bits
 
 
 def find_world_bits(poss_bits):
     '''finds the world bits from a list of possible bits.
     used in print_states() and find_relations()'''
@@ -71,70 +69,73 @@
     #     #     raise ValueError(f'{not_world} was not in world_bits but is a world per the model')
     return world_bits
 
 
 def find_compatible_parts(verifier_bit, poss_bits, eval_world):
     """
     Finds the parts of the eval_world compatible with the verifier_bit.
-    Used in find_alt_bits()
+    Used in find_alt_bits() method in ModelStructure class
     """
     comp_parts = []
     for part in poss_bits:
         if bit_fusion(verifier_bit, part) in poss_bits and bit_part(part, eval_world):
             comp_parts.append(part)
             # ie, if fusion is possible and the bit part is in the eval_world
     return comp_parts
 
 
 def find_max_comp_ver_parts(verifier_bit, comp_parts):
     """
     Finds a list of fusions of the verifier_bit and a maximal compatible part.
-    Used in find_alt_bits(), immediately after find_compatible_parts() above.
+    Used in find_alt_bits() method of ModelStructure class,
+    immediately after find_compatible_parts() above.
     """
     not_max_comp_part = []
     for max_part in comp_parts:
         for test in comp_parts:
             if bit_proper_part(max_part, test):
                 not_max_comp_part.append(max_part)
                 break  # continues with the first for loop
     max_comp_parts = [part for part in comp_parts if part not in not_max_comp_part]
     max_comp_ver_parts = [bit_fusion(verifier_bit, max) for max in max_comp_parts]
     return max_comp_ver_parts
 
-def relate_sents_and_states(all_bits, sentence, model, relation):
+def relate_sents_and_states(all_bits, sentence, z3_model, relation):
     """helper function for finding verifier and falsifier states to sentences in a model
-    Used in find_relations()
+    Used in atomic_propositions_dict
     DOES NOT CHECK IF THESE ARE POSSIBLE. """
     relation_set = set()
     for bit in all_bits:
-        if model.evaluate(relation(bit, model[sentence])):
+        if z3_model.evaluate(relation(bit, z3_model[sentence])):
             relation_set.add(bit)
     return relation_set
 
-def find_true_and_false_in_alt(alt_bit, parent_model_structure):
+def find_true_and_false_in_alt(alt_bit, model_structure):
     """returns two sets as a tuple, one being the set of sentences true in the alt world and the other the set being false.
-    Used in Proposition class print_alt_worlds"""
-    extensional_sentences = parent_model_structure.extensional_subsentences
-    # TODO: creates problem with nested counterfactuals
+    Used in evaluate_mainclause_cf_expr()"""
+    extensional_sentences = model_structure.extensional_subsentences
+    # B: is this still true once modal and counterfactual prop_objects include verifiers and falsifiers?
+    # TODO: below creates problem with nested counterfactuals
+    # TODO: I think this was resolved
     # extensional_sentences = parent_model_structure.all_subsentences
-    all_bits = parent_model_structure.all_bits
+    all_bits = model_structure.all_bits
     true_in_alt = []
     for R in extensional_sentences:
         for bit in all_bits:
             # print(model.evaluate(extended_verify(bit, R, evaluate=True), model_completion=True))
             # print(type(model.evaluate(extended_verify(bit, R, evaluate=True), model_completion=True)))
-            if bit in parent_model_structure.find_complex_proposition(R)[0] and bit_part(bit, alt_bit):
+            if bit in find_complex_proposition(model_structure, R, alt_bit)[0] and bit_part(bit, alt_bit):
                 true_in_alt.append(R)
                 break  # returns to the for loop over sentence_letters
     false_in_alt = [R for R in extensional_sentences if not R in true_in_alt] # replace with
     return (repeats_removed(true_in_alt), repeats_removed(false_in_alt))
     # was giving repeats for some reason? Wasn't previously. fixed it up with repeats_removed
 
 
-def make_set_pretty_for_print(set_with_strings):
+def pretty_set_print(set_with_strings):
     """input a set with strings
     print that same set but with no quotation marks around each individual string, and also with the set in order
     returns the set as a string
     Used in print_vers_and_fals() and print_alt_worlds()"""
     sorted_set = sorted(list(set_with_strings))  # actually type list, not set
     print_str = "{"
     for i, elem in enumerate(sorted_set):
@@ -151,43 +152,27 @@
             product_set.add(bit_fusion(a,b))
     return product_set
 
 def coproduct(set_A, set_B):
     A_U_B = set_A.union(set_B)
     return A_U_B.union(product(set_A, set_B))
 
-def atomic_propositions_dict(all_bits, sentence_letters, model, verify, falsify):
+def atomic_propositions_dict_maker(ms_object):
+    all_bits = ms_object.all_bits
+    sentence_letters = ms_object.sentence_letters
+    z3_model = ms_object.z3_model
+    verify = ms_object.verify
+    falsify = ms_object.falsify
     atomic_VFs_dict = {}
     for letter in sentence_letters:
-        ver_bits = relate_sents_and_states(all_bits, letter, model, verify)
-        fal_bits = relate_sents_and_states(all_bits, letter, model, falsify)
+        ver_bits = relate_sents_and_states(all_bits, letter, z3_model, verify)
+        fal_bits = relate_sents_and_states(all_bits, letter, z3_model, falsify)
         atomic_VFs_dict[letter] = (ver_bits, fal_bits)
     return atomic_VFs_dict
 
-def print_alt_relation(alt_relation_set, alt_bit, relation_truth_value, N,output=sys.__stdout__):
-    """true is a string representing the relation ("true" for true_in_alt; m.m. for false) that is being used for
-    alt_relation_set is the set of prefix sentences that have truth value relation_truth_value in a
-    given alternative world alt_bit
-    returns None, only prints
-    Used in print_alt_worlds()"""
-    if not alt_relation_set:
-        return
-    alt_relation_list = sorted([Infix(sent) for sent in alt_relation_set])
-    alt_relation_string = ", ".join(alt_relation_list)
-    if len(alt_relation_set) == 1:
-        print(
-            f"    {alt_relation_string} is {relation_truth_value} in {bitvec_to_substates(alt_bit, N)}",
-            file=output
-        )
-    else:
-        print(
-            f"    {alt_relation_string} are {relation_truth_value} in {bitvec_to_substates(alt_bit, N)}",
-            file=output
-        )
-
 
 #############################################
 ######### MOVED FROM DEFINITIONS.PY #########
 #############################################
         
 
 
@@ -238,15 +223,15 @@
     if integer//2 == 0: # base case: we've reached the end
         remaining_0s_to_tack_on = number - len(new_backwards_str) # to fill in the zeroes
         return '#b' + remaining_0s_to_tack_on * '0' + new_backwards_str[::-1]
     new_int = integer//2
     return int_to_binary(new_int, number, new_backwards_str)
 
 
-# TODO: linter says all or none of the returns should be an expression
+# has to do with printing
 def bitvec_to_substates(bit_vec, N):
     '''converts bitvectors to fusions of atomic states.'''
     bit_vec_as_string = bit_vec.sexpr()
     if 'x' in bit_vec_as_string: # if we have a hexadecimal, ie N=4m
         integer = int(bit_vec_as_string[2:],16)
         bit_vec_as_string = int_to_binary(integer, N)
     bit_vec_backwards = bit_vec_as_string[::-1]
@@ -255,28 +240,43 @@
         if char == "b":
             if not state_repr:
                 return "□"  #  null state
             return state_repr[0 : len(state_repr) - 1]
         if char == "1":
             state_repr += index_to_substate(i)
             state_repr += "."
+    raise ValueError("should have run into 'b' at the end but didn't")
 
-def infix_combine(prem,con):
+def infix_combine(premises, conclusions):
     '''combines the premises with the negation of the conclusion(s).
     premises are infix sentences, and so are the conclusions
-    imported by model_structure'''
-    # if prem is None:
-    #     prem = []
-    input_sent = prem
-    for sent in con:
+    imported by model_structure, in __init__ method of ModelStructure'''
+    input_sentences = premises[:]
+    for sent in conclusions:
         neg_sent = '\\neg ' + sent
-        input_sent.append(neg_sent)
-    return input_sent
-
+        input_sentences.append(neg_sent)
+    return input_sentences
 
+def disjoin_prefix(sentences):
+    """disjoins the list of sentences in prefix form
+    helper for prefix_combine (immediately below)"""
+    if len(sentences) > 2:
+        copy_sentences = sentences[:]
+        first_sent = copy_sentences.pop(0)
+        return ['\\vee ', first_sent, disjoin_prefix(copy_sentences)]
+    # if len(sentences) == 1:
+    #     return sentences[0]
+    return sentences
+
+def prefix_combine(prefix_premises, prefix_conclusions):
+    '''negates and disjoins the prefix conclusions, combining the result with
+    prefix premises to form a new list'''
+    neg_conclusions = [['\\neg ', con] for con in prefix_conclusions]
+    disjoin_neg_conclusions = disjoin_prefix(neg_conclusions)
+    return prefix_premises + disjoin_neg_conclusions
 
 #################################
 ##### MOVED FROM SEMANTICS ######
 #################################
 
 def is_counterfactual(prefix_sentence):
     '''returns a boolean to say whether a given sentence is a counterfactual
@@ -322,59 +322,138 @@
         # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
         left_subsentences = all_subsentences_of_a_sentence(prefix_sentence[1], progress)
         # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
         right_subsentences = all_subsentences_of_a_sentence(prefix_sentence[2], progress)
         all_subsentences = left_subsentences + right_subsentences
         return all_subsentences
 
-# def find_extensional_subsentences(prefix_sentences):
-#         '''finds all the extensional subsentences in a list of prefix sentences
-#         used in find_all_constraints'''
-#         # all_subsentences = [all_subsentences_of_a_sentence(sent) for sent in prefix_sentences]
-#         all_subsentences = []
-#         for prefix_sent in prefix_sentences:
-#             # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-#             all_subsentences.extend(all_subsentences_of_a_sentence(prefix_sent))
-#         extensional_subsentences = [sent for sent in all_subsentences if not is_counterfactual(sent)]
-#         return repeats_removed(extensional_subsentences)
-
-# def find_cf_subsentences(prefix_sentences):
-#     '''finds all the counterfactual subsentences in a list of prefix sentences
-#     used in find_all_constraints'''
-#     # all_subsentences = [all_subsentences_of_a_sentence(sent) for sent in prefix_sentences]
-#     all_subsentences = []
-#     for prefix_sent in prefix_sentences:
-#         # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-#         all_subsentences.extend(all_subsentences_of_a_sentence(prefix_sent))
-#     cf_subsentences = [sent for sent in all_subsentences if is_counterfactual(sent)]
-#     return repeats_removed(cf_subsentences)
-
 def find_subsentences_of_kind(prefix_sentences, kind):
     '''used to find the extensional, modal, and counterfactual sentences. 
     kind is a string, either "extensional", "modal", "counterfactual", or 'all' for a tuple of
     of the three kinds in the order extensional, modal, counterfactual, and then all the subsents
     returns a list of that kind'''
     rr = repeats_removed
     all_subsentences = []
     for prefix_sent in prefix_sentences:
         all_subsentences.extend(all_subsentences_of_a_sentence(prefix_sent))
     if kind == 'extensional':
-        return_list = rr([sent for sent in all_subsentences if is_extensional(sent)])
-    if kind == 'modal': 
-        return_list = rr([sent for sent in all_subsentences if is_modal(sent)])
+        return_list = [sent for sent in all_subsentences if is_extensional(sent)]
+    if kind == 'modal':
+        return_list = [sent for sent in all_subsentences if is_modal(sent)]
     if kind == 'counterfactual':
-        return_list = rr([sent for sent in all_subsentences if is_counterfactual(sent)])
+        return_list = [sent for sent in all_subsentences if is_counterfactual(sent)]
     if kind == 'all':
         counterfactual = rr([sent for sent in all_subsentences if is_counterfactual(sent)])
         modal = rr([sent for sent in all_subsentences if is_modal(sent)])
         extensional = rr([sent for sent in all_subsentences if sent not in counterfactual and sent not in modal])
         return (extensional, modal, counterfactual, all_subsentences)
-    return return_list
+    return rr(return_list)
 
 def repeats_removed(L):
     '''takes a list and removes the repeats in it.
     used in find_all_constraints'''
     seen = []
     for obj in L:
         if obj not in seen:
             seen.append(obj)
     return seen
+
+
+########################################
+###### MOVED FROM model_structure ######
+########################################
+
+def evaluate_modal_expr(model_structure, prefix_modal, eval_world):
+    '''evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
+    used to initialize Counterfactuals
+    returns a bool representing whether the counterfactual is true at the world or not'''
+    op, argument = prefix_modal[0], prefix_modal[1]
+    if is_modal(argument):
+        if model_structure.evaluate_modal_expr(prefix_modal) is True: # ie, verifiers is null state
+            return True # both Box and Diamond will return true, since verifiers is not empty
+        return False
+    if 'Diamond' in op:
+        # TODO: linter error: uninitalized is not iterable  "__iter__" does not return object
+        for poss in model_structure.poss_bits:
+            if poss in find_complex_proposition(model_structure, argument, eval_world)[0]:
+                return True
+        return False
+    if 'Box' in op:
+        # TODO: linter error: uninitalized is not iterable  "__iter__" does not return object
+        for poss in model_structure.poss_bits:
+            if poss in find_complex_proposition(model_structure, argument, eval_world)[1]:
+                return False
+        return True
+
+def evaluate_mainclause_cf_expr(model_structure, prefix_cf, eval_world):
+    """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
+    used to initialize Counterfactuals
+    returns a bool representing whether the counterfactual is true at the world or not
+    """
+    op = prefix_cf[0]
+    assert "boxright" in op, f"{prefix_cf} is not a main-clause counterfactual!"
+    ant_expr, consequent_expr = prefix_cf[1], prefix_cf[2]
+    # assert is_extensional(ant_expr), f"the antecedent {ant_expr} is not extensional!"
+    ant_verifiers = find_complex_proposition(model_structure, ant_expr, eval_world)[0]
+    ant_alts_to_eval_world = model_structure.find_alt_bits(ant_verifiers, eval_world)
+    for u in ant_alts_to_eval_world:
+        # QUESTION: why is string required? Is Z3 removing the lists?
+        if is_counterfactual(consequent_expr):
+            if not find_complex_proposition(model_structure, consequent_expr, u)[0]:
+                return False
+        elif str(consequent_expr) not in str(find_true_and_false_in_alt(u, model_structure)[0]):
+            return False
+    return True
+
+def true_and_false_worlds_for_cf(model_structure, complex_cf_sent):
+    '''used in find_complex_proposition'''
+    worlds_true_at, worlds_false_at = set(), set()
+    for world in model_structure.world_bits:
+        if find_complex_proposition(model_structure, complex_cf_sent, world)[0]:
+            worlds_true_at.add(world)
+            continue
+        worlds_false_at.add(world)
+    return (worlds_true_at, worlds_false_at)
+
+def find_complex_proposition(model_structure, complex_sentence, eval_world):
+    """sentence is a sentence in prefix notation
+    For a given complex proposition, returns the verifiers and falsifiers of that proposition
+    given a solved model
+    for a counterfactual, it'll just give the worlds it's true at and worlds it's not true at
+    """
+    if not model_structure.atomic_props_dict:
+        raise ValueError(
+            "There is nothing in atomic_props_dict yet. Have you actually run the model?"
+        )
+    if len(complex_sentence) == 1:
+        sent = complex_sentence[0]
+        # TODO: linter error: expected 0 arguments
+        return model_structure.atomic_props_dict[sent]
+    op = complex_sentence[0]
+    Y = complex_sentence[1]
+    if "neg" in op:
+        Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
+        return (Y_F, Y_V)
+    null_state = {BitVecVal(0,model_structure.N)}
+    if 'Box' in op or 'Diamond' in op:
+        if evaluate_modal_expr(model_structure, complex_sentence, eval_world):
+            return (null_state, set())
+        return (set(), null_state)
+    Z = complex_sentence[2]
+    Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
+    Z_V, Z_F = find_complex_proposition(model_structure, Z, eval_world)
+    if "wedge" in op:
+        return (product(Y_V, Z_V), coproduct(Y_F, Z_F))
+    if "vee" in op:
+        return (coproduct(Y_V, Z_V), product(Y_F, Z_F))
+    if "leftrightarrow" in op:
+        return (
+            product(coproduct(Y_F, Z_V), coproduct(Y_V, Z_F)),
+            coproduct(product(Y_V, Z_F), product(Y_F, Z_V)),
+        )
+    if "rightarrow" in op:
+        return (coproduct(Y_F, Z_V), product(Y_V, Z_F))
+    if "boxright" in op:
+        if evaluate_mainclause_cf_expr(model_structure, complex_sentence, eval_world):
+            return (null_state, set())
+        return (set(), null_state)
+    raise ValueError(f"Don't know how to handle {op} operator")
```

### Comparing `model_checker-0.2.9/scr/model_checker/model_structure.py` & `model_checker-0.3.2/src/model_checker/model_structure.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,775 +6,585 @@
 import time
 import sys
 from z3 import (
     Function,
     BitVecSort,
     BoolSort,
     BitVec,
+    BitVecVal
 )
+
+# from model_checker.semantics import ( # for packaging
 from semantics import (
     make_constraints,
     solve_constraints,
 )
+# from model_checker.model_definitions import ( # for packaging
 from model_definitions import (
     find_compatible_parts,
-    atomic_propositions_dict,
-    coproduct,
+    atomic_propositions_dict_maker,
     find_all_bits,
     find_max_comp_ver_parts,
-    find_null_bit,
     find_poss_bits,
     find_world_bits,
-    make_set_pretty_for_print,
-    find_true_and_false_in_alt,
-    product,
+    prefix_combine,
+    pretty_set_print,
     bit_part,
     bitvec_to_substates,
     int_to_binary,
-    infix_combine,
     find_subsentences_of_kind,
     is_counterfactual,
-    is_modal,
-
+    true_and_false_worlds_for_cf,
+    find_complex_proposition,
 )
+# from model_checker.syntax import ( # for packaging
 from syntax import (
     AtomSort,
-    Infix,
+    infix,
+    prefix,
+    add_backslashes_to_infix,
 )
 
-# TODO: the three types of objects that it would be good to store as classes
-# include: (1) premises, conclusions, input_sentences, prefix_sentences,
-# prefix_sub_sentences, infix_sub_sentences, sentence_letters, constraints;
-# (2) z3_model, model_status, model_run_time, all_bits, poss_bits, world_bits,
-# eval_world_bit; (3) ext_props_dict, true_in_world_dict, alt_worlds_dict.
-# NOTE: I think we've basically done this no? Just checking—was cleaning up this and other files
-
-# NOTE: the ext_props_dict should associate each extensional prefix_sub_sentence
-# with its infix form, and its proposition. the true_in_world_dict should
-# associate each world with the set of prefix_sub_sentences (extensional or
-# otherwise) that are true in that world. the alt_worlds_dict should associate
-# the antecedent of any counterfactuals with the alternatives to the world of
-# evaluation in question (this will only differ from the eval_world_bit in the
-# case of nested counterfactuals).
-
 inputs_template = Template(
-    """
+'''Run time: ${runtime} seconds
+"""
+
 # path to parent directory
 import os
 parent_directory = os.path.dirname(__file__)
+file_name = os.path.basename(__file__)
 
 # input sentences
 premises = ${premises}
 conclusions = ${conclusions}
 
 # number of atomic states
 N = ${N}
 
 # print all Z3 constraints if a model is found
 print_cons_bool = False
 
 # print core unsatisfiable Z3 constraints if no model exists
 print_unsat_core_bool = True
 
+# print all states including impossible states
+print_impossible_states_bool = False
+
 # present option to save output
 save_bool = False
-
-# use constraints to find models in stead of premises and conclusions
-use_constraints_bool = False
-"""
+'''
 )
 
 
-class Uninitalized:
-    """class for uninitalized attributes"""
-
-    def __init__(self, name):
-        self.name = name
-
-    def __iter__(self):
-        raise AttributeError(
-            f"cannot iterate through {self.name} because it isnt initialized"
-        )
-
-    def __str__(self):
-        return f"{self.name} (uninitialized)"
-
-
-class ModelStructure:
-    """self.premises is a list of prefix sentences
-    self.conclusions is a list of prefix sentences
-    self.input_sentences is the combination of self.premises and self.conclusions with the
-    conclusions negated
-    self.sentence letters is a list of atomic sentence letters (each of sort AtomSort)
-    self.constraints is a list (?) of constraints
-    everything else is initialized as None"""
-
-    def __init__(
-        self, input_premises, input_conclusions, verify, falsify, possible, assign, N, w
-    ):
-        self.verify = verify
-        self.falsify = falsify
-        self.possible = possible
-        self.assign = assign
+# class Uninitalized:
+#     """class for uninitalized attributes"""
+#
+#     def __init__(self, name):
+#         self.name = name
+#
+#     def __iter__(self):
+#         raise AttributeError(
+#             f"cannot iterate through {self.name} because it isnt initialized")
+#
+#     def __getitem__(self):
+#         raise AttributeError(
+#             f"cannot get an item from {self.name} because it isnt initialized")
+#
+#     def __str__(self):
+#         return f"{self.name} (uninitialized)"
+
+class ModelSetup:
+    """class which includes all elements provided by the user as well as those
+    needed to find a model if there is one"""
+
+    def __init__(self, N, infix_premises, infix_conclusions):
+        self.infix_premises = infix_premises
+        self.infix_conclusions = infix_conclusions
         self.N = N
-        self.w = w
-        self.premises = input_premises
-        self.conclusions = input_conclusions
-        self.input_infix_sentences = infix_combine(input_premises, input_conclusions)
+        self.possible = Function("possible", BitVecSort(N), BoolSort())
+        self.verify = Function("verify", BitVecSort(N), AtomSort, BoolSort())
+        self.falsify = Function("falsify", BitVecSort(N), AtomSort, BoolSort())
+        self.assign = Function("assign", BitVecSort(N), AtomSort, BitVecSort(N))
+        self.w = BitVec("w", N) # what will be the main world
+        self.prefix_premises = [prefix(prem) for prem in infix_premises]
+        # M: I think below is a problem
+        self.prefix_conclusions = [prefix(con) for con in infix_conclusions]
+        self.prefix_sentences = prefix_combine(self.prefix_premises, self.prefix_conclusions)
         find_constraints_func = make_constraints(
-            verify, falsify, possible, assign, N, w
+            self.verify,
+            self.falsify,
+            self.possible,
+            self.assign,
+            self.N,
+            self.w
         )
-        consts, sent_lets, input_prefix_sents = find_constraints_func(
-            self.input_infix_sentences
-        )
-        self.sentence_letters = sent_lets
-        self.constraints = consts
-        self.input_prefix_sentences = input_prefix_sents
-        ext, modal, cf, altogether = find_subsentences_of_kind(input_prefix_sents, 'all')
+        constraints, sentence_letters = find_constraints_func(self.prefix_sentences)
+        self.sentence_letters = sentence_letters
+        self.constraints = constraints
+        ext, modal, cf, altogether = find_subsentences_of_kind(self.prefix_sentences, 'all')
         self.extensional_subsentences = ext
         self.counterfactual_subsentences = cf
         self.modal_subsentences = modal
-        self.all_subsentences = altogether
-        # initialize yet-undefined attributes
-        self.model_status = Uninitalized("model_status")
-        self.model = Uninitalized("model")
-        self.model_runtime = Uninitalized("model_runtime")
-        self.null_bit = Uninitalized("null_bit")
-        self.all_bits = Uninitalized("all_bits")
-        self.poss_bits = Uninitalized("poss_bits")
-        self.world_bits = Uninitalized("world_bits")
-        self.eval_world = Uninitalized("eval_world")
-        self.atomic_props_dict = Uninitalized("atomic_props_dict")
-        self.extensional_propositions = Uninitalized("extensional_propositions")
-        self.counterfactual_propositions = Uninitalized("counterfactual_propositions")
-        self.all_propositions = Uninitalized("all_propositions")
-        self.input_propositions = Uninitalized("input_propositions")
+        self.all_subsentences = altogether # in prefix form
+
+    # def constraints_func(self):
+    #     """returns constraints_func"""
+    #     return self.find_constraints_func
 
     def solve(self):
-        """solves the model, returns None
+        """solves for the model, returns None
         self.model is the ModelRef object resulting from solving the model
         self.model_runtime is the runtime of the model as a float
         self.all_bits is a list of all bits (each of sort BitVecVal)
         self.poss_bits is a list of all possible bits
         self.world_bits is a lsit of all world bits
-        self.eval_world is the eval world (as a BitVecVal)
+        self.main_world is the eval world (as a BitVecVal)
         self.atomic_props_dict is a dictionary with keys AtomSorts and keys (V,F)
         """
         model_start = time.time()  # start benchmark timer
-        solved_model_status, solved_model = solve_constraints(self.constraints)
-        self.model_status = solved_model_status
-        self.model = solved_model
+        z3_model_status, z3_model = solve_constraints(self.constraints)
         model_end = time.time()
-        model_total = round(model_end - model_start, 4)
-        self.model_runtime = model_total
+        model_runtime = round(model_end - model_start, 4)
+        return (z3_model_status, z3_model, model_runtime)
+
+
+class ModelStructure:
+    """self.premises is a list of prefix sentences
+    self.conclusions is a list of prefix sentences
+    self.input_sentences is the combination of self.premises and self.conclusions with the
+    conclusions negated
+    self.sentence letters is a list of atomic sentence letters (each of sort AtomSort)
+    self.constraints is a list (?) of constraints
+    everything else is initialized as None"""
+
+    def __init__(self, model_status, model_setup, z3_model, model_runtime):
+        self.model_status = model_status
+        self.model_setup = model_setup
+        self.z3_model = z3_model
+        self.model_runtime = model_runtime
+        self.infix_premises = model_setup.infix_premises
+        self.infix_conclusions = model_setup.infix_conclusions
+        self.N = model_setup.N
+        self.prefix_premises = [prefix(prem) for prem in model_setup.infix_premises]
+        # M: I think below is a problem
+        self.prefix_conclusions = [prefix(con) for con in model_setup.infix_conclusions]
+        self.prefix_sentences = prefix_combine(self.prefix_premises, self.prefix_conclusions)
+
+    def build_test_file(self, output):
+        """generates a test file from input to be saved"""
+        inputs_data = {
+            "N": self.model_setup.N,
+            "premises": self.infix_premises,
+            "conclusions": self.infix_conclusions,
+            "runtime": self.model_runtime,
+        }
+        inputs_content = inputs_template.substitute(inputs_data)
+        print(inputs_content, file=output)
+
+    def print_enumerate(self, output):
+        """prints the premises and conclusions with numbers"""
+        infix_premises = self.infix_premises
+        infix_conclusions = self.infix_conclusions
+        start_con_num = len(infix_premises) + 1
+        if self.infix_premises:
+            if len(self.infix_premises) < 2:
+                print("Premise:", file=output)
+            else:
+                print("Premises:", file=output)
+            for index, sent in enumerate(self.infix_premises, start=1):
+                print(f"{index}. {sent}", file=output)
+        if infix_conclusions:
+            if len(infix_conclusions) < 2:
+                print("\nConclusion:", file=output)
+            else:
+                print("\nConclusions:", file=output)
+            for index, sent in enumerate(infix_conclusions, start=start_con_num):
+                print(f"{index}. {sent}", file=output)
+
+    def no_model_print(self, print_unsat_core_bool, output=sys.__stdout__):
+        """prints the argument when there is no model with the option to
+        include Z3 constraints."""
+        print(f"There are no {self.N}-models of:\n", file=output)
+        self.print_enumerate(output)
+        print(file=output)
+        if print_unsat_core_bool:
+            self.print_constraints(self.z3_model, output)
+        print(f"Run time: {self.model_runtime} seconds\n", file=output)
+
+    def no_model_save(self, print_unsat_core_bool, output):
+        """saves the arguments to a new file when there is no model with the
+        option to include Z3 constraints."""
+        constraints = self.model_setup.constraints
+        print(f"There are no {self.N}-models of:\n", file=output)
+        self.print_enumerate(output)
+        self.build_test_file(output)
+        if print_unsat_core_bool:
+            print("# Unsatisfiable constraints", file=output)
+            print(f"all_constraints = {constraints}", file=output)
+
+    def print_constraints(self, consts, output=sys.__stdout__):
+        """prints constraints in an numbered list"""
         if self.model_status:
-            self.null_bit = find_null_bit(self.N)
-            self.all_bits = find_all_bits(self.N)
-            self.poss_bits = find_poss_bits(self.model, self.all_bits, self.possible)
-            self.world_bits = find_world_bits(self.poss_bits)
-            self.eval_world = self.model[self.w]
-            self.atomic_props_dict = atomic_propositions_dict(
-                self.all_bits,
-                self.sentence_letters,
-                self.model,
-                self.verify,
-                self.falsify,
-            )
-            self.extensional_propositions = [Extensional(ext_subsent, self, self.eval_world)
-                                            for ext_subsent in self.extensional_subsentences]
-            self.counterfactual_propositions = [Counterfactual(cf_subsent, self, self.eval_world)
-                                            for cf_subsent in self.counterfactual_subsentences]
-            self.modal_propositions = [
-                Modal(modal_subsent, self, self.eval_world)
-                for modal_subsent in self.modal_subsentences
-            ]
-            self.all_propositions = (self.extensional_propositions +
-                                     self.counterfactual_propositions + self.modal_propositions)
-            self.input_propositions = self.find_input_propositions()
-            # just missing the which-sentences-true-in-which-worlds
-        # else: # NOTE: maybe these should be defined as something for the sake of init above
+            print("Satisfiable constraints:\n", file=output)
+        else:
+            print("Unsatisfiable core constraints:\n", file=output)
+        for index, con in enumerate(consts, start=1):
+            print(f"{index}. {con}\n", file=output)
+            # print(f"Constraints time: {time}\n")
+
 
-    def find_alt_bits(self, proposition_verifier_bits, comparison_world=None):
+class StateSpace:
+    """class for all states and their attributes"""
+
+    def __init__(self, model_setup, model_structure):
+        self.model_setup = model_setup
+        self.model_structure = model_structure
+        self.z3_model = model_structure.z3_model
+        self.model_runtime = model_structure.model_runtime
+        self.model_status = model_structure.model_status
+        self.N = model_setup.N
+        self.main_world = model_setup.w
+        self.all_bits = find_all_bits(self.N)
+        self.poss_bits = find_poss_bits(self.z3_model, self.all_bits, model_setup.possible)
+        self.world_bits = find_world_bits(self.poss_bits)
+        self.main_world = self.z3_model[self.main_world]
+        self.sentence_letters = model_setup.sentence_letters
+        self.verify = model_setup.verify
+        self.falsify = model_setup.falsify
+        self.atomic_props_dict = atomic_propositions_dict_maker(self)
+
+        # TODO: one attribute for all propositions (check)
+        # self.all_subsentences = model_setup.all_subsentences
+        self.extensional_subsentences = model_setup.extensional_subsentences
+        self.extensional_propositions = [Proposition(ext_subsent, self, self.main_world)
+                                        for ext_subsent in model_setup.extensional_subsentences]
+        self.counterfactual_propositions = [Proposition(cf_subsent, self, self.main_world)
+                                        for cf_subsent in model_setup.counterfactual_subsentences]
+        self.modal_propositions = [Proposition(modal_subsent, self, self.main_world)
+                                    for modal_subsent in model_setup.modal_subsentences]
+        self.all_propositions = (self.extensional_propositions +
+                                 self.counterfactual_propositions + self.modal_propositions)
+        self.premise_propositions = self.find_propositions(model_structure.prefix_premises, True)
+        self.conclusion_propositions = self.find_propositions(model_structure.prefix_conclusions, True)
+
+    def find_alt_bits(self, verifier_bits, evaulation_world=None):
         """
-        Finds the alternative bits given verifier bits, possible states, worlds, and
-        the evaluation world. Used in Proposition class alternative worlds and Proposition
-        class attribute update_comparison_world().
+        Finds the alternative bits given verifier bits of an extensional proposition,
+        possible states, worlds, and the evaluation world.
+        Used in evaluate_cf_expression() and rec_print().
         """
-        if comparison_world is None:
-            comparison_world = self.eval_world
+        if evaulation_world is None:
+            evaulation_world = self.main_world
         alt_bits = set()
-        for ver in proposition_verifier_bits:
-            comp_parts = find_compatible_parts(ver, self.poss_bits, comparison_world)
+        for ver in verifier_bits:
+            comp_parts = find_compatible_parts(ver, self.poss_bits, evaulation_world)
             max_comp_ver_parts = find_max_comp_ver_parts(ver, comp_parts)
-            # TODO: linter error: "Uninitalized" is not iterable   "__iter__" method does not return an object
             for world in self.world_bits:
                 if not bit_part(ver, world):
                     continue
                 for max_ver in max_comp_ver_parts:
-                    if bit_part(max_ver, world) and world.sexpr():
+                    if bit_part(max_ver, world):
                         alt_bits.add(world)
                         break  # to return to the second for loop over world_bits
         return alt_bits
 
-    def evaluate_modal_expr(self, prefix_modal):
-        '''evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
-        used to initialize Counterfactuals
-        returns a bool representing whether the counterfactual is true at the world or not'''
-        op, argument = prefix_modal[0], prefix_modal[1]
-        if is_modal(argument):
-            if self.evaluate_modal_expr(prefix_modal) is True: # ie, verifiers is all worlds
-                return True # both Box and Diamond will return true, since verifiers is not empty
-            return False
-        if 'Diamond' in op:
-            for world in self.world_bits:
-                if world in self.find_complex_proposition(argument)[0]:
-                    return True
-            return False
-        if 'Box' in op:
-            for world in self.world_bits:
-                if world not in self.find_complex_proposition(argument)[0]:
-                    return False
-            return True
-
-    def evaluate_cf_expr(self, prefix_cf, eval_world):
-        """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
-        used to initialize Counterfactuals
-        returns a bool representing whether the counterfactual is true at the world or not
-        """
-        op, antecedent_expr, consequent_expr = prefix_cf[0], prefix_cf[1], prefix_cf[2]
-        assert "boxright" in op, f"{prefix_cf} is not a counterfactual!"
-        ant_prop = self.find_proposition_object(antecedent_expr, ext_only=True)
-        ant_prop.update_comparison_world(eval_world)
-        for u in ant_prop["alternative worlds"]:
-            # print(type(consequent_expr))
-            # print(type(find_true_and_false_in_alt(u, self)))
-            # QUESTION: why is string required? Is Z3 removing the lists?
-            if is_counterfactual(consequent_expr):
-                if self.evaluate_cf_expr(consequent_expr, u) is False:
-                    return False
-            elif str(consequent_expr) not in str(find_true_and_false_in_alt(u, self)[0]):
-                return False
-        return True
-
-    def find_complex_proposition(self, complex_sentence):
-        """sentence is a sentence in prefix notation
-        For a given complex proposition, returns the verifiers and falsifiers of that proposition
-        given a solved model
-        for a counterfactual, it'll just give the worlds it's true at and worlds it's not true at
-        """
-        # if 'boxright' in complex_sentence:
-        #     raise ValueError("There is no proposition for non-extensional sentences.")
-        if not self.atomic_props_dict:
-            raise ValueError(
-                "There is nothing in atomic_props_dict yet. Have you actually run the model?"
-            )
-        if len(complex_sentence) == 1:
-            sent = complex_sentence[0]
-            # TODO: linter error: "__getitem__" method not defined on type "Uninitalized"
-            return self.atomic_props_dict[sent]
-        op = complex_sentence[0]
-        Y = complex_sentence[1]
-        if "neg" in op:
-            Y_V = self.find_complex_proposition(Y)[0]
-            Y_F = self.find_complex_proposition(Y)[1]
-            return (Y_F, Y_V)
-        if 'Box' in op:
-            if not self.evaluate_modal_expr(complex_sentence):
-                return (set(), set(self.world_bits))
-            return (set(self.world_bits), set())
-        if 'Diamond' in op:
-            if self.evaluate_modal_expr(complex_sentence):
-                return (set(self.world_bits), set())
-            return (set(), set(self.world_bits))
-        Z = complex_sentence[2]
-        Y_V = self.find_complex_proposition(Y)[0]
-        Y_F = self.find_complex_proposition(Y)[1]
-        Z_V = self.find_complex_proposition(Z)[0]
-        Z_F = self.find_complex_proposition(Z)[1]
-        if "wedge" in op:
-            return (product(Y_V, Z_V), coproduct(Y_F, Z_F))
-        if "vee" in op:
-            return (coproduct(Y_V, Z_V), product(Y_F, Z_F))
-        if "leftrightarrow" in op:
-            return (
-                product(coproduct(Y_F, Z_V), coproduct(Y_V, Z_F)),
-                coproduct(product(Y_V, Z_F), product(Y_F, Z_V)),
-            )
-        if "rightarrow" in op:
-            return (coproduct(Y_F, Z_V), product(Y_V, Z_F))
-        # NOTE: could assign the sentence to the worlds which make the
-        # counterfactual true in this final case. should probably call another
-        # function here which finds that set of worlds if we go this route.
-        if "boxright" in op:
-            worlds_true_at = set()
-            for world in self.world_bits:
-                if self.evaluate_cf_expr(complex_sentence, world):
-                    worlds_true_at.add(world)
-            worlds_false_at = {
-                world for world in self.world_bits if world not in worlds_true_at
-            }
-            return (worlds_true_at, worlds_false_at)
-        raise ValueError(f"Don't know how to handle {op} operator")
-
-    def find_proposition_object(self, prefix_expression, ext_only=False):
-        """given a prefix sentence, finds the Proposition object in the model that corresponds
+    # Useful to user now that can search an infix expression
+    def find_proposition_object(self, expression, prefix_search=False):
+        """given a sentence, finds the Proposition object in the model that corresponds
         to it. Can optionally search through only the extensional sentences
+        Also defaults to searching an infix sentence, though internally it always searches
+        prefix. 
+        If search infix, make sure you put double backslashes always!!
         returns a Proposition object"""
-        search_list = self.extensional_propositions
-        if ext_only is False:
-            search_list = self.all_propositions
-        # TODO: linter error: "Uninitalized" is not iterable   "__iter__" method does not return an object
-        for prop in search_list:
-            if prop["prefix expression"] == prefix_expression:
-                return prop
+        search_list = self.all_propositions
+        if prefix_search:
+            for prop_object in search_list:
+                if prop_object["prefix expression"] == expression:
+                    return prop_object
+        else:
+            for prop_object in search_list:
+                if str(prop_object) == add_backslashes_to_infix(expression):
+                    return prop_object
         raise ValueError(
-            f"there is no proposition with prefix expression {prefix_expression}"
-        )
+            f"there is no Proposition with expression {expression}")
 
-    def find_input_propositions(self):
+    # Useful to user now that can search infix expressions
+    def find_propositions(self, sentences, prefix_search=False):
         """finds all the Proposition objects in a ModelStructure
-        that correspond to the input sentences.
+        that correspond to the prefix sentences in sentences.
         returns them as a list"""
-        input_propositions = []
-        for prefix_sent in self.input_prefix_sentences:
-            input_propositions.append(self.find_proposition_object(prefix_sent))
-        return input_propositions
-
-    def print_states(self, output=sys.__stdout__):
-        """print all fusions of atomic states in the model
-        first print function in print.py"""
-        N = self.N
-        print("\nPossible states:", file=output)  # Print states
-        # TODO: linter error: "Uninitalized" is not iterable   "__iter__" method does not return an object
-        for bit in self.all_bits:
-            state = bitvec_to_substates(bit, N)
-            bin_rep = (
-                bit.sexpr()
-                if N % 4 != 0
-                else int_to_binary(int(bit.sexpr()[2:], 16), N)
-            )
-            if bit in self.world_bits:
-                print(f"  {bin_rep} = {state} (world)", file=output)
-            # invalid conditional operand band-aid fixed with bool
-            # TODO: linter error: Cannot access member "evaluate" for type "AstVector"    Member "evalutate" is unknown
-            elif bool(self.model.evaluate(self.possible(bit))):
-                # NOTE: the following comments are to debug
-                # result = self.model.evaluate(possible(bit))
-                # print(type(result))  # Debug to confirm it's a Boolean
-                # result_bool = bool(self.model.evaluate(possible(bit)))
-                # print(type(result_bool))  # Debug to confirm it's a Boolean
-                print(f"  {bin_rep} = {state}", file=output)
-            else:
-                # print(f"  {bin_rep} = {state} (impossible)")
-                continue
+        propositions = []
+        for sent in sentences:
+            propositions.append(self.find_proposition_object(sent, prefix_search=prefix_search))
+        return propositions
 
     def print_evaluation(self, output=sys.__stdout__):
-        """print the evaluation world and all sentences true/false in that world
-        sentence letters is a list
-        second print function in print.py"""
-        N = self.N
+        """print the evaluation world and all sentences letters that true/false
+        in that world"""
+        # TODO: all this seems to do is print the sentences true/false in each world.
+        # can this be simplified? might it make sense to store sentence letters true
+        # at the designated world and the sentence letters false at the designated
+        # world in the class? then those could be easily called here.
+        N = self.model_setup.N
+        sentence_letters = self.sentence_letters
+        main_world = self.main_world
         print(
-            f"\nThe evaluation world is {bitvec_to_substates(self.eval_world, N)}:",
+            f"\nThe evaluation world is {bitvec_to_substates(main_world, N)}:",
             file=output,
         )
         true_in_eval = set()
-        for sent in self.sentence_letters:
-            # TODO: linter error: "Uninitalized" is not iterable   "__iter__" method does not return an object
+        for sent in sentence_letters:
+            # TODO: linter error: "Uninitalized" is not iterable  "__iter__" method does not return an object
             for bit in self.all_bits:
-                # TODO: linter error: "__getitem__" method not defined on type "Uninitalized"
-                ver_bool = self.verify(bit, self.model[sent])
-                part_bool = bit_part(bit, self.eval_world)
+                # TODO: linter error: expected 0 positional arguments
+                ver_bool = self.model_setup.verify(bit, self.z3_model[sent])
+                part_bool = bit_part(bit, main_world)
                 # TODO: linter error: invalid conditional operand band-aid fixed with bool
-                if bool(self.model.evaluate(ver_bool) and part_bool):
+                if bool(self.z3_model.evaluate(ver_bool) and part_bool):
                     true_in_eval.add(sent)
                     break  # exits the first for loop
-        false_in_eval = {R for R in self.sentence_letters if not R in true_in_eval}
+        false_in_eval = {R for R in sentence_letters if not R in true_in_eval}
         if true_in_eval:
             true_eval_list = sorted([str(sent) for sent in true_in_eval])
             true_eval_string = ", ".join(true_eval_list)
             print(
-                f"  {true_eval_string}  (True in {bitvec_to_substates(self.eval_world, N)})",
+                f"  {true_eval_string}  (True in {bitvec_to_substates(main_world, N)})",
                 file=output,
             )
         if false_in_eval:
             false_eval_list = sorted([str(sent) for sent in false_in_eval])
             false_eval_string = ", ".join(false_eval_list)
             print(
-                f"  {false_eval_string}  (Not true in {bitvec_to_substates(self.eval_world, N)})",
+                f"  {false_eval_string}  (False in {bitvec_to_substates(main_world, N)})",
                 file=output,
             )
         print(file=output)
 
-    def print_constraints(self, consts, output=sys.__stdout__):
-        """prints constraints in an numbered list"""
-        for index, con in enumerate(consts, start=1):
-            print(f"{index}. {con}\n", file=output)
-            # print(f"Constraints time: {time}\n")
+    def print_to(self, print_cons_bool, print_impossible, output=sys.__stdout__):
+        """append all elements of the model to the file provided"""
+        self.print_all(print_impossible, output)
+        if print_cons_bool:
+            self.z3_model.print_constraints(self.model_setup.constraints, output)
+        print(f"Run time: {self.model_runtime} seconds\n", file=output)
 
-    def rec_print(self, prop, current_world, output, indent=0):
+    def save_to(self, cons_include, print_impossible, output):
+        """append all elements of the model to the file provided"""
+        constraints = self.model_setup.constraints
+        self.print_all(print_impossible, output)
+        self.model_structure.build_test_file(output)
+        if cons_include:
+            print("# Satisfiable constraints", file=output)
+            # TODO: print constraint objects, not constraint strings
+            print(f"all_constraints = {constraints}", file=output)
+
+    def print_states(self, print_impossible, output=sys.__stdout__):
+        """print all fusions of atomic states in the model
+        first print function in print.py"""
+        N = self.model_setup.N
+        print("\nPossible states:", file=output)  # Print states
+        for bit in self.all_bits:
+            state = bitvec_to_substates(bit, N)
+            bin_rep = (
+                bit.sexpr()
+                if N % 4 != 0
+                else int_to_binary(int(bit.sexpr()[2:], 16), N)
+            )
+            if bit in self.world_bits:
+                print(f"  {bin_rep} = {state} (world)", file=output)
+                continue
+            if bit in self.poss_bits:
+                print(f"  {bin_rep} = {state}", file=output)
+                continue
+            if print_impossible:
+                print(f"  {bin_rep} = {state} (impossible)", file=output)
+
+    def rec_print(self, prop_obj, world_bit, print_impossible, output, indent=0):
         """recursive print function (previously print_sort)
         returns None"""
-        N = self.N
-        indent_num = indent
-        substate_current_world = bitvec_to_substates(current_world, N)
-        substate_prop_comp_world = bitvec_to_substates(prop["comparison world"], N)
-        if substate_prop_comp_world != substate_current_world:
-            prop.update_comparison_world(current_world)
-        if str(prop) in [str(atom) for atom in self.sentence_letters]:
-            prop.print_verifiers_and_falsifiers(current_world, indent_num, output)
+        N = self.model_setup.N
+        sentence_letters = self.sentence_letters
+        prop_obj.print_verifiers_and_falsifiers(world_bit, print_impossible, indent, output)
+        if str(prop_obj) in [str(atom) for atom in sentence_letters]:
             return
-        print(
-            f"{'  ' * indent_num}{prop}  ({prop.truth_value_at(current_world)} in "
-            f"{bitvec_to_substates(current_world, N)})",
-            file=output
-        )
-        prefix_expr = prop["prefix expression"]
+        prefix_expr = prop_obj["prefix expression"]
         op = prefix_expr[0]
-        first_subprop = self.find_proposition_object(prefix_expr[1])
-        # print(f"TEST: {self.find_proposition_object(prefix_expr[1])}")
+        first_subprop = self.find_proposition_object(prefix_expr[1], prefix_search=True)
+        indent += 1 # begin subcases, so indent
         if "neg" in op:
-            indent_num += 1
-            self.rec_print(first_subprop, current_world, output, indent_num)
+            self.rec_print(first_subprop, world_bit, print_impossible, output, indent)
             return
         if 'Diamond' in op or 'Box' in op:
-            indent_num += 1
             for u in self.world_bits:
-                self.rec_print(first_subprop, u, output, indent_num)
+                self.rec_print(first_subprop, u, print_impossible, output, indent)
             return
-        # if 'Box' in op:
-        #     indent_num += 1
-        #     if self.evaluate_modal_expr(prefix_expr):
-        #         self.rec_print(first_subprop, current_world, output, indent_num)
-        #     # modal_prop = self.find_complex_proposition(prefix_expr) 
-        #     for u in self.world_bits:
-        #         self.rec_print(first_subprop, current_world, output, indent_num)
-        #         if 
-        #             self.rec_print(first_subprop, u, output, indent_num)
-        #     return
         left_subprop = first_subprop
-        right_subprop = self.find_proposition_object(prefix_expr[2])
+        right_subprop = self.find_proposition_object(prefix_expr[2], prefix_search=True)
         if "boxright" in op:
-            indent_num += 1
-            assert (
-                left_subprop in self.extensional_propositions
-            ), "{prop} not a valid cf because antecedent {left_subprop} is not extensional"
-            self.rec_print(left_subprop, current_world, output, indent_num)
-            alt_worlds = {bitvec_to_substates(u,N) for u in left_subprop["alternative worlds"]}
+            # assert (
+            #     left_subprop in self.extensional_propositions
+            # ), f"{prop_obj} is not a valid cf because antecedent {left_subprop} is not extensional"
+            left_subprop_vers = left_subprop['verifiers']
+            phi_alt_worlds_to_world_bit = self.find_alt_bits(left_subprop_vers, world_bit)
+            alt_worlds_as_strings = {bitvec_to_substates(u,N) for u in phi_alt_worlds_to_world_bit}
+            self.rec_print(left_subprop, world_bit, print_impossible, output, indent)
             print(
-                f'{"  " * indent_num}'
-                f'{left_subprop}-alternatives to {bitvec_to_substates(current_world, N)} = '
-                f'{make_set_pretty_for_print(alt_worlds)}',
+                f'{"  " * indent}'
+                f'{left_subprop}-alternatives to {bitvec_to_substates(world_bit, N)} = '
+                f'{pretty_set_print(alt_worlds_as_strings)}',
                 file=output
             )
-            indent_num += 1
-            for u in left_subprop["alternative worlds"]:
-                self.rec_print(right_subprop, u, output, indent_num)
-        else:
-            indent_num += 1
-            self.rec_print(left_subprop, current_world, output, indent_num)
-            self.rec_print(right_subprop, current_world, output, indent_num)
+            indent += 1
+            for u in phi_alt_worlds_to_world_bit:
+                self.rec_print(right_subprop, u, print_impossible, output, indent)
+            return
+        self.rec_print(left_subprop, world_bit, print_impossible, output, indent)
+        self.rec_print(right_subprop, world_bit, print_impossible, output, indent)
 
-    def print_inputs_recursively(self, output):
+    def print_inputs_recursively(self, print_impossible, output):
         """does rec_print for every proposition in the input propositions
         returns None"""
-        initial_eval_world = self.eval_world
-        # TODO: linter error: "Uninitalized" is not iterable   "__iter__" method does not return an object
-        # for input_prop in self.input_propositions:
-        for index, input_prop in enumerate(self.input_propositions, start=1):
-            print(f"{index}.", end="", file=output)
-            self.rec_print(input_prop, initial_eval_world, output, 1)
-            print(file=output)
-
-    # TODO: how can print_to and save_to be cleaned up and made less redundant?
-    def print_to(self, print_cons_bool, print_unsat_core_bool, output=sys.__stdout__):
-        """append all elements of the model to the file provided"""
-        N = self.N
-        if self.model_status:
+        initial_eval_world = self.main_world
+        infix_premises = self.model_setup.infix_premises
+        infix_conclusions = self.model_setup.infix_conclusions
+        start_con_num = len(infix_premises) + 1
+        if self.premise_propositions:
+            if len(infix_premises) < 2:
+                print("Interpreted premise:\n", file=output)
+            else:
+                print("Interpreted premises:\n", file=output)
+            for index, input_prop in enumerate(self.premise_propositions, start=1):
+                print(f"{index}.", end="", file=output)
+                self.rec_print(input_prop, initial_eval_world, print_impossible, output, 1)
+                print(file=output)
+        if self.conclusion_propositions:
+            if len(infix_conclusions) < 2:
+                print("Interpreted conclusion:\n", file=output)
+            else:
+                print("Interpreted conclusions:\n", file=output)
+            for index, input_prop in enumerate(self.conclusion_propositions, start=start_con_num):
+                print(f"{index}.", end="", file=output)
+                self.rec_print(input_prop, initial_eval_world, print_impossible, output, 1)
+                print(file=output)
+
+    def print_all(self, print_impossible, output):
+        """prints states, sentence letters evaluated at the designated world and
+        recursively prints each sentence and its parts"""
+        N = self.model_setup.N
+        print(f"There is a {N}-model of:\n", file=output)
+        self.model_structure.print_enumerate(output)
+        self.print_states(print_impossible, output)
+        self.print_evaluation(output)
+        self.print_inputs_recursively(print_impossible, output)
 
-            print(f"\nThere is a {N}-model of:\n", file=output)
-            for index, sent in enumerate(self.input_infix_sentences, start=1):
-                print(f"{index}. {sent}", file=output)
-            self.print_states(output)
-            self.print_evaluation(output)
-            # self.print_props(output)
-            self.print_inputs_recursively(output)
-            if print_cons_bool:
-                print("Satisfiable constraints:\n", file=output)
-                self.print_constraints(self.constraints, output)
-        else:
-            print(f"\nThere are no {N}-models of:\n", file=output)
-            for index, sent in enumerate(self.input_infix_sentences, start=1):
-                print(f"{index}. {sent}", file=output)
-            print(file=output)
-            if print_unsat_core_bool:
-                print("Unsatisfiable core constraints:\n", file=output)
-                self.print_constraints(self.model, output)
-        print(f"Run time: {self.model_runtime} seconds\n", file=output)
 
-    def save_to(self, doc_name, cons_include, output):
-        """append all elements of the model to the file provided"""
-        if self.model_status:
-            print(f"# TITLE: {doc_name}\n", file=output)
-            print('"""', file=output)
-            print(f"There is a {self.N}-model of:\n", file=output)
-            for sent in self.input_infix_sentences:
-                print(sent, file=output)
-            self.print_states(output)
-            self.print_evaluation(output)
-            # self.print_props(output)
-            self.print_inputs_recursively(output)
-            print(f"Run time: {self.model_runtime} seconds", file=output)
-            print('"""', file=output)
-            inputs_data = {
-                "N": self.N,
-                "premises": self.premises,
-                "conclusions": self.conclusions,
-            }
-            inputs_content = inputs_template.substitute(inputs_data)
-            print(inputs_content, file=output)
-            if cons_include:
-                print("\n# satisfiable constraints", file=output)
-                # TODO: print constraint objects, not constraint strings
-                print(f"all_constraints = {self.constraints}", file=output)
-        else:
-            print(f"# TITLE: {doc_name}\n", file=output)
-            print('"""', file=output)
-            print(f"\nThere are no {self.N}-models of:\n", file=output)
-            for sent in self.input_infix_sentences:
-                print(sent, file=output)
-            print("\n# unsatisfiable core constraints", file=output)
-            self.print_constraints(self.model, output)
-            print('"""', file=output)
-            print(
-                inputs_block, file=output
-            )  # TODO: looks like inputs_block is undefined
-            if cons_include:
-                print(f"all_constraints = {self.constraints}", file=output)
 
 
 class Proposition:
     """class for propositions to store their verifiers, falsifiers, alt worlds, etc
     has two subclasses Extensional and Counterfactual—Counterfactual is a Proposition
     subclass to make stuff easier"""
 
-    def __init__(self, prefix_expr, model_structure, world):
-        """prefix_expr is a prefix expression. model is a ModelStructure"""
+    def __init__(self, prefix_expr, model_structure, eval_world):
+        """for modals and counterfactuals, if they're true then the verifiers
+        are only the null state and falsifiers are nothing; if they're false the opposite"""
         self.prop_dict = {}
-        self.prop_dict["comparison world"] = world
         self.prop_dict["prefix expression"] = prefix_expr
-        self.parent_model_structure = model_structure
-        (
-            verifiers_in_model,
-            falsifiers_in_model,
-        ) = model_structure.find_complex_proposition(prefix_expr)
-        # for CFs, verifiers are worlds true at and falsifiers are worlds not true at
-        # for modals, same as CFs, except it is either all worlds or no worlds in each
-        self.prop_dict["verifiers"] = verifiers_in_model
-        self.prop_dict["falsifiers"] = falsifiers_in_model
-
-    def update_comparison_world(self, new_world):
-        """updates the comparison world (which is a BitVecVal) to a new one; updates
-        the alt worlds based on that
-        returns None"""
-        if new_world == self["comparison world"]:
-            return
-        model_structure = self.parent_model_structure
-        if isinstance(self, Extensional):
-            self["alternative worlds"] = model_structure.find_alt_bits(
-                self["verifiers"], new_world
-            )
-        self["comparison world"] = new_world
+        self.model_structure = model_structure
+        verifiers, falsifiers = find_complex_proposition(model_structure, prefix_expr, eval_world)
+        self.world_bits = model_structure.world_bits # NOTE: this isn't being called anywhere
+        self.prop_dict["verifiers"] = verifiers
+        self.prop_dict["falsifiers"] = falsifiers
+        # if is_modal(prefix_expr):
+        #     arg = prefix_expr[1]
+        #     arg_worlds, non_arg_worlds = find_complex_proposition(model_structure, arg, eval_world)
+        #     self['arg worlds'] = arg_worlds
+        #     self['non arg worlds'] = non_arg_worlds
+        if is_counterfactual(prefix_expr):
+            self.current_eval_world = eval_world
+            true_worlds, false_worlds = true_and_false_worlds_for_cf(model_structure, prefix_expr)
+            self['worlds cf true at'] = true_worlds
+            self['worlds cf false at'] = false_worlds
 
     def __setitem__(self, key, value):
         self.prop_dict[key] = value
 
     def __getitem__(self, key):
+        '''NOTE: If a user wants to access a modal or counterfactual Proposition's verifiers, 
+        THEY SHOULD NOT. They should instead use the truth_value_at() method'''
         return self.prop_dict[key]
 
     def __str__(self):
-        return Infix(self["prefix expression"])
-
-
-class Extensional(Proposition):
-    """Subclass of Proposition for extensional sentences"""
+        return infix(self["prefix expression"])
 
-    def __init__(self, prefix_expr, model_structure, world):
-        super().__init__(prefix_expr, model_structure, world)
-        self.prop_dict["alternative worlds"] = model_structure.find_alt_bits(
-            self["verifiers"], world
-        )
-
-    def truth_value_at(self, eval_world):
-        """finds whether a CF is true at a certain world
-        returns a Boolean representing yes or no"""
-        for verifier in self["verifiers"]:
-            if bit_part(verifier, eval_world):
-                return True
-        return False
+    def update_verifiers(self, new_world):
+        if not is_counterfactual(self['prefix expression']):
+            raise AttributeError(f'You can only update verifiers for CFs, and {self} is not a CF.')
+        N = self.model_structure.N
+        if new_world == self.current_eval_world:
+            return 
+        if new_world in self['worlds cf true at']:
+            self['verifiers'], self['falsifiers'] = {BitVecVal(0,N)}, set()
+            return
+        self['verifiers'], self['falsifiers'] = set(), {BitVecVal(0,N)}
+        return
 
-    def print_verifiers_and_falsifiers(self, current_world, indent=0, output=sys.__stdout__):
+    def print_verifiers_and_falsifiers(self, eval_world, print_impossible=False, indent=0, output=sys.__stdout__):
         """prints the possible verifiers and falsifier states for a sentence.
-        inputs: the verifier states and falsifier states.
-        Outputs: None, but prints the verifiers and falsifiers
-        Used in print_prop()"""
-        N = self.parent_model_structure.N
-        truth_value = self.truth_value_at(current_world)
+        used in: rec_print() 
+        ensures eval_world is in fact the eval_world for CFs"""
+        N = self.model_structure.N
+        truth_value = self.truth_value_at(eval_world)
+        if self in self.model_structure.counterfactual_propositions:
+            self.update_verifiers(eval_world)
         indent_num = indent
-        possible = self.parent_model_structure.possible
-        model = self.parent_model_structure.model
+        possible = self.model_structure.model_setup.possible
+        z3_model = self.model_structure.z3_model
+        ver_prints = '∅'
         ver_states = {
             bitvec_to_substates(bit, N)
             for bit in self["verifiers"]
-            if model.evaluate(possible(bit))
+            if z3_model.evaluate(possible(bit))
+            or print_impossible
         }
+        if ver_states:
+            ver_prints = pretty_set_print(ver_states)
+        fal_prints = '∅'
         fal_states = {
             bitvec_to_substates(bit, N)
             for bit in self["falsifiers"]
-            if model.evaluate(possible(bit))
+            if z3_model.evaluate(possible(bit))
+            or print_impossible
         }
-        world_state = bitvec_to_substates(current_world, N)
-        if ver_states and fal_states:
-            print(
-                f"{'  ' * indent_num}|{self}| = < {make_set_pretty_for_print(ver_states)}, {make_set_pretty_for_print(fal_states)} >"
-                f"  ({truth_value} in {world_state})",
-                file=output,
-            )
-        elif ver_states and not fal_states:
-            print(
-                f"{'  ' * indent_num}|{self}| = < {make_set_pretty_for_print(ver_states)}, ∅ >"
-                f"  ({truth_value} in {world_state})",
-                file=output,
-            )
-        elif not ver_states and fal_states:
-            print(
-                f"{'  ' * indent_num}|{self}| = < ∅, {make_set_pretty_for_print(fal_states)} >"
-                f"  ({truth_value} in {world_state})",
-                file=output,
-            )
-        else:
-            print(
-                f"{'  ' * indent_num}|{self}| = < ∅, ∅ >"
-                f"({truth_value} in {world_state})", file=output
-            )
-
-    # def print_props(self, output=sys.__stdout__):
-    #     """prints possible verifiers and falsifiers for every extensional proposition
-    #     and also the prop-alt worlds to the main world of evaluation"""
-    #     # test_print = [ext["prefix expression"] for ext in self.extensional_propositions]
-    #     # print(test_print)
-    #     for ext_proposition in self.extensional_propositions:
-    #         # print([bitvec_to_substates(bv, self.N) for bv in ext_proposition["verifiers"]])
-    #         ext_proposition.print_possible_verifiers_and_falsifiers(output)
-    #         ext_proposition.print_alt_worlds(output)
-
-    # def print_possible_verifiers_and_falsifiers(self, output=sys.__stdout__):
-    #     """prints the possible verifiers and falsifier states for a sentence.
-    #     inputs: the verifier states and falsifier states.
-    #     Outputs: None, but prints the verifiers and falsifiers
-    #     Used in print_prop()"""
-    #     N = self.parent_model_structure.N
-    #     possible = self.parent_model_structure.possible
-    #     model = self.parent_model_structure.model
-    #     ver_states = {
-    #         bitvec_to_substates(bit, N)
-    #         for bit in self["verifiers"]
-    #         if model.evaluate(possible(bit))
-    #     }
-    #     fal_states = {
-    #         bitvec_to_substates(bit, N)
-    #         for bit in self["falsifiers"]
-    #         if model.evaluate(possible(bit))
-    #     }
-    #     if ver_states and fal_states:
-    #         print(
-    #             f"  |{self}| = < {make_set_pretty_for_print(ver_states)}, {make_set_pretty_for_print(fal_states)} >",
-    #             file=output,
-    #         )
-    #     elif ver_states and not fal_states:
-    #         print(
-    #             f"  |{self}| = < {make_set_pretty_for_print(ver_states)}, ∅ >",
-    #             file=output,
-    #         )
-    #     elif not ver_states and fal_states:
-    #         print(
-    #             f"  |{self}| = < ∅, {make_set_pretty_for_print(fal_states)} >",
-    #             file=output,
-    #         )
-    #     else:
-    #         print(f"  |{self}| = < ∅, ∅ >", file=output)
-
-    # def print_alt_worlds(self, output=sys.__stdout__):
-    #     """prints everything that has to do with alt worlds
-    #     Used in print_prop()
-    #     Takes in a proposition. Note that this proposition has itself a comparison world.
-    #     This is not inputted into the method, but accessed. So, need to make sure, before the method
-    #     is called, that the proposition has the proper comparison world before calling the function
-    #     """
-    #     N = self.parent_model_structure.N
-    #     comp_world = self["comparison world"]
-    #     # model = self.parent_model_structure.model  # ModelRef object (unused)
-    #     alt_worlds = {bitvec_to_substates(alt, N) for alt in self["alternative worlds"]}
-    #     if alt_worlds:
-    #         print(
-    #             f"  {self}-alternatives to {bitvec_to_substates(comp_world, N)} = {make_set_pretty_for_print(alt_worlds)}",
-    #             file=output,
-    #         )
-    #         for alt_bit in self["alternative worlds"]:
-    #             true_in_alt, false_in_alt = find_true_and_false_in_alt(
-    #                 alt_bit, self.parent_model_structure
-    #             )
-    #             print_alt_relation(true_in_alt, alt_bit, "true", N, output)
-    #             print_alt_relation(false_in_alt, alt_bit, "not true", N, output)
-    #         print(file=output)  # for an extra blank line
-    #     else:
-    #         print(
-    #             f"  There are no {self}-alternatives to {bitvec_to_substates(comp_world, N)}",
-    #             file=output,
-    #         )
-    #         print(file=output)  # for an extra blank line
-
-
-class Counterfactual(Proposition):
-    """subclass of Proposition for counterfactuals"""
-
-    # def __init__(self, prefix_expr, model_structure, world):
-    def truth_value_at(self, eval_world):
-        """finds whether a CF is true at a certain world
-        returns a Boolean representing yes or no"""
-        if eval_world in self["verifiers"]:
-            return True
-        return False
-
-class Modal(Proposition):
-    '''subclass of Proposition for modals'''
-    def __init__(self, prefix_expr, model_structure, world):
-        super().__init__(prefix_expr, model_structure, world)
-        arg = prefix_expr[1]
-        arg_worlds, non_arg_worlds = self.parent_model_structure.find_complex_proposition(arg)
-        self['arg worlds'] = arg_worlds
-        self['non arg worlds'] = non_arg_worlds
-
+        if fal_states:
+            fal_prints = pretty_set_print(fal_states)
+        world_state = bitvec_to_substates(eval_world, N)
+        print(
+            f"{'  ' * indent_num}|{self}| = < {ver_prints}, {fal_prints} >"
+            f"  ({truth_value} in {world_state})",
+            file=output,
+        )
 
     def truth_value_at(self, eval_world):
-        if eval_world in self["verifiers"]:
-            return True
+        '''Given a world, returns the truth value of the Proposition at that world.
+        Used in print_verifiers_and_falsifiers.'''
+        prefix_expr = self['prefix expression']
+        if is_counterfactual(prefix_expr):
+            return True if eval_world in self['worlds cf true at'] else False
+        # if is_modal(prefix_expr):
+        #     return True if self["verifiers"] else False
+         # else case: extensional. Last to be computationally efficient (see def of is_extensional)
+        for verifier in self["verifiers"]:
+            if bit_part(verifier, eval_world):
+                return True
         return False
 
 
-def make_model_for(N):
+def make_model_for(N, premises, conclusions):
     """
-    input: N
+    input: N (int of number of atomic states you want in the model)
     returns a function that will solve the premises and conclusions"""
-
-    def make_relations_and_solve(premises, conclusions):
-        possible = Function("possible", BitVecSort(N), BoolSort())
-        verify = Function("verify", BitVecSort(N), AtomSort, BoolSort())
-        falsify = Function("falsify", BitVecSort(N), AtomSort, BoolSort())
-        assign = Function("assign", BitVecSort(N), AtomSort, BitVecSort(N))
-        w = BitVec("w", N)
-        mod = ModelStructure(
-            premises, conclusions, verify, falsify, possible, assign, N, w
-        )
-        mod.solve()
-        return mod
-
-    return make_relations_and_solve
+    backslash_premises = [add_backslashes_to_infix(prem) for prem in premises]
+    backslash_conclusions = [add_backslashes_to_infix(concl) for concl in conclusions]
+    model_setup = ModelSetup(N, backslash_premises, backslash_conclusions)
+    z3_model_status, z3_model, model_runtime = model_setup.solve()
+    model_structure = ModelStructure(z3_model_status, model_setup, z3_model, model_runtime)
+    return model_setup, model_structure
```

### Comparing `model_checker-0.2.9/scr/model_checker/semantics.py` & `model_checker-0.3.2/src/model_checker/semantics.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,62 +11,42 @@
     Implies,
     Or,
     Not,
     Solver,
     And,
     BitVec,
 )
-from syntax import Prefix
-
-# from sympy import symbols, Or, And, Implies, Not, to_cnf
-
-# def bit_vec_length():
-#     from test_complete import N
-#     return N
-# N = bit_vec_length()
-
-
-# NOTE: we used to have it where we declared a fixed set of variables.
-# a, b, c = BitVecs("a b c", N)
-# r, s, t = BitVecs("r s t", N)
-# u, v, w = BitVecs("u v w", N)
-# x, y, z = BitVecs("x y z", N)
-
-# NOTE: variables are now declared inside each function where they are used.
-# QUESTIONS: is there a clear reason to prefer one way over the other?
-# is it possible/desirable to avoid use of 'Exists' entirely?
-
 
 def make_constraints(verify, falsify, possible, assign, N, w):
     '''function that makes the function to make the constraints (and list of sentence letters
     and prefix sentences) This has to be done in order to define N in an input file—you'll see
     here that N is passed in as a variable to the function, after which these 'make' a semantics
     with that N (and the other inputs to this function also depend on N)
     returns a function find_all_constraints that is used to find the constraints, the sentence letters,
     and prefix sentences.. 
     '''
-    def non_null_verify(bit_s, atom):
-        """bit_s verifies atom and is not the null state
-        returns a Z3 constraint"""
-        return And(Not(bit_s == 0), verify(bit_s, atom))
-
-    def non_null_falsify(bit_s, atom):
-        """bit_s verifies atom and is not the null state
-        returns a Z3 constraint"""
-        return And(Not(bit_s == 0), falsify(bit_s, atom))
-
-    def non_triv_verify(bit_s, atom):
-        """bit_s verifies atom and is not the null state
-        returns a Z3 constraint"""
-        return And(non_null_verify(bit_s, atom), possible(bit_s))
-
-    def non_triv_falsify(bit_s, atom):
-        """bit_s verifies atom and is not the null state
-        returns a Z3 constraint"""
-        return And(non_null_falsify(bit_s, atom), possible(bit_s))
+    # def non_null_verify(bit_s, atom):
+    #     """bit_s verifies atom and is not the null state
+    #     returns a Z3 constraint"""
+    #     return And(Not(bit_s == 0), verify(bit_s, atom))
+    #
+    # def non_null_falsify(bit_s, atom):
+    #     """bit_s verifies atom and is not the null state
+    #     returns a Z3 constraint"""
+    #     return And(Not(bit_s == 0), falsify(bit_s, atom))
+    #
+    # def non_triv_verify(bit_s, atom):
+    #     """bit_s verifies atom and is not the null state
+    #     returns a Z3 constraint"""
+    #     return And(non_null_verify(bit_s, atom), possible(bit_s))
+    #
+    # def non_triv_falsify(bit_s, atom):
+    #     """bit_s verifies atom and is not the null state
+    #     returns a Z3 constraint"""
+    #     return And(non_null_falsify(bit_s, atom), possible(bit_s))
 
     def fusion(bit_s, bit_t):
         """the result of taking the maximum for each index in bit_s and bit_t
         returns a Z3 constraint"""
         return bit_s | bit_t
 
     def is_part_of(bit_s, bit_t):
@@ -78,15 +58,15 @@
         """the fusion of bit_x and bit_y is possible
         returns a Z3 constraint"""
         return possible(fusion(bit_x, bit_y))
 
     def maximal(bit_w):
         """bit_w includes all compatible states as parts.
         returns a Z3 constraint"""
-        x = BitVec("max_dummy", N)
+        x = BitVec("max_x", N)
         return ForAll(
             x,
             Implies(
                 compatible(x, bit_w),
                 is_part_of(x, bit_w),
             ),
         )
@@ -98,236 +78,241 @@
             possible(bit_w),
             maximal(bit_w),
         )
 
     def max_compatible_part(bit_x, bit_w, bit_y):
         """bit_x is the biggest part of bit_w that is compatible with bit_y.
         returns a Z3 constraint"""
-        z = BitVec("max_part_dummy", N)
+        z = BitVec("max_part", N)
         return And(
             is_part_of(bit_x, bit_w),
             compatible(bit_x, bit_y),
             ForAll(
                 z,
                 Implies(
                     And(
-                        is_part_of(z, bit_w), compatible(z, bit_y), is_part_of(bit_x, z)
+                        is_part_of(z, bit_w),
+                        compatible(z, bit_y),
+                        is_part_of(bit_x, z),
                     ),
                     bit_x == z,
                 ),
             ),
         )
 
     def is_alternative(bit_u, bit_y, bit_w):
         """
         bit_u is a world that is the alternative that results from imposing state bit_y on
         world bit_w.
         returns a Z3 constraint
         """
-        z = BitVec("alt_dummy", N)
+        z = BitVec("alt_z", N)
         return And(
             is_world(bit_u),
             is_part_of(bit_y, bit_u),
             Exists(z, And(is_part_of(z, bit_u), max_compatible_part(z, bit_w, bit_y))),
         )
 
-    def extended_verify(state, ext_sent): # used to have default var evaluate=False, seems like
-        # it was unnecessary
+    def extended_verify(state, ext_sent, eval_world):
         """ext_sent is in prefix form. The state is the state that verifies ext_sent. 
         evaluate is an optional bool to evaluate something (now unused).
         returns a Z3 constraint"""
         if len(ext_sent) == 1:
             return verify(state, ext_sent[0])
         op = ext_sent[0]
-        if "boxright" in op:
-            raise ValueError(f"The sentence {ext_sent} is not extensional.")
+        if "boxright" in op or "Box" in op or "Diamond" in op:
+            return true_at(ext_sent, eval_world)
+            # raise ValueError(
+            #     f"\n\nThe antecedent of a counterfactual conditional must be extensional.\n"
+            #     f"The sentence '{infix(ext_sent)}' is not extensional.\n"
+            # )
         if "neg" in op:
-            return extended_falsify(state, ext_sent[1])
-        Y = ext_sent[1]  # should be a list itself
-        Z = ext_sent[2]  # should be a list itself
+            return extended_falsify(state, ext_sent[1], eval_world)
+        Y = ext_sent[1]  # is a list itself
+        Z = ext_sent[2]  # is a list itself
         if "wedge" in op:
-            y = BitVec("ex_ver_dummy_y", N)
-            z = BitVec("ex_ver_dummy_z", N)
+            y = BitVec("ex_ver_y", N)
+            z = BitVec("ex_ver_z", N)
             # if evaluate is True:
             #     return And(
             #         fusion(y, z) == state, extended_verify(y, Y), extended_verify(z, Z)
             #     )
             # had this in here for some reason. Don't remember why.
             return Exists(
                 [y, z],
                 And(
-                    fusion(y, z) == state, extended_verify(y, Y), extended_verify(z, Z)
+                    fusion(y, z) == state,
+                    extended_verify(y, Y, eval_world),
+                    extended_verify(z, Z, eval_world),
                 ),
             )
         if "vee" in op:
             return Or(
-                extended_verify(state, Y),
-                extended_verify(state, Z),
-                extended_verify(state, ["wedge", Y, Z]),
+                extended_verify(state, Y, eval_world),
+                extended_verify(state, Z, eval_world),
+                extended_verify(state, ["wedge", Y, Z], eval_world),
             )
         if "leftrightarrow" in op:
             return Or(
-                extended_verify(state, ["wedge", Y, Z]),
-                extended_falsify(state, ["vee", Y, Z]),
+                extended_verify(state, ["wedge", Y, Z], eval_world),
+                extended_falsify(state, ["vee", Y, Z], eval_world),
             )
         if "rightarrow" in op:
             return Or(
-                extended_falsify(state, Y),
-                extended_verify(state, Z),
-                extended_verify(state, ["wedge", ["neg", Y], Z]),
+                extended_falsify(state, Y, eval_world),
+                extended_verify(state, Z, eval_world),
+                extended_verify(state, ["wedge", ["neg", Y], Z], eval_world),
             )
         raise ValueError(
             f"Something went wrong in extended_verify in evaluating the operator {op} in [{op}, {Y}, {Z}]"
         )
 
-    def extended_falsify(state, ext_sent):
+    def extended_falsify(state, ext_sent, eval_world):
         """ext_sent is in prefix form. The state is the state that falsifies ext_sent. 
         returns a Z3 constraint"""
         if len(ext_sent) == 1:
             return falsify(state, ext_sent[0])
         op = ext_sent[0]
-        if "boxright" in op:
-            raise ValueError(f"The sentence {ext_sent} is not extensional.")
+        if "boxright" in op or "Box" in op or "neg" in op:
+            return false_at(ext_sent, eval_world)
+            # raise ValueError(
+            #     f"\n\nThe antecedent of a counterfactual conditional must be extensional.\n"
+            #     f"The sentence '{infix(ext_sent)}' is not extensional.\n"
+            # )
         if "neg" in op:
-            return extended_verify(state, ext_sent[1])
+            return extended_verify(state, ext_sent[1], eval_world)
         Y = ext_sent[1]
         Z = ext_sent[2]
         if "wedge" in op:
             return Or(
-                extended_falsify(state, Y),
-                extended_falsify(state, Z),
-                extended_falsify(state, ["vee", Y, Z]),
-            )
-        y = BitVec("ex_fal_dummy_y", N)
-        z = BitVec("ex_fal_dummy_z", N)
-        # usage of these two in vee and right arrow is mutually exclusive, so can define uphere
+                extended_falsify(state, Y, eval_world),
+                extended_falsify(state, Z, eval_world),
+                extended_falsify(state, ["vee", Y, Z], eval_world),
+            )
+        y = BitVec("ex_fal_y", N)
+        z = BitVec("ex_fal_z", N)
+        # usage of these two in vee and right arrow is mutually exclusive,
+        # so can define the y and z dummy bitvecs up here
         if "vee" in op:
             return Exists(
                 [y, z],
                 And(
                     state == fusion(y, z),
-                    extended_falsify(y, Y),
-                    extended_falsify(z, Z),
+                    extended_falsify(y, Y, eval_world),
+                    extended_falsify(z, Z, eval_world),
                 ),
             )
         if "leftrightarrow" in op:
             return Or(
-                extended_verify(state, ["wedge", Y, ["neg", Z]]),
-                extended_falsify(state, ["vee", Y, ["neg", Z]]),
+                extended_verify(state, ["wedge", Y, ["neg", Z]], eval_world),
+                extended_falsify(state, ["vee", Y, ["neg", Z]], eval_world),
             )
         if "rightarrow" in op:
             return Exists(
                 [y, z],
                 And(
-                    state == fusion(y, z), extended_verify(y, Y), extended_falsify(z, Z)
+                    state == fusion(y, z),
+                    extended_verify(y, Y, eval_world),
+                    extended_falsify(z, Z, eval_world),
                 ),
             )
         raise ValueError(
             f"Something went wrong in extended_verify in evaluating the operator {op} in [{op}, {Y}, {Z}]"
         )
 
-    # NOTE: the true_at/false-at definitions are bilateral to accommodate the fact
-    # that the exhaustivity constraint is not included in the definition of props
-    # this should avoid the need for specific clauses for (un)negated CFs
-    def true_at(sentence, world):
-        """sentence is a sentence in prefix notation
+    def true_at(sentence, eval_world):
+        """sentence is a sentence in prefix notation. Eval world is the world the sentence is
+        to be evaluated at (changes for counterfactuals). 
+        NOTE: the true_at/false-at definitions are bilateral to accommodate the fact
+        that the exhaustivity constraint is not included in the definition of props
+        this should avoid the need for specific clauses for (un)negated CFs. 
         returns a Z3 constraint"""
-        x = BitVec("t_dummy_x", N)
-        u = BitVec("t_dummy_u", N)
-        y = BitVec("t_dummy_y", N)
+        x = BitVec("t_x", N)
+        u = BitVec("t_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
-            if 'top' in str(sent)[0]:
-                raise ValueError('This is raised in principle when top is a proposition. @B, what should we do?')
-                # if top is a sentence letter, its constraint is already in the model.
-                # It wouldn't hurt to add it again I think in principle, but if there's something
-                # else that should go here when top is passed in by itself then it would go here
-                # return ForAll(x, And(verify(x, sent),Not(falsify(x, sent)))) # this is the top constraint
-            return Exists(x, And(is_part_of(x, world), verify(x, sent)))
+            if 'top' not in str(sent)[0]: # top const alr in model, see find_model_constraints
+                return Exists(x, And(is_part_of(x, eval_world), verify(x, sent)))
         op = sentence[0]
         if "neg" in op:
-            return false_at(sentence[1], world)
+            return false_at(sentence[1], eval_world)
         if len(sentence) == 2 and 'Box' in op:
             return ForAll(u, Implies(is_world(u), true_at(sentence[1], u)))
-            # return ForAll(x, Implies(possible(x), Exists(y, And(extended_verify(y,sentence[1]), compatible(x,y)))))
         if len(sentence) == 2 and 'Diamond' in op:
-            # print(sentence)
             return Exists(u, And(is_world(u), true_at(sentence[1], u)))
-            # return Exists(x, And(possible(x), extended_verify(x,sentence[1])))
         Y = sentence[1]
         Z = sentence[2]
         if "wedge" in op:
-            return And(true_at(Y, world), true_at(Z, world))
+            return And(true_at(Y, eval_world), true_at(Z, eval_world))
         if "vee" in op:
-            return Or(true_at(Y, world), true_at(Z, world))
+            return Or(true_at(Y, eval_world), true_at(Z, eval_world))
         if "leftrightarrow" in op:
             return Or(
-                And(true_at(Y, world), true_at(Z, world)),
-                And(false_at(Y, world), false_at(Z, world)),
+                And(true_at(Y, eval_world), true_at(Z, eval_world)),
+                And(false_at(Y, eval_world), false_at(Z, eval_world)),
             )
         if "rightarrow" in op:
-            return Or(false_at(Y, world), true_at(Z, world))
+            return Or(false_at(Y, eval_world), true_at(Z, eval_world))
         if "boxright" in op:
             return ForAll(
                 [x, u],
                 Implies(
-                    And(extended_verify(x, Y), is_alternative(u, x, world)),
+                    And(extended_verify(x, Y, eval_world), is_alternative(u, x, eval_world)),
                     true_at(Z, u),
                 ),
             )
-        raise ValueError(f'No if statements triggered— true_at for {sentence} at world {world}')
+        raise ValueError(f'No if statements triggered— true_at for {sentence} at world {eval_world}')
 
-    def false_at(sentence, world):
-        """X is a sentence in prefix notation
+    def false_at(sentence, eval_world):
+        """X is a sentence in prefix notation, eval world is the world the sentence is to be
+        evaulated at. See true_at (above) for an important note on exhaustivity.
         returns a Z3 constraint"""
-        x = BitVec("f_dummy_x", N)
-        u = BitVec("f_dummy_u", N)
+        x = BitVec("f_x", N)
+        u = BitVec("f_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
-            # if str(sent) == "\\top":
-            #     return ForAll(x, And(verify(x, sent),Not(falsify(x, sent))))
-            return Exists(x, And(is_part_of(x, world), falsify(x, sent)))
+            return Exists(x, And(is_part_of(x, eval_world), falsify(x, sent)))
         op = sentence[0]
         if "neg" in op:
-            return true_at(sentence[1], world)
+            return true_at(sentence[1], eval_world)
         if len(sentence) == 2 and 'Box' in op:
             # print(sentence)
             return Exists(u, And(is_world(u), false_at(sentence[1], u)))
         if len(sentence) == 2 and 'Diamond' in op:
             # print(sentence)
             return ForAll(u, Implies(is_world(u), false_at(sentence[1], u)))
         Y = sentence[1]
         Z = sentence[2]
         if "wedge" in op:
-            return Or(false_at(Y, world), false_at(Z, world))
+            return Or(false_at(Y, eval_world), false_at(Z, eval_world))
         if "vee" in op:
-            return And(false_at(Y, world), false_at(Z, world))
+            return And(false_at(Y, eval_world), false_at(Z, eval_world))
         if "leftrightarrow" in op:
             return Or(
-                And(true_at(Y, world), false_at(Z, world)),
-                And(false_at(Y, world), true_at(Z, world)),
+                And(true_at(Y, eval_world), false_at(Z, eval_world)),
+                And(false_at(Y, eval_world), true_at(Z, eval_world)),
             )
         if "rightarrow" in op:
-            return And(true_at(Y, world), false_at(Z, world))
+            return And(true_at(Y, eval_world), false_at(Z, eval_world))
         if "boxright" in op:
             return Exists(
                 [x, u],
-                And(extended_verify(x, Y), is_alternative(u, x, world), false_at(Z, u)),
+                And(extended_verify(x, Y, eval_world), is_alternative(u, x, eval_world), false_at(Z, u)),
             )
-        raise ValueError(f'No if statements triggered— false_at for {sentence} at world {world}')
+        raise ValueError(f'No if statements triggered in false_at for {sentence} at world {eval_world}')
 
     def prop_const(atom):
         """
         atom is a proposition since its verifiers and falsifiers are closed under
         fusion respectively, and the verifiers and falsifiers for atom are
         incompatible (exclusivity). NOTE: exhaustivity crashes Z3 so left off.
         returns a Z3 constraint for the proposition atom
         """
-        x = BitVec("prop_dummy_x", N)
-        y = BitVec("prop_dummy_y", N)
+        x = BitVec("prop_x", N)
+        y = BitVec("prop_y", N)
         sent_to_prop = [
             Not(verify(0, atom)),
             Not(falsify(0, atom)),
             # Exists(x, non_null_verify(x, atom)),
             # Exists(y, non_null_falsify(y, atom)),
             # Exists(x, non_triv_verify(x, atom)),
             # Exists(y, non_triv_falsify(y, atom)),
@@ -357,98 +342,63 @@
                     ),
                 ),
             ),
         ]
         return sent_to_prop
 
     def find_frame_constraints():
-        """find the constraints that depend only on the sentence letters
+        """returns constraints that govern how states act:
+        1. for any two states x and y, if y is possible and x is a part of y, then x is possible
+        2. for any two states x and y, there exists a state z that is the fusion of x and y
+        3. there is a state which is a world state (we call it w)
         returns a list of Z3 constraints"""
-        x = BitVec("frame_dummy_x", N)
-        y = BitVec("frame_dummy_y", N)
-        z = BitVec("frame_dummy_z", N)
+        x = BitVec("frame_x", N)
+        y = BitVec("frame_y", N)
+        z = BitVec("frame_z", N)
         frame_constraints = [
             ForAll([x, y], Implies(And(possible(y), is_part_of(x, y)), possible(x))),
             ForAll([x, y], Exists(z, fusion(x, y) == z)),
-            is_world(w),
+            is_world(w), # w is passed in from the big outer function
         ]
-        # test_atom = [Const("test_atom", AtomSort)]
-        # test_constraints = [
-        #     Exists(x,
-        #         And(
-        #            is_world(x),
-        #            Not(true_at(test_atom, x)),
-        #            Not(false_at(test_atom, x)),
-        #         )
-        #     ),
-        # ]
-        return frame_constraints # + test_constraints
-
-    # def add_general_constraints(solv, input_sentence_letters):
-    #     """adds the constraints that go in every solver"""
-    #     possible_part = ForAll(
-    #         [x, y], Implies(And(possible(y), is_part_of(x, y)), possible(x))
-    #     )
-    #     solv.add(possible_part)
-    #     print(f"\nPossibility constraint:\n {possible_part}\n")
-    #     # NOTE: seems to slightly slow things down with no obvious gains but I'm
-    #     # still unsure if this is needed or not. would be good to confirm.
-    #     fusion_closure = ForAll([x, y], Exists(z, fusion(x, y) == z))
-    #     solv.add(fusion_closure)
-    #     print(f"Fusion constraint:\n {fusion_closure}\n")
-    #     world_const = is_world(w)
-    #     solv.add(world_const)
-    #     print(f"World constraint: {world_const}")
-    #     for sent_letter in input_sentence_letters:
-    #         print(f"\nSentence {sent_letter} yields the general constraints:\n")
-    #         for const in prop_const(sent_letter):
-    #             solv.add(const)
-    #             print(f"{const}\n")
+        return frame_constraints
 
     def find_model_constraints(prefix_sents,input_sentence_letters):
         """find constraints corresponding to the input sentences
-        returns a list of Z3 constraints"""
+        takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
+        returns a list of Z3 constraints
+        used in find_all_constraints"""
         prop_constraints = []
         input_constraints = []
         for sent_letter in input_sentence_letters:
             if 'top' in str(sent_letter):
                 x = BitVec("top_x", N)
                 top_constraint = ForAll(x,
                     And(
                         verify(x,sent_letter),
                         Not(falsify(x,sent_letter))
                     )
                 )
                 prop_constraints.append(top_constraint)
-                continue
+                continue # ie, prop_const should never be called on '\\top'
             for constraint in prop_const(sent_letter):
                 prop_constraints.append(constraint)
         for sentence in prefix_sents:
             sentence_constraint = true_at(sentence, w)
             input_constraints.append(sentence_constraint)
         model_constraints = prop_constraints + input_constraints
         return model_constraints
 
-    # def add_input_constraints(solv, prefix_sentences):
-    #     """add input-specific constraints to the solver"""
-    #     for sentence in prefix_sentences:
-    #         print(sentence)
-    #         sentence_constraint = true_at(sentence, w)
-    #         print(
-    #             f"Sentence {sentence} yields the model constraint:\n {sentence_constraint}\n"
-    #         )
-    #         solv.add(sentence_constraint)
-
     def sentence_letters_in_compound(prefix_input_sentence):
         """finds all the sentence letters in ONE input sentence. returns a list. WILL HAVE REPEATS
-        used in all_sentence_letters
         returns a list of AtomSorts. CRUCIAL: IN THAT SENSE DOES NOT FOLLOW SYNTAX OF PREFIX SENTS.
-        But that's ok, just relevant to know"""
+        But that's ok, just relevant to know
+        used in all_sentence_letters
+        """
         if len(prefix_input_sentence) == 1:  # base case: atomic sentence
-            return prefix_input_sentence
+            return [prefix_input_sentence[0]] # redundant but conceptually clear
         return_list = []
         for part in prefix_input_sentence[1:]:
             return_list.extend(sentence_letters_in_compound(part))
         return return_list
 
     def all_sentence_letters(prefix_input_sentences):
         """finds all the sentence letters in a list of input sentences.
@@ -458,26 +408,27 @@
         for prefix_input in prefix_input_sentences:
             sentence_letters_in_input = sentence_letters_in_compound(prefix_input)
             for sentence_letter in sentence_letters_in_input:
                 sentence_letters.add(sentence_letter)
         return list(sentence_letters)
         # sort just to make every output the same, given sets aren't hashable
 
-    def find_all_constraints(infix_input_sentences):
+    def find_all_constraints(prefix_input_sentences):
         """find Z3 constraints for input sentences
         input_sents are a list of infix sentences
         returns a tuple with all Z3 constraints, for the model, the sentence letters
         (a list of AtomSorts), and the prefix_sentences (a list of lists, since prefix
-        sentences are lists)"""
-        prefix_sentences = [Prefix(input_sent) for input_sent in infix_input_sentences]
-        sentence_letters = all_sentence_letters(prefix_sentences)  # this works
-        input_const = find_model_constraints(prefix_sentences, sentence_letters)
+        sentences are lists)
+        function that is returned by the big outer function"""
+        # prefix_sentences = [Prefix(input_sent) for input_sent in infix_input_sentences]
+        sentence_letters = all_sentence_letters(prefix_input_sentences)  # this works
+        input_const = find_model_constraints(prefix_input_sentences, sentence_letters)
         gen_const = find_frame_constraints()
         const = gen_const + input_const
-        return (const, sentence_letters, prefix_sentences)
+        return (const, sentence_letters)
 
     return find_all_constraints
 
 
 def solve_constraints(all_constraints): # all_constraints is a list
     """find model for the input constraints if there is any
     returns a tuple with a boolean representing if the constraints were solved or not
```

### Comparing `model_checker-0.2.9/scr/model_checker/syntax.py` & `model_checker-0.3.2/src/model_checker/syntax.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 """
 file contains all syntactic definitions
 
 NOTES:
-All sentence letters are capital letters.
-All commands must be strictly in lowercase; they can have double backslash, a forward slash, or nothing (nothing so long as the first letter is lowercase).
+All commands must be strictly in lowercase. They must have nothing before or double backslash.
+Sentence letters can be anything.
 The unary operators are defined in a separate set for clarity in the code.
 """
 from z3 import Const, DeclareSort
 
 
 AtomSort = DeclareSort("AtomSort")
-# sentence_stuff = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','Z','W','Y','Z'}
-# operator_stuff = {'\\','/','a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z'}
-unary_operators = {"\\neg", "/neg", "neg", "box", "Box", "\\Box", "\\box", "Diamond", "diamond", "\\diamond", "\\Diamond"}
+capital_alphabet = {"A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M",
+                    "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z",}
+unary_operators = {"\\neg", "neg", "Box", "\\Box", "Diamond", "\\Diamond"}
+binary_operators = {"\\wedge", 'wedge', '\\vee', 'vee', '\\rightarrow', 'rightarrow',
+                    '\\leftrightarrow', 'leftrightarrow', '\\boxright', 'boxright'}
+all_operators = unary_operators.union(binary_operators)
+
+
+def add_double_backslashes(tokens):
+    """adds a double backslash to tokens in the output of tokenize that meet these 3 conditions:
+    1. are not capital letters,
+    2. do not already have a double backslash in them, AND
+    3. are not parentheses
+    returns the input tokens list with tokens having those qualities modified as described
+    """
+    new_tokens = []
+    for token in tokens:
+        if (token in all_operators and "\\" not in token):
+            token = "\\" + token
+        new_tokens.append(token)
+    return new_tokens
 
 
 def tokenize(str_exp):
     """
     >>> tokenize("(A /wedge (B /vee C))")
     ['(', 'A', '/wedge', '(', 'B', '/vee', 'C', ')', ')']
 
     >>> tokenize("(/neg A /wedge (B /vee C))")
     ['(', '/neg', 'A', '/wedge', '(', 'B', '/vee', 'C', ')', ')']
 
-    >>> tokenize('((A /operator ((C /operator D) /operator F)) /operator E)')
-    ['(', '(', 'A', '/operator', '(', '(', 'C', '/operator', 'D', ')', '/operator', 'F', ')', ')', '/operator', 'E', ')']
+    >>> tokenize('((A /op ((C /op D) /op F)) /op E)')
+    ['(', '(', 'A', '/op', '(', '(', 'C', '/op', 'D', ')', '/op', 'F', ')', ')', '/op', 'E', ')']
 
     >>> tokenize('/neg A')
     ['/neg', 'A']
     """
     split_str = str_exp.split()  # small issue here with doctest cases and backslashes
 
     def tokenize_improved_input(split_str):
@@ -44,16 +62,31 @@
                 tokenized_l.append(")")
                 return tokenized_l
             return split_str  # else case: covers sentence letter case and latex operator case
         tokenized_l = tokenize_improved_input([split_str[0]])
         tokenized_l.extend(tokenize_improved_input(split_str[1:]))
         return tokenized_l
 
-    return tokenize_improved_input(split_str)
+    raw_tokens = tokenize_improved_input(split_str)
+    return add_double_backslashes(raw_tokens)
 
+def rejoin_tokens(tokens):
+    infix_expr = ''
+    for token in tokens:
+        if token in binary_operators:
+            token = f' {token} '
+        if token in unary_operators:
+            token = f'{token} '
+        infix_expr += token
+    return infix_expr
+
+def add_backslashes_to_infix(infix_expr):
+    tokens_with_backslashes = tokenize(infix_expr)
+    rejoined_with_backslashes = rejoin_tokens(tokens_with_backslashes)
+    return rejoined_with_backslashes
 
 def binary_comp(tokenized_expression):
     """
     finds complexity, defined by number of operators, in a tokenized_expression.
     In reality, it counts left parentheses. But it can easily be shown by induction
     that this number and that of operators is equal.
 
@@ -94,22 +127,31 @@
         raise ValueError(tokenized_expression, "Error: parentheses unmatched")
     # [1:] to exclude the left parens (thus complexity) of the main operator
     for i, token in enumerate(tokenized_expression[1:]):
         if token == "(":
             left_parentheses += 1
         elif token == ")":
             right_parentheses += 1
-        # ignore this case since we care about binary complexity
-        elif token in unary_operators:
+        elif (
+            token in unary_operators
+        ):  # ignore this case since this func is for binary complexity
             continue
         if left_parentheses == right_parentheses:
             # +1 bc list is [1:] and we want original index, and +1 bc it's next
             # elem where the main op is
             return i + 2
-    raise ValueError(tokenized_expression, f"Error: looks like nothing was passed into main_op_index ({tokenized_expression})")
+    raise ValueError(
+        tokenized_expression,
+        f"Looks like nothing was passed into main_op_index ({tokenized_expression})",
+    )
+
+# # M: most likely not necessary, but leaving here in case later it is
+# def find_atom_strings(tokens):
+#     """make list of all basic tokens to apply AtomSort to"""
+#     pass
 
 
 def parse(tokens):
     """
     >>> parse(tokenize("(A /wedge (B /lor C))"))
     ['/wedge', ['A'], ['/lor', ['B'], ['C']]]
 
@@ -119,62 +161,41 @@
     >>> parse(tokenize("A")) # note: atomic sentence should return a single element list
     ['A']
 
     >>> parse(tokenize('((A /op (B /op C)) /op (D /op E))'))
     ['/op', ['/op', ['A'], ['/op', ['B'], ['C']]], ['/op', ['D'], ['E']]]
     """
     bin_comp_tokens = binary_comp(tokens)
-    # if tokens[0] == "\\top":
-    #     return ["\\top"]
-    #     return [Const(token, AtomSort)]
-    if tokens[0] in unary_operators:
+    if tokens[0] in unary_operators:  # must go before bin_comp_tokens == 0 case
         return [tokens[0], parse(tokens[1:])]
     if bin_comp_tokens == 0:
         token = tokens[0]
-        # Const is a function to make a constant
-        return [Const(token, AtomSort)]
-    main_operator_index = main_op_index(tokens)
-    # determines how far the operation is
+        return [Const(token, AtomSort)]  # Const is a function to make a constant
+    main_operator_index = main_op_index(tokens)  # determines how far the operation is
     op_str = tokens[main_operator_index]
     # start 1 (exclude first parenthesis), stop at same pos of above (exclusive)
     left_expression = tokens[1:main_operator_index]
-    # from pos of op plus 1 to the penultimate, thus excluding the last
-    # parentheses, which belongs to the main expression
     if main_operator_index is None:
         raise SyntaxError("Error: 'main_operator_index' is not set.")
+    # from pos of op plus 1 to the penultimate, thus excluding the last
+    # parentheses, which belongs to the main expression
     right_expression = tokens[main_operator_index + 1 : -1]
     return [op_str, parse(left_expression), parse(right_expression)]
 
 
-def Prefix(A):
-    """takes a sentence in Infix notation and translates it to Prefix notation"""
-    return parse(tokenize(A))
-
-
-def Infix(A):
-    """takes a sentence in Prefix notation and translates it to infix notation"""
-    if len(A) == 1:
-        return str(A[0])
-    if len(A) == 2:
-        if 'neg' in A[0]:
-            return f"\\neg {Infix(A[1])}"
-        if 'iamond' in A[0]:
-            return f"\\Diamond {Infix(A[1])}"
-        return f"\\Box {Infix(A[1])}"
-    op = A[0]
-    left_expr = A[1]
-    right_expr = A[2]
-    return f"({Infix(left_expr)} {op} {Infix(right_expr)})"
-
-
-# doctest.testmod()
-# print(tokenize("(A \\wedge (B \\vee C))")) # the doctests fail, but this works. Need to do double backslash for abfnrtv.
-# print(Prefix("(A \\wedge (B \\vee \\neg C))")) # ['\\wedge', ['A'], ['\\vee', ['B'], ['\\neg', ['C']]]]
-# print(Prefix("A"))
-# print(Prefix('((A \\op (B \\op C)) \\op (D \\op E))')) # ['\\op', ['\\op', ['A'], ['\\op', ['B'], ['C']]], ['\\op', ['D'], ['E']]]
-
-# sentences = [Prefix("(A \\wedge (B \\vee \\neg C))"), Prefix("A"), Prefix('((A \\op (B \\op Z)) \\op (D \\op E))')]
-# print(all_sentence_letters(sentences)) # correctly prints ['A', 'B', 'C', 'D', 'E', 'Z']
-# print(Prefix("\\neg (A \\boxright B)"))
-# print(all_sentence_letters([Prefix("\\neg (A \\boxright B)")]))
+def prefix(infix_sentence):
+    """takes a sentence in infix notation and translates it to prefix notation"""
+    return parse(tokenize(infix_sentence))
+
+
+def infix(prefix_sent):
+    """takes a sentence in prefix notation and translates it to infix notation"""
+    if len(prefix_sent) == 1:
+        return str(prefix_sent[0])
+    op = prefix_sent[0]
+    if len(prefix_sent) == 2:
+        return f"{op} {infix(prefix_sent[1])}"
+    left_expr = prefix_sent[1]
+    right_expr = prefix_sent[2]
+    return f"({infix(left_expr)} {op} {infix(right_expr)})"
 
 # moved unused prefix_combine to the boneyard
```

