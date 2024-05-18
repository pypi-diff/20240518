# Comparing `tmp/pysymmpol-0.1.1.tar.gz` & `tmp/pysymmpol-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysymmpol-0.1.1.tar", max compression
+gzip compressed data, was "pysymmpol-0.1.2.tar", max compression
```

## Comparing `pysymmpol-0.1.1.tar` & `pysymmpol-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    35149 2024-03-19 18:59:42.710170 pysymmpol-0.1.1/LICENSE
--rw-r--r--   0        0        0     6431 2024-03-21 11:27:31.765151 pysymmpol-0.1.1/README.md
--rw-r--r--   0        0        0      417 2024-03-21 12:45:23.901708 pysymmpol-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      434 2024-03-19 18:59:42.734171 pysymmpol-0.1.1/pysymmpol/__init__.py
--rw-r--r--   0        0        0       33 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/partitions/__init__.py
--rw-r--r--   0        0        0     4442 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/partitions/conjugacy.py
--rw-r--r--   0        0        0     2797 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/partitions/states.py
--rw-r--r--   0        0        0     8053 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/partitions/young.py
--rw-r--r--   0        0        0        1 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/polynomials/__init__.py
--rw-r--r--   0        0        0     1395 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/polynomials/elementary.py
--rw-r--r--   0        0        0     4100 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/polynomials/hall.py
--rw-r--r--   0        0        0     3742 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/polynomials/homogeneous.py
--rw-r--r--   0        0        0      952 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/polynomials/monomial.py
--rw-r--r--   0        0        0     3494 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/polynomials/schur.py
--rw-r--r--   0        0        0      244 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/utils/__init__.py
--rw-r--r--   0        0        0     1179 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/utils/inner.py
--rw-r--r--   0        0        0     2300 2024-03-19 18:59:42.735170 pysymmpol-0.1.1/pysymmpol/utils/tools.py
--rw-r--r--   0        0        0     6913 1970-01-01 00:00:00.000000 pysymmpol-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-19 18:59:42.710170 pysymmpol-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7334 2024-05-18 16:33:32.873489 pysymmpol-0.1.2/README.md
+-rw-r--r--   0        0        0      434 2024-05-18 16:56:24.993546 pysymmpol-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      434 2024-03-19 18:59:42.734171 pysymmpol-0.1.2/pysymmpol/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/partitions/__init__.py
+-rw-r--r--   0        0        0     4620 2024-05-18 16:33:32.899489 pysymmpol-0.1.2/pysymmpol/partitions/conjugacy.py
+-rw-r--r--   0        0        0     2759 2024-05-18 16:33:32.899489 pysymmpol-0.1.2/pysymmpol/partitions/states.py
+-rw-r--r--   0        0        0     8169 2024-05-18 16:33:32.899489 pysymmpol-0.1.2/pysymmpol/partitions/young.py
+-rw-r--r--   0        0        0        1 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/polynomials/__init__.py
+-rw-r--r--   0        0        0     1395 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/polynomials/elementary.py
+-rw-r--r--   0        0        0     4100 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/polynomials/hall.py
+-rw-r--r--   0        0        0     3742 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/polynomials/homogeneous.py
+-rw-r--r--   0        0        0      952 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/polynomials/monomial.py
+-rw-r--r--   0        0        0     3494 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/polynomials/schur.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:33:32.899489 pysymmpol-0.1.2/pysymmpol/py.typed
+-rw-r--r--   0        0        0      244 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/utils/__init__.py
+-rw-r--r--   0        0        0     1802 2024-05-18 16:33:32.900490 pysymmpol-0.1.2/pysymmpol/utils/inner.py
+-rw-r--r--   0        0        0     2300 2024-03-19 18:59:42.735170 pysymmpol-0.1.2/pysymmpol/utils/tools.py
+-rw-r--r--   0        0        0     7816 1970-01-01 00:00:00.000000 pysymmpol-0.1.2/PKG-INFO
```

### Comparing `pysymmpol-0.1.1/LICENSE` & `pysymmpol-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/README.md` & `pysymmpol-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     3. Monomial symmetric polynomials 
     4. Schur polynomials
     5. Hall-Littlewood polynomials
 
 Additionally, the package contains a module with basic functionalities
 for manipulating integer partitions and Young diagrams.
 
+Read our Statement of need [here](STATEMENT-OF-NEED.md).
+
 Tutorials can be found in the [documentation page](https://thraraujo.github.io/pysymmpol/index.html).
 
 ## Dependencies
 
 This package has been tested with the following versions:
-- Python 3.12
-- SymPy 1.12
-- NumPy 1.26.4
+- Python >= 3.11
+- SymPy >= 1.11
+- NumPy >= 1.26.2
 
 ## Installation
 
 The package can be installed with pip:
 ```bash
 $ pip install pysymmpol
 ```
@@ -91,15 +93,15 @@
 ```python
 n = 3
 t = create_miwa(n)
 
 homogeneous = HomogeneousPolynomial(n)
 elementary = ElementaryPolynomial(n)
 print(f"homogeneous: {homogeneous.explicit(t)}")
-print(f"elementary: {elementary.explicit(t)})
+print(f"elementary: {elementary.explicit(t)}")
 ```
 gives the output 
 ```
 homogeneous: t1**3/6 + t1*t2 + t3
 elementary: t1**3/6 - t1*t2 + t3
 ```
 
@@ -179,14 +181,25 @@
 print(f"hall-littlewood: {hall_littlewood.explicit(x, Q)}")
 ```
 gives
 ```
 hall-littlewood: x1*x2*x3*(-Q**2*x1*x2*x3 - Q*x1*x2*x3 + x1**2*x2 + x1**2*x3 + x1*x2**2 + 2*x1*x2*x3 + x1*x3**2 + x2**2*x3 + x2*x3**2)
 ```
 
+# References
+
+Here are some recommended resources covering symmetric polynomials,
+combinatorics, and their significance in theoretical physics:
+
+- [Symmetric Functions and Hall Polynomials - Ian Macdonald](https://books.google.com.br/books/about/Symmetric_Functions_and_Hall_Polynomials.html?id=srv90XiUbZoC&redir_esc=y)
+- [An Introduction to Symmetric Functions and Their Combinatorics - Eric S. Egge](https://bookstore.ams.org/stml-91)
+- [Counting with Symmetric Functions - Mendes and Remmel](https://link.springer.com/book/10.1007/978-3-319-23618-6)
+- [Solitons: Differential Equations, Symmetries and Infinite Dimensional Algebras - Miwa, Jimbo and Date](https://books.google.com.br/books/about/Solitons.html?id=kQDw1ZcqLjUC&redir_esc=y)
+- [The uses of random partitions - Andrei Okounkov](https://arxiv.org/abs/math-ph/0309015)
+
 # Citation & Contributing
 
 If you found this package useful in your research, please consider citing the companion 
 paper available here: [arxiv.org/abs/2403.13580](https://arxiv.org/abs/2403.13580). 
 ```
 @article{Araujo:2024piv,
     author = "Araujo, Thiago",
```

### Comparing `pysymmpol-0.1.1/pysymmpol/partitions/conjugacy.py` & `pysymmpol-0.1.2/pysymmpol/partitions/conjugacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from itertools import pairwise
+from numbers import Number
+
 import numpy as np
 from .young import YoungDiagram
 
 
 @dataclass(frozen=True)
 class ConjugacyClass: 
     '''
-    Represents the conjugacy class of the partitions. For example,
+    Represents the conjugacy class of partitions. For example,
     the partition L = (5, 3, 2, 2, 2, 1, 1) can represented by
     L = (1: 2, 2: 3, 3: 1, 4: 0, 5: 1) that means 2 rows of
     length 1, 3 rows of length 2, 2 rows of length 3, 0 rows of
     length 4 and 1 row of length 5.
 
     To avoid cluttering, we could simply write the vector
     k = (2, 3, 1, 0, 1) to describe the same partition.
     We do it in an internal method below, but we will return
     dictionaries to avoid confusion with the partitions. 
 
     The dictionary must be in the form {1: k1, 2: k2, ..., n: kn}
 
-    The vectors k=(k1,k2, ..., kn) is one conjugacy class of the
-    symmetric group S_n, and for this reason, we call it
-    conjugacy class vectors.
+    The vectors k = (k1,k2, ..., kn) represents one conjugacy class of
+    the symmetric group S_n, and for this reason, we call it conjugacy
+    class vectors.
 
     In terms of the Heisenberg algebra, the components of these vectors
     denote the power of the Heisenberg operator J_{-n} when acting on the
     vacuum state |0>
     '''
     _conjugacy_vector: dict
 
 
     def __post_init__(self) -> None:
         '''
         Validates the form of the dictionary: {1: k1, 2: k2, ..., n: kn}
         '''
+
         keys = tuple(self._conjugacy_vector.keys())
-        A = all([keys[i] - keys[i-1] == 1 for i in range(1, len(keys))])
-        if keys[0] != 1 or not A:
+
+        val_A = all(y - x == 1 for x,y in pairwise(keys))
+        val_B = all(isinstance(m, Number) for m in self._conjugacy_vector.values())
+
+        if keys[0] != 1 or not val_A:
            raise TypeError("Argument must be a dictionary in the form {1: k1, 2: k2, ..., n: kn}")
+        elif not val_B:
+           raise TypeError("Values in the dictionary must be numeric.")
 
 
     @property
     def conjugacy(self) -> tuple:
         '''
         Getter for the conjugacy class vector
         '''
@@ -125,15 +134,14 @@
 
         Then when we put it in decreasing order we find [4,4,4,4,2,2,1]
         '''
 
         partition = np.array([])
 
         for i in range(len(self.conjugacy)):
-            #row = list(np.repeat(i+1, self.conjugacy[i]))
             row = np.repeat(i+1, self.conjugacy[i])
             partition = np.concatenate((partition, row), axis=0)
 
         partition = -np.sort(-partition, axis=0) # Sorts the numpy array in decreasing order.
         partition = partition.astype(int) # Converts entries into integers
 
         return tuple(partition)
```

### Comparing `pysymmpol-0.1.1/pysymmpol/partitions/states.py` & `pysymmpol-0.1.2/pysymmpol/partitions/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,32 +28,32 @@
 
     def _conjugacy_states(self) -> tuple:
         '''
         For a level n, this method gives all vector k
         (the conjugacy class states) that belong to this subspace.
         Remember that these states are built with the operators J_{-m} 
         of the Heisenberg algebra. In other words, these are
-        bosonic states. This nonpublic method can make our life easier.
+        bosonic states. 
         '''
         lev = self.level
 
         if lev == 0:
             return tuple()
         else:
-            vectors_k = [] # Here I create a list to save the vectors
+            vectors_k = []       # Here I create a list to save the vectors
             vectors_k_tuple = [] # Here I create a list to save the tuples after all manipulations
 
             for a in _accel_asc(lev):
-                vec = [0]*lev
+                vec = np.array([0]*lev)
                 for i in range(len(a)):
                     vec[a[i]-1] += 1
                 vectors_k.append(vec)
 
             for a in vectors_k:
-                vectors_k_tuple.append(tuple(a))
+                vectors_k_tuple.append(a)
 
             return tuple(vectors_k_tuple)
 
 
     def conjugacy_states(self) -> tuple:
         '''
         Returns the previous method in
```

### Comparing `pysymmpol-0.1.1/pysymmpol/partitions/young.py` & `pysymmpol-0.1.2/pysymmpol/partitions/young.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from itertools import pairwise
+from numbers import Number
+
 import numpy as np
 import sympy as sp
 
 '''
-In this module we define 2 concepts that
-are completely connected.
-
-    1. First we define the class of Young (or Ferrers) Diagrams
-    using the usual partition notation.
-
-    2. Then we define the class of Conjugacy Classes.
+In this module we define the class of Young (or Ferrers) Diagrams
+using the usual partition notation.
 '''
 
 @dataclass(frozen=True)
 class YoungDiagram:
     '''
     Represents Young diagrams in the standard
-    partition notation: It is a monotonic decreasing sequence
+    partition notation. It is a monotonic decreasing sequence
     L = (L1, L2, L3, ...,Ln) with L1 >= L2 >=L3 >= ... >= Ln.
 
-    Example: (3,2,2,1)
+    Example: (3,2,2,1).
     '''
     _partition: tuple
 
 
     def __post_init__(self) -> None:
 
         '''
         Validade Young diagram:
-        1) The argument must be monotonic decreasing.
-        2) The argument is a tuple.
+        1) The argument is a tuple or a numpy array.
+        2) The argument must be monotonic decreasing.
         '''
 
-        # Validate _partition as a tuple
-        if not isinstance(self.partition, tuple):
-            raise TypeError(f"Argument must be a tuple, and you passed a {type(self._partition)}")
+        # Validade its type.
+        val_A = isinstance(self._partition, (tuple, np.ndarray))
+        val_B = all(isinstance(m, Number) for m in self._partition )
+        if val_A and val_B:
+            par = self._partition
+        else:
+            raise TypeError(f"Argument must be a tuple or a numpy array with numeric entries.")
 
-        # Validade if the partition is a monotonic decreasing sequence. 
-        par = self._partition
-        A = all([x >= y for x,y in zip(par, par[1:])])
-        #A = all([self._partition[i+1] <= self._partition[i] for i in range(len(self._partition) -1)])
+        # Validade if it is a monotonic decreasing sequence. 
+        val_C = all(x >= y for x,y in pairwise(par))
 
-        if not A:
+        if not val_C:
             raise ValueError("Argument must be a monotonic decreasing sequence.")
         
 
     @property
     def partition(self) -> tuple:
         '''
         Gives the partition notation for the Young diagram.
@@ -75,98 +75,156 @@
     def boxes(self) -> int: 
         '''
         This gives the number of boxes in the diagram.
         '''
         return sum(self.partition)
 
 
+    def count_diagonal(self) -> int: 
+        '''
+        Gives the number of boxes in the diagonal.
+        '''
+
+        return len(self.frobenius_coordinates())
+
+
     def draw_diagram(self, n: int=0) -> None:
         '''
         Pictorial representation of the Young/Ferrers diagram in
         French notation. 
         '''
         emo = ['■', '•', '🎲', '🎯', '#']
         for i in range(self.rows):
             if self.partition[-i-1] > 0:
                 print(f"{emo[n]} " * self.partition[-i-1])
 
 
-    def count_diagonal(self) -> int: 
+    def conjugacy_partition(self) -> dict:
         '''
-        Gives the number of boxes in the diagonal.
+        Converts the partition notation to 
+        the conjugacy class notation
+        Example:
+        [4,4,4,2,2,1] to {1: 1, 2: 2, 3: 0, 4: 3}.
 
-        In order to do this calculation,
-        the method represents the Young diagram as a 
-        partition[0] x len(partition) matrix filled
-        with 1 and 0. After that, it sums over the diagonal.
-        '''
+        The algorithm works as follows:
 
-        matrix = np.zeros((self.rows, self.columns))
+        It creates a list of zeros with length equal
+        to the largest row. In our case, 4
+        conjugacy = [0, 0, 0, 0].
 
-        diagonal = 0
+        It iterates over the partition, adding 1s to the
+        corresponding slot in the conjugacy vector, for example
+        partition (4,4,4,2,2,1) gives
+        - loop 01: i = 4
+            conjugacy[3] = 1
+            conjugacy = [0,0,0,1]
+        - loop 02: i = 4
+            conjugacy[3] = 2
+            conjugacy = [0,0,0,2]
+        - loop 03: i = 4
+            conjugacy[3] = 3
+            conjugacy = [0,0,0,3]
+        - loop 04: i = 2
+            conjugacy[1] = 1
+            conjugacy = [0,1,0,3]
+        - loop 05: i = 2
+            conjugacy[1] = 2
+            conjugacy = [0,2,0,3]
+        - loop 06: i = 1
+            conjugacy[0] = 1
+            conjugacy = [1,2,0,3]
 
-        for row in range(self.rows):
-            for column in range(self.partition[row]):
-                matrix[row][column] = 1
-        return int(np.trace(matrix))
+        At the end we convert to a dictionary, and
+        conjugacy = {1: 1, 2: 2, 3: 0, 4: 3}
+        '''
 
+        length = self.partition[0]
+        conjugacy = [0]*length
 
-    def frobenius_coordinates(self) -> list:
-        '''
-        Frobenius coordinates for a given partition.
+        for i in self.partition:
+            conjugacy[i-1] += 1
 
-        The minus in the definition below is related
-        to the fact that python lists start at 0 and not 1.
-        Moreover, the method uses the definition where the coordinates
-        are half integers. 
-        '''
+        # We finally create a dictionary for the conjugacy class
+        conjugacy_class = dict(enumerate(conjugacy,1)) 
 
-        transposed_diagram = self.transpose().partition
-        FrobCoor = []
-        for i in range(self.count_diagonal()):
-            FrobCoor.append([self.partition[i] - i - sp.Rational(1,2),
-                             -(transposed_diagram[i] - i - sp.Rational(1,2))])
-        return FrobCoor
+        return conjugacy_class
 
 
     def transpose(self) -> YoungDiagram:
         '''
         Gives the transposed (or conjugate) Young diagram. 
         For example, the conjugate of [3,2] is [2,2,1].
 
-        The algorithm follows the logic: 
+        Here I follow an interesting property that Knuth mentions in
+        TAOCP, volume 4A, equation (11) of section 7.2.1.4 - Other
+        representations of partitions. He claims that for any partiton
+        L = (L1, L2, ...), its coeficcients satisfy
+
+                            Li - L(i+1) = LTci
+
+        where LTc is the conjugate of L in the conjugacy class notation. 
+        '''
+
+        m = tuple(self.partition) + (0,) # pad a zero at the end of the partition tuple
+
+        m_transpose_un = np.array([])
+
+        for j in range(len(m)-1):
+            rows = m[j] - m[j+1] # This gives the number of rows of length j+1
+            m_transpose_un = np.append(m_transpose_un, np.array(rows * [j+1]))
+
 
-        The method builds a list of zeros and length equal
-        to the highest column: that is the partition[0].
-        In our example: partition[0]=3, then [0,0,0]
+        m_transpose = -np.sort(-m_transpose_un, axis=0) # Sorts the numpy array in decreasing order.
+        m_transpose = m_transpose.astype(int) # Converts entries into integers
 
-        We now fill in the list defined above, we loop over
-        the length of the original partition, in our case i =1, 2
+        return YoungDiagram(tuple(m_transpose))
 
-        transposed_diagram = [0,0,0]
 
-        - loop 01: (i, row_length) = (0,3) => j =0,1,2. 
-                j = 0 transporsed_diagram[0] = 1
-                j = 1 transposed_diagram[1] = 1
-                j = 2 transposed diagram[2] = 1
-        and now we have transposed_diagram = [1,1,1]
-        - loop 02 (i, row_length) = (1, 2) => j =0,1
-                j = 0 transposed_diagram[0] = 2
-                j = 1 transposed_diagram[0] = 2
-        and now we have transposed_diagram = [2,2,1]
+    def frobenius_coordinates(self, fermionic: bool=True) -> list:
         '''
-        transposed_diagram = [0] * (self.partition[0])
+        Frobenius coordinates for the diagrams are determined as follows:
 
-        for i, row_length in enumerate(self.partition):
-            for j in range(row_length):
-                transposed_diagram[j] += 1
+        Given a partition L = (L1, L2, ...), the Frobenius coordinates
+        are defined by (a_n , b_n), where a_n = L_n -n and b_n - L'_n - n,
+        (the prime denotes the conjugate diagram). Note that
+        we subtract 1 because Python lists start at 0. For fermionic
+        representations (which are the default), we need to add 1/2 because
+        indices are half-integers. Therefore, an overall offset of -1/2 is
+        required for fermionic representation, while -1 suffices for the
+        standard representation.
 
-        transposed_diagram_tuple = tuple(transposed_diagram)
+        Additionally, I prefer to consider the representation where all
+        negative sites are occupied. Thus, in the fermionic
+        representation, I adjust the notation to -b for clarity.
+        '''
+
+        if fermionic:
+            sign = -1
+            offset = - sp.Rational(1,2)
+        else: 
+            sign = 1
+            offset = - 1
+
+        partition = self.partition
+        conjugate = self.transpose().partition
+        FrobCoor = []
 
-        return YoungDiagram(transposed_diagram_tuple)
+        short = min([partition, conjugate], key=len)
+
+        for m in range(len(short)):
+
+            alpha = partition[m] - m + offset
+            beta  = conjugate[m] - m + offset
+
+            if alpha < 0 or beta < 0: 
+                break
+
+            FrobCoor.append((alpha, sign * beta))
+
+        return FrobCoor
 
 
     def contains(self, other_young: YoungDiagram) -> bool:
         '''
         Checks if the original partition contains the new one.
         '''
 
@@ -176,20 +234,19 @@
 
         # Pad some zeros to write the two partitions in the same form (length).
         if len(other_partition) < len(partition):
             other_partition += (0,)*abs(len(partition) - len(other_partition))
         elif len(other_partition) > len(partition):
             partition += (0,)*abs(len(partition) - len(other_partition))
 
-        sub_partition_condition = [x >= y for x, y in zip(partition, other_partition)]
+        for x,y in zip(partition, other_partition):
+            if x < y:
+                return False
 
-        if all(sub_partition_condition):
-            return True
-        else:
-            return False
+        return True
 
 
     def interlaces(self, other_young: YoungDiagram) -> bool:
         '''
         Checks if the original partition interlaces the new one.
         '''
 
@@ -199,64 +256,17 @@
 
         # Here I pad some zeros to write the two partitions in the same form (length).
         if len(other_partition) < len(partition):
             other_partition += (0,)*abs(len(partition) - len(other_partition))
         elif len(other_partition) > len(partition):
             partition += (0,)*abs(len(partition) - len(other_partition))
 
-        interlacing_condition   = [x >= y for x, y in zip(other_partition, partition[1:])]
-
-        if self.contains(other_young) and all(interlacing_condition):
-            return True
-        else:
+        if not self.contains(other_young):
             return False
+        else:
+            for x,y in zip(other_partition, partition[1:]):
+                if x < y:
+                    return False
 
+        return True
+            
 
-    def conjugacy_partition(self) -> dict:
-        '''
-        Converts the partition notation to 
-        the conjugacy class notation
-        Example:
-        [4,4,4,2,2,1] to {1: 1, 2: 2, 3: 0, 4: 3}.
-
-        The algorithm works as follows:
-
-        It creates a list of zeros with length equal
-        to the largest row. In our case, 4
-        conjugacy = [0, 0, 0, 0].
-
-        It iterates over the partition, adding 1s to the
-        corresponding slot in the conjugacy vector, for example
-        partition (4,4,4,2,2,1) gives
-        - loop 01: i = 4
-            conjugacy[3] = 1
-            conjugacy = [0,0,0,1]
-        - loop 02: i = 4
-            conjugacy[3] = 2
-            conjugacy = [0,0,0,2]
-        - loop 03: i = 4
-            conjugacy[3] = 3
-            conjugacy = [0,0,0,3]
-        - loop 04: i = 2
-            conjugacy[1] = 1
-            conjugacy = [0,1,0,3]
-        - loop 05: i = 2
-            conjugacy[1] = 2
-            conjugacy = [0,2,0,3]
-        - loop 06: i = 1
-            conjugacy[0] = 1
-            conjugacy = [1,2,0,3]
-
-        At the end we convert to a dictionary, and
-        conjugacy = {1: 1, 2: 2, 3: 0, 4: 3}
-        '''
-
-        length = self.partition[0]
-        conjugacy = [0]*length
-
-        for i in self.partition:
-            conjugacy[i-1] += 1
-
-        # We finally create a dictionary for the conjugacy class
-        conjugacy_class = dict(enumerate(conjugacy,1)) 
-
-        return conjugacy_class
```

### Comparing `pysymmpol-0.1.1/pysymmpol/polynomials/elementary.py` & `pysymmpol-0.1.2/pysymmpol/polynomials/elementary.py`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/pysymmpol/polynomials/hall.py` & `pysymmpol-0.1.2/pysymmpol/polynomials/hall.py`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/pysymmpol/polynomials/homogeneous.py` & `pysymmpol-0.1.2/pysymmpol/polynomials/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/pysymmpol/polynomials/monomial.py` & `pysymmpol-0.1.2/pysymmpol/polynomials/monomial.py`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/pysymmpol/polynomials/schur.py` & `pysymmpol-0.1.2/pysymmpol/polynomials/schur.py`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/pysymmpol/utils/tools.py` & `pysymmpol-0.1.2/pysymmpol/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysymmpol-0.1.1/PKG-INFO` & `pysymmpol-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysymmpol
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package for manipulation of symmetric polynomials.
 License: GPL-3.0
 Author: Thiago Araujo
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
@@ -29,22 +29,24 @@
     3. Monomial symmetric polynomials 
     4. Schur polynomials
     5. Hall-Littlewood polynomials
 
 Additionally, the package contains a module with basic functionalities
 for manipulating integer partitions and Young diagrams.
 
+Read our Statement of need [here](STATEMENT-OF-NEED.md).
+
 Tutorials can be found in the [documentation page](https://thraraujo.github.io/pysymmpol/index.html).
 
 ## Dependencies
 
 This package has been tested with the following versions:
-- Python 3.12
-- SymPy 1.12
-- NumPy 1.26.4
+- Python >= 3.11
+- SymPy >= 1.11
+- NumPy >= 1.26.2
 
 ## Installation
 
 The package can be installed with pip:
 ```bash
 $ pip install pysymmpol
 ```
@@ -105,15 +107,15 @@
 ```python
 n = 3
 t = create_miwa(n)
 
 homogeneous = HomogeneousPolynomial(n)
 elementary = ElementaryPolynomial(n)
 print(f"homogeneous: {homogeneous.explicit(t)}")
-print(f"elementary: {elementary.explicit(t)})
+print(f"elementary: {elementary.explicit(t)}")
 ```
 gives the output 
 ```
 homogeneous: t1**3/6 + t1*t2 + t3
 elementary: t1**3/6 - t1*t2 + t3
 ```
 
@@ -193,14 +195,25 @@
 print(f"hall-littlewood: {hall_littlewood.explicit(x, Q)}")
 ```
 gives
 ```
 hall-littlewood: x1*x2*x3*(-Q**2*x1*x2*x3 - Q*x1*x2*x3 + x1**2*x2 + x1**2*x3 + x1*x2**2 + 2*x1*x2*x3 + x1*x3**2 + x2**2*x3 + x2*x3**2)
 ```
 
+# References
+
+Here are some recommended resources covering symmetric polynomials,
+combinatorics, and their significance in theoretical physics:
+
+- [Symmetric Functions and Hall Polynomials - Ian Macdonald](https://books.google.com.br/books/about/Symmetric_Functions_and_Hall_Polynomials.html?id=srv90XiUbZoC&redir_esc=y)
+- [An Introduction to Symmetric Functions and Their Combinatorics - Eric S. Egge](https://bookstore.ams.org/stml-91)
+- [Counting with Symmetric Functions - Mendes and Remmel](https://link.springer.com/book/10.1007/978-3-319-23618-6)
+- [Solitons: Differential Equations, Symmetries and Infinite Dimensional Algebras - Miwa, Jimbo and Date](https://books.google.com.br/books/about/Solitons.html?id=kQDw1ZcqLjUC&redir_esc=y)
+- [The uses of random partitions - Andrei Okounkov](https://arxiv.org/abs/math-ph/0309015)
+
 # Citation & Contributing
 
 If you found this package useful in your research, please consider citing the companion 
 paper available here: [arxiv.org/abs/2403.13580](https://arxiv.org/abs/2403.13580). 
 ```
 @article{Araujo:2024piv,
     author = "Araujo, Thiago",
```

