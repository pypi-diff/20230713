# Comparing `tmp/jijmodeling-1.0.0rc2-cp39-none-win_amd64.whl.zip` & `tmp/jijmodeling-1.0.0rc3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 740811 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2702 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/WHEEL
--rw-r--r--  4.6 unx     3445 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx      127 b- defN 23-Jul-11 02:43 jijmodeling/__init__.py
--rw-r--r--  4.6 unx    81515 b- defN 23-Jul-11 02:43 jijmodeling/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-11 02:43 jijmodeling/py.typed
--rwxr-xr-x  4.6 unx  2157568 b- defN 23-Jul-11 02:43 jijmodeling/jijmodeling.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      677 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/RECORD
-8 files, 2246128 bytes uncompressed, 739627 bytes compressed:  67.1%
+Zip file size: 743481 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2902 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3445 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      127 b- defN 23-Jul-13 11:16 jijmodeling/__init__.py
+-rw-r--r--  4.6 unx   129449 b- defN 23-Jul-13 11:16 jijmodeling/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-13 11:16 jijmodeling/py.typed
+-rwxr-xr-x  4.6 unx  2172928 b- defN 23-Jul-13 11:16 jijmodeling/jijmodeling.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      678 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/RECORD
+8 files, 2309623 bytes uncompressed, 742297 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: jijmodeling-1.0.0rc2.dist-info/METADATA
+Filename: jijmodeling-1.0.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: jijmodeling-1.0.0rc2.dist-info/WHEEL
+Filename: jijmodeling-1.0.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt
+Filename: jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: jijmodeling/__init__.py
 Comment: 
 
 Filename: jijmodeling/__init__.pyi
 Comment: 
 
 Filename: jijmodeling/py.typed
 Comment: 
 
 Filename: jijmodeling/jijmodeling.cp39-win_amd64.pyd
 Comment: 
 
-Filename: jijmodeling-1.0.0rc2.dist-info/RECORD
+Filename: jijmodeling-1.0.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jijmodeling/__init__.pyi

```diff
@@ -1,8 +1,8 @@
-import typing
+import typing, enum
 
 @typing.final
 class AbsOp:
     """
     A class for representing the absolute value
     
     The AbsOp class is used to represent the absolute value.
@@ -10,17 +10,116 @@
     
     Attributes:
         operand: The operand.
     
     Note:
         The AbsOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -41,28 +140,127 @@
         terms: A sequence of operands to be added.
     
     Note:
         The AddOp class does not have a constructor. Its intended
         instantiation method is by calling the addition operation on other
         expressions.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
         pass
 
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 @typing.final
 class AndOp:
     """
     A class for representing logical AND
     
     The AndOp class is used to represent logical AND (`&`) of an arbitrary number of operands.
     For example `a & b & c & d` would be one AndOp object.
@@ -70,28 +268,78 @@
     
     Attributes:
         terms: A sequence of operands to apply the AND operation.
     
     Note:
         The AndOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
         pass
 
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 @typing.final
 class ArrayLength:
     """
     A class for referring to the length of an array at a given axis.
     
     The ArrayLength class is to refer to the number of elements of an axis in an array.
     
@@ -109,17 +357,118 @@
     Examples:
         Create a length of axis 0 in a 2-dimensional placeholder.
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
         >>> N = a.len_at(0, latex="N")
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
         pass
 
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    array: typing.Any
+    axis: typing.Any
+    description: str
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -163,45 +512,225 @@
         Create a 1-dimensional binary variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.BinaryVar("x", shape=[124])
         >>> x[123]
         BinaryVar(name='x', shape=[NumberLit(value=124)])[NumberLit(value=123)]
     """
-    def __init__(name: str, *, shape=None, latex=None, description=None):
+    def __new__(cls, name: str, *, shape=None, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
         pass
 
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    description: str
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
 @typing.final
 class CeilOp:
     """
     A class for representing the ceil operator
     
     The CeilOp class is used to represent the ceil operator.
     The number of dimensions of the operand is zero.
     
     Attributes:
         operand: The operand.
     
     Note:
         The CeilOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
         pass
 
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -257,17 +786,26 @@
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N, N))
         >>> jm.Constraint("constraint", x[i,j] <= 2, forall=[i, (j, j != i)])
         {'expression': x[i, j] <= 2, 'forall': [i, (j, j != i)]}
         
     """
-    def __init__(name: str, expression, *, forall=None):
+    def __new__(cls, name: str, expression, *, forall=None):
+        pass
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    expression: typing.Any
+    forall: typing.Any
     def is_equality(self, /):
         """
         Returns true if the constraint is an equality constraint.
         
         Returns:
             bool: True if the constraint is an equality constraint. Otherwise, False.
         
@@ -296,22 +834,29 @@
             >>> x = jm.BinaryVar("x", shape=(N,))
             >>> constraint = jm.Constraint("constraint", jm.sum(i, x[i]) <= 1)
             >>> assert constraint.is_inequality()
         """
         pass
 
 
+    left: typing.Any
+    name: str
+    right: typing.Any
+    sense: typing.Any
 @typing.final
 class ConstraintSense:
     """
     Equality of a constraint
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    EQUAL: ConstraintSense
+    GREATER_THAN_EQUAL: ConstraintSense
+    LESS_THAN_EQUAL: ConstraintSense
 @typing.final
 class ContinuousVar:
     """
     A class for creating a continuous variable
     
     The ContinuousVar class is used to create a continuous variable.
     The lower and upper bounds of the variable can be specified by:
@@ -360,28 +905,111 @@
         Create a 1-dimensional continuous variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.ContinuousVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
         ContinuousVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
-    def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+    def __new__(cls, name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
         pass
 
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    description: str
+    lower_bound: typing.Any
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
+    upper_bound: typing.Any
 @typing.final
 class CustomPenaltyTerm:
     """
     A class for creating a custom penalty term
     
     The CustomPenaltyTerm class is used to create a custom penalty term.
     
@@ -424,25 +1052,104 @@
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N, N))
         >>> jm.CustomPenaltyTerm("custom penalty term", (x[i,j] - 2)**2, forall=[i, (j, j != i)])  # doctest: +ELLIPSIS
         <jijmodeling.CustomPenaltyTerm object at 0x...>
     """
-    def __init__(name: str, expression, *, forall=None):
+    def __new__(cls, name: str, expression, *, forall=None):
+        pass
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    expression: typing.Any
+    forall: typing.Any
+    name: str
 @typing.final
 class DataType:
     """
     
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    FLOAT: DataType
+    INTEGER: DataType
+@typing.final
+class DummyIndexedVar:
+    """
+    A class for representing a subscripted variable with dummy indices
+    
+    The DummyIndexedVar class is an intermediate representation to support syntactic sugar of sum/prod with slices.
+    
+    Note:
+        The DummyIndexedVar class does not have a constructor.
+    """
+    def __new__(cls):
+        pass
+
+    def prod(self, /):
+        """
+        Take a prod of the decision variable over the elements for which the slice is given and return a ProdOp object.
+        
+        Returns:
+            ProdOp: A ProdOp object taken a prod of the decision variable over the elements for which the slice is given.
+        
+        Note:
+            An automatically created dummy index
+            - has a name of the form `__dummy_{decision_var.name}_{axis}` where `axis` is the axis of the slice.
+            - belongs to a range whose start defaults to 0 and end defaults to the length of the axis.
+            - has description of the form `dummy index at {axis} for {decision_var.name}`.
+            - has latex string of the form `\\ast_{axis}`.
+        
+        Examples:
+            Create a prodOp object taken a prod of the 2-dim binary variable over the 0-th elements for which the slice is given.
+        
+            >>> import jijmodeling as jm
+            >>> n = jm.Placeholder("n")
+            >>> x = jm.BinaryVar("x", shape=(n, n))
+            >>> i = jm.Element("__dummy_x_0", belong_to=n)
+            >>> j = jm.Element("j", belong_to=n)
+            >>> assert jm.is_same(x[:, j].prod(), jm.prod(i, x[i, j]))
+        """
+        pass
+
+
+    def sum(self, /):
+        """
+        Take a sum of the decision variable over the elements for which the slice is given and return a SumOp object.
+        
+        Returns:
+            SumOp: A SumOp object taken a sum of the decision variable over the elements for which the slice is given.
+        
+        Note:
+            An automatically created dummy index
+            - has a name of the form `__dummy_{decision_var.name}_{axis}` where `axis` is the axis of the slice.
+            - belongs to a range whose start defaults to 0 and end defaults to the length of the axis.
+            - has description of the form `dummy index at {axis} for {decision_var.name}`.
+            - has latex string of the form `\\ast_{axis}`.
+        
+        Examples:
+            Create a SumOp object taken a sum of the 2-dim binary variable over the 0-th elements for which the slice is given.
+        
+            >>> import jijmodeling as jm
+            >>> n = jm.Placeholder("n")
+            >>> x = jm.BinaryVar("x", shape=(n, n))
+            >>> i = jm.Element("__dummy_x_0", belong_to=n)
+            >>> j = jm.Element("j", belong_to=n)
+            >>> assert jm.is_same(x[:, j].sum(), jm.sum(i, x[i, j]))
+        """
+        pass
+
+
 @typing.final
 class Element:
     """
     A class for creating an element
     
     The Element class is used to create an element.
     It is used in the following cases:
@@ -492,35 +1199,145 @@
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
         >>> e = jm.Element("e", belong_to=a)
         >>> e[123]
         Element(name='e', belong_to=Placeholder(name='a', ndim=2))[NumberLit(value=123)]
     """
-    def __init__(name: str, *, belong_to, latex=None, description=None):
+    def __new__(cls, name: str, *, belong_to, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
         pass
 
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    belong_to: typing.Any
+    description: str
     def len_at(self, /, axis, *, latex=None, description=None):
         """
         
         """
         pass
 
 
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
 @typing.final
 class EqualOp:
     """
     A class for representing the equal operator
     
     The EqualOp class is used to represent the equal operator (`==`).
     The number of dimensions of each operand is zero.
@@ -528,17 +1345,68 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The EqualOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
         pass
 
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -557,42 +1425,51 @@
         energy (numpy.ndarray): The value of energy of each sample.
         objective (numpy.ndarray): The value of an objective function of each sample.
         constraint_violations (dict[str, numpy.ndarray]): The constraint violation of each sample.
         constraint_forall (dict[str, numpy.ndarray]): The constraint forall of each sample.
         constraint_values (numpy.ndarray): The constraint value of each sample.
         penalty (dict[str, numpy.ndarray]): The penalty of each sample.
     """
-    def __init__(energy=Ellipsis, objective=Ellipsis, constraint_violations=Ellipsis, constraint_forall=Ellipsis, constraint_values=Ellipsis, penalty=Ellipsis):
+    def __new__(cls, energy=Ellipsis, objective=Ellipsis, constraint_violations=Ellipsis, constraint_forall=Ellipsis, constraint_values=Ellipsis, penalty=Ellipsis):
         pass
 
+    constraint_expr_values: typing.Any
+    constraint_forall: typing.Any
+    constraint_values: typing.Any
+    constraint_violations: typing.Any
+    energy: typing.Any
+    @staticmethod
     def from_dict(dict):
         """
         Create a Evaluation object from the given dict.
         
         If a key is not the name of the Evaluation fields, the value value is ignored.
         
         Args:
             dict: A dict whose keys are name of the Evaluation fields.
         """
         pass
 
 
+    @staticmethod
     def from_json(json):
         """
         Create a Evaluation object from the JSON string.
         
         Args:
             json (str): A JSON string.
         
         Returns:
             Evaluation: An Evaluation object.
         """
         pass
 
 
+    objective: typing.Any
+    penalty: typing.Any
     def to_dict(self, /):
         """
         Convert into a dict.
         
         Returns:
             dict: A dict whose keys are name of the Evaluation's fields.
         """
@@ -632,17 +1509,116 @@
     
     Attributes:
         operand: The operand.
     
     Note:
         The FloorOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
         pass
 
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -661,17 +1637,68 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The GreaterThanEqualOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -690,17 +1717,68 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The GreaterThanOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
         pass
 
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -760,28 +1838,111 @@
         Create a 1-dimensional integer variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.IntegerVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
         IntegerVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
-    def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+    def __new__(cls, name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
         pass
 
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    description: str
+    lower_bound: typing.Any
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
+    upper_bound: typing.Any
 @typing.final
 class LessThanEqualOp:
     """
     A class for representing the less than equal operator
     
     The LessThanEqualOp class is used to represent the less than equal operator (`<=`).
     The number of dimensions of each operand is zero.
@@ -789,17 +1950,68 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The LessThanEqualOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -818,17 +2030,68 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The LessThanOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
         pass
 
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -846,17 +2109,116 @@
     
     Attributes:
         operand: The operand.
     
     Note:
         The LnOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
         pass
 
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -874,17 +2236,116 @@
     
     Attributes:
         operand: The operand.
     
     Note:
         The Log10Op class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
         pass
 
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -902,17 +2363,116 @@
     
     Attributes:
         operand: The operand.
     
     Note:
         The Log2Op class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
         pass
 
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -931,41 +2491,141 @@
     Attributes:
         terms: A sequence of operands.
     
     Note:
         The MaxOp class does not have a constructor. Its intended
         instantiation method is by calling the `max` function.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 @typing.final
 class MeasuringTime:
     """
     A class for storing time to be measured.
     
     Attributes:
         solve (SolvingTime): Time to solve the problem.
         system (SystemTime): Time to measure system time.
         total (float, optional): Total time to solve the problem. Defaults to None.
     """
-    def __init__(solve=Ellipsis, system=Ellipsis, total=None):
+    def __new__(cls, solve=Ellipsis, system=Ellipsis, total=None):
         pass
 
+    @staticmethod
     def from_dict(dict):
         """
         Create a MeasuringTime object from the given dict.
         
         If a key is not the name of the MeasuringTime fields, the value value is ignored.
         
         Args:
@@ -973,27 +2633,30 @@
         
         Returns:
             A MeasuringTime object.
         """
         pass
 
 
+    @staticmethod
     def from_json(json):
         """
         Create a MeasuringTime object from the JSON string.
         
         Args:
             json (str): A JSON string.
         
         Returns:
             MeasuringTime: A MeasuringTime object.
         """
         pass
 
 
+    solve: typing.Any
+    system: typing.Any
     def to_dict(self, /):
         """
         Convert into a dict.
         
         Returns:
             dict: A dict whose keys are name of the MeasuringTime's fields.
         """
@@ -1009,14 +2672,15 @@
         
         Note:
             A numpy array is serialized into a list.
         """
         pass
 
 
+    total: typing.Any
 @typing.final
 class MinOp:
     """
     A class for representing the minimum value.
     
     The MinOp class is used to represent the minimum value of operands.
     The number of dimensions of each operand is zero.
@@ -1024,28 +2688,127 @@
     Attributes:
         terms: A sequence of operands.
     
     Note:
         The MinOp class does not have a constructor. Its intended
         instantiation method is by calling the `min` function.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 @typing.final
 class ModOp:
     """
     A class for representing modulo
     
     The ModOp class is used to represent modulo (or remainder) (`%`).
     The number of dimensions of each operand is zero.
@@ -1053,36 +2816,137 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The ModOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
 @typing.final
-class ModelingError:
+class ModelingError(BaseException):
     """
     Common base class for all non-exit exceptions.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    args: typing.Any
     def with_traceback():
         """
         Exception.with_traceback(tb) --
         set self.__traceback__ to tb and return self.
         """
         pass
 
@@ -1100,28 +2964,127 @@
         terms: A sequence of operands to be multiplied.
     
     Note:
         The MulOp class does not have a constructor. Its intended
         instantiation method is by calling the multiplication operation on other
         expressions.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
         pass
 
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 @typing.final
 class NotEqualOp:
     """
     A class for representing the not equal operator
     
     The NotEqualOp class is used to represent the not equal operator (`!=`).
     The number of dimensions of each operand is zero.
@@ -1129,17 +3092,68 @@
     Attributes:
         left: The left-hand operand.
         right: The right-hand operand.
     
     Note:
         The NotEqualOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    left: typing.Any
+    right: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -1176,17 +3190,117 @@
         Create a number literal with a float value `1.23`.
     
         >>> import jijmodeling as jm
         >>> v = jm.NumberLit(1.23)
         >>> assert v.value == 1.23
         >>> assert v.dtype == jm.DataType.FLOAT
     """
-    def __init__(value):
+    def __new__(cls, value):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    dtype: typing.Any
+    value: typing.Any
 @typing.final
 class OrOp:
     """
     A class for representing logical OR
     
     The OrOp class is used to represent logical OR (`|`) of an arbitrary number of operands.
     For example `a | b | c | d` would be one OrOp object.
@@ -1194,28 +3308,78 @@
     
     Attributes:
         terms: A sequence of operands to apply the OR operation.
     
     Note:
         The OrOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
+        pass
+
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
         pass
 
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 @typing.final
 class Placeholder:
     """
     A class for creating a placeholder
     
     The Placeholder class is used to create a placeholder.
     It is a symbol to be replaced by a numerical value when you solve an optimization problem.
@@ -1253,35 +3417,144 @@
         Create a 1-dimensional placeholder with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
         >>> a[123]
         Placeholder(name='a', ndim=2)[NumberLit(value=123)]
     """
-    def __init__(name: str, *, ndim=0, latex=None, description=None):
+    def __new__(cls, name: str, *, ndim=0, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
         pass
 
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    description: str
     def len_at(self, /, axis, *, latex=None, description=None):
         """
         
         """
         pass
 
 
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
 @typing.final
 class PowOp:
     """
     A class for representing the power operator
     
     The ModOp class is used to represent the power operator(`**`).
     The number of dimensions of each operand is zero.
@@ -1289,17 +3562,117 @@
     Attributes:
         base: The base operand.
         exponent: The exponent operand.
     
     Note:
         The PowOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    base: typing.Any
+    exponent: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -1323,25 +3696,39 @@
         custom_penalty_terms (dict): A dictionary that stores custom penalty terms.
             A key is the name of a custom penalty and the value is the custom penalty object.
     
     Args:
         name (str): A name of the optimization problem.
         sense (optional): Sense of the optimization problem. Defaults to :obj:`ProblemSense.MINIMIZE`.
     """
-    def __init__(name: str, *, sense=Ellipsis):
+    def __new__(cls, name: str, *, sense=Ellipsis):
+        pass
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    constraints: typing.Any
+    custom_penalty_terms: typing.Any
+    name: str
+    objective: typing.Any
+    sense: typing.Any
 @typing.final
 class ProblemSense:
     """
     An optimization sense
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    MAXIMIZE: ProblemSense
+    MINIMIZE: ProblemSense
 @typing.final
 class ProdOp:
     """
     A class for representing product
     
     The ProdOp class is used to represent product.
     The number of dimensions of the opreand is zero.
@@ -1350,52 +3737,155 @@
         index: The index of product.
         condition: The condition for the product index.
         operand: The opreand.
     
     Note:
         The ProdOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    condition: typing.Any
+    index: typing.Any
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
 @typing.final
-class ProtobufDeserializationError:
+class ProtobufDeserializationError(BaseException):
     """
     Common base class for all non-exit exceptions.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    args: typing.Any
     def with_traceback():
         """
         Exception.with_traceback(tb) --
         set self.__traceback__ to tb and return self.
         """
         pass
 
 
 @typing.final
-class ProtobufSerializationError:
+class ProtobufSerializationError(BaseException):
     """
     Common base class for all non-exit exceptions.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    args: typing.Any
     def with_traceback():
         """
         Exception.with_traceback(tb) --
         set self.__traceback__ to tb and return self.
         """
         pass
 
@@ -1411,17 +3901,19 @@
     Attributes:
         start: The lower bound of the range (inclusive).
         end: The upper bound of the range (exclusive).
     
     Note:
         This class does not contain any decision variable.
     """
-    def __init__():
+    def __new__(cls):
         pass
 
+    end: typing.Any
+    start: typing.Any
 @typing.final
 class Record:
     """
     A class for representing a record.
     
     There are two types of solutions that can be given; dense solutions and sparse solutions.
     A dense solution is a dict whose key is a variable name and the value is a list of numpy.ndarray.
@@ -1448,17 +3940,18 @@
     }
     ```
     
     Attributes:
         solution (Union[Dict[str, List[numpy.ndarray]], Dict[str, List[Tuple[List[int], List[float], Tuple[int, ...]]]]]): A solution.
         num_occurrences (List[int]): A list of the number of occurrences in which the solution is observed.
     """
-    def __init__(solution, num_occurrences):
+    def __new__(cls, solution, num_occurrences):
         pass
 
+    @staticmethod
     def from_dict(dict):
         """
         Create a Record object from the given dict.
         
         If a key is not one of "solution" or "num_occurrences", the value is ignored.
         
         Args:
@@ -1466,14 +3959,15 @@
         
         Returns:
             A Record object.
         """
         pass
 
 
+    @staticmethod
     def from_json(json):
         """
         Create a Record object from the JSON string.
         
         Args:
             json (str): A JSON string.
         
@@ -1499,14 +3993,16 @@
         
         Returns:
             bool: True if the solution is sparse.
         """
         pass
 
 
+    num_occurrences: typing.Any
+    solution: typing.Any
     def to_dense(self, /):
         """
         Return a Record object whose solution is dense.
         If the solution is already dense, the solution is not converted.
         Otherwise, the solution is converted into a dense solution.
         
         Returns:
@@ -1568,17 +4064,18 @@
     Attributes:
         post_problem_and_instance_data (float, optional): Time to upload problem and instance_data to blob. Defaults to None.
         request_queue (float, optional): Time to send request to queue. Defaults to None.
         fetch_problem_and_instance_data (float, optional): Time to fetch problme and instance_data from blob. Defaults to None.
         fetch_result (float, optional): Time to fetch result. Defaults to None.
         deserialize_solution (float, optional): Time to deserialize json object. Defaults to None.
     """
-    def __init__(record, evaluation, measuring_time, metadata=None):
+    def __new__(cls, record, evaluation, measuring_time, metadata=None):
         pass
 
+    evaluation: typing.Any
     def feasible(self, /, rtol=1e-05, atol=1e-08):
         """
         Return a Sampleset with only feasible solutions.
         If there is no feasible solution, the record and evaluation are empty.
         
         Args:
             rtol (float): The relative tolerance parameter. Defaults to 1e-5.
@@ -1590,14 +4087,15 @@
         Note:
             The feasible solutions are determined by the following condition:
             $$ |0 - v| \\leq \\mathrm{atol} + \\mathrm{rtol} \\cdot |v| $$
         """
         pass
 
 
+    @staticmethod
     def from_dict(dict):
         """
         Create a SampleSet object from the given dict.
         
         If a key is not the name of the SampleSet fields, the value value is ignored.
         
         Args:
@@ -1605,14 +4103,15 @@
         
         Returns:
             A SampleSet object.
         """
         pass
 
 
+    @staticmethod
     def from_json(json):
         """
         Create a SampleSet object from the JSON string.
         
         Args:
             json (str): A JSON string.
         
@@ -1686,14 +4185,17 @@
         Note:
             The feasible solutions are determined by the following condition:
             $$ |0 - v| \\leq \\mathrm{atol} + \\mathrm{rtol} \\cdot |v| $$
         """
         pass
 
 
+    measuring_time: typing.Any
+    metadata: typing.Any
+    record: typing.Any
     def to_dense(self, /):
         """
         Return a Sampleset whose record is converted into a dense solution format.
         If the record is already a dense solution format, return itself.
         
         Returns:
             SampleSet: A SampleSet object.
@@ -1786,28 +4288,111 @@
         Create a 1-dimensional semi-continuous variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.SemiContinuousVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
         SemiContinuousVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
-    def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+    def __new__(cls, name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
         pass
 
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    description: str
+    lower_bound: typing.Any
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
+    upper_bound: typing.Any
 @typing.final
 class SemiIntegerVar:
     """
     A class for creating a semi-integer variable
     
     The SemiIntegerVar class is used to create a semi-integer variable.
     The lower and upper bounds of the variable can be specified by:
@@ -1856,41 +4441,125 @@
         Create a 1-dimensional semi-integer variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.SemiIntegerVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
         SemiIntegerVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
-    def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+    def __new__(cls, name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
+    description: str
+    lower_bound: typing.Any
+    name: str
+    ndim: int
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    shape: tuple
+    upper_bound: typing.Any
 @typing.final
 class SolvingTime:
     """
     A class for storing time to solve a problem.
     
     Attributes:
         preprocess (float, optional): Time to preprocess the problem. Defaults to None.
         solve (float, optional): Time to solve the problem. Defaults to None.
         postprocess (float, optional): Time to postprocess the problem. Defaults to None.
     """
-    def __init__(preprocess=None, solve=None, postprocess=None):
+    def __new__(cls, preprocess=None, solve=None, postprocess=None):
         pass
 
+    @staticmethod
     def from_dict(dict):
         """
         Create a SolvingTime object from the given dict.
         
         If a key is not one of "preprocess", "solve", or "postprocess", the value is ignored.
         
         Args:
@@ -1898,27 +4567,31 @@
         
         Returns:
             A SolvingTime object.
         """
         pass
 
 
+    @staticmethod
     def from_json(json):
         """
         Create a SolvingTime object from the JSON string.
         
         Args:
             json (str): A JSON string.
         
         Returns:
             SolvingTime: A SolvingTime object.
         """
         pass
 
 
+    postprocess: typing.Any
+    preprocess: typing.Any
+    solve: typing.Any
     def to_dict(self, /):
         """
         Convert into a dict.
         
         Returns:
             dict: A dict with keys "preprocess", "solve", and "postprocess".
         """
@@ -1949,24 +4622,133 @@
         variable: A variable that has subscripts.
         subscripts (list): A list of subscripts.
         ndim (int): The number of dimensions of the subscripted variable.
     
     Note:
         The Subscript class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __getitem__(self, key, /):
+        """
+        Return self[key].
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
+        pass
+
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
         pass
 
+
     def len_at(self, /, axis, *, latex=None, description=None):
         """
         
         """
         pass
 
 
+    ndim: int
+    shape: tuple
+    subscripts: typing.Any
+    variable: typing.Any
 @typing.final
 class SumOp:
     """
     A class for representing summation
     
     The SumOp class is used to represent summation.
     The number of dimensions of the opreand is zero.
@@ -1975,17 +4757,118 @@
         index: The index of summation.
         condition: The condition for the summation index.
         operand: The opreand.
     
     Note:
         The SumOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __add__(self, value, /):
+        """
+        Return self+value.
+        """
+        pass
+
+
+    def __mod__(self, value, /):
+        """
+        Return self%value.
+        """
+        pass
+
+
+    def __mul__(self, value, /):
+        """
+        Return self*value.
+        """
+        pass
+
+
+    def __neg__(self, /):
+        """
+        -self
+        """
+        pass
+
+
+    def __pow__(self, value, mod=None, /):
+        """
+        Return pow(self, value, mod).
+        """
+        pass
+
+
+    def __radd__(self, value, /):
+        """
+        Return value+self.
+        """
+        pass
+
+
+    def __rmod__(self, value, /):
+        """
+        Return value%self.
+        """
+        pass
+
+
+    def __rmul__(self, value, /):
+        """
+        Return value*self.
+        """
+        pass
+
+
+    def __rpow__(self, value, mod=None, /):
+        """
+        Return pow(value, self, mod).
+        """
         pass
 
+
+    def __rsub__(self, value, /):
+        """
+        Return value-self.
+        """
+        pass
+
+
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
+    def __sub__(self, value, /):
+        """
+        Return self-value.
+        """
+        pass
+
+
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
+    condition: typing.Any
+    index: typing.Any
+    operand: typing.Any
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
@@ -2001,17 +4884,21 @@
     Attributes:
         post_problem_and_instance_data (float, optional): Time to upload problem and instance_data to blob. Defaults to None.
         request_queue (float, optional): Time to send request to queue. Defaults to None.
         fetch_problem_and_instance_data (float, optional): Time to fetch problme and instance_data from blob. Defaults to None.
         fetch_result (float, optional): Time to fetch result. Defaults to None.
         deserialize_solution (float, optional): Time to deserialize json object. Defaults to None.
     """
-    def __init__(post_problem_and_instance_data=None, request_queue=None, fetch_problem_and_instance_data=None, fetch_result=None, deserialize_solution=None):
+    def __new__(cls, post_problem_and_instance_data=None, request_queue=None, fetch_problem_and_instance_data=None, fetch_result=None, deserialize_solution=None):
         pass
 
+    deserialize_solution: typing.Any
+    fetch_problem_and_instance_data: typing.Any
+    fetch_result: typing.Any
+    @staticmethod
     def from_dict(dict):
         """
         Create a SystemTime object from the given dict.
         
         If a key is not the name of the SystemTime fields, the value value is ignored.
         
         Args:
@@ -2019,27 +4906,30 @@
         
         Returns:
             A SystemTime object.
         """
         pass
 
 
+    @staticmethod
     def from_json(json):
         """
         Create a SystemTime object from the JSON string.
         
         Args:
             json (str): A JSON string.
         
         Returns:
             SystemTime: A SystemTime object.
         """
         pass
 
 
+    post_problem_and_instance_data: typing.Any
+    request_queue: typing.Any
     def to_dict(self, /):
         """
         Convert into a dict.
         
         Returns:
             dict: A dict whose keys are name of the SystemTime's fields.
         """
@@ -2070,28 +4960,78 @@
     
     Attributes:
         terms: A sequence of operands to apply the XOR operation.
     
     Note:
         The XorOp class does not have a constructor.
     """
-    def __init__():
+    def __new__(cls):
+        pass
+
+    def __and__(self, value, /):
+        """
+        Return self&value.
+        """
         pass
 
+
+    def __or__(self, value, /):
+        """
+        Return self|value.
+        """
+        pass
+
+
+    def __rand__(self, value, /):
+        """
+        Return value&self.
+        """
+        pass
+
+
+    def __ror__(self, value, /):
+        """
+        Return value|self.
+        """
+        pass
+
+
+    def __rxor__(self, value, /):
+        """
+        Return value^self.
+        """
+        pass
+
+
+    def __xor__(self, value, /):
+        """
+        Return self^value.
+        """
+        pass
+
+
+    def _repr_latex_(self, /):
+        """
+        
+        """
+        pass
+
+
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
         If the LaTeX representation is not set, the default representation is set.
         
         Args:
             latex (str, optional): LaTeX representation of the object. Defaults to None.
         """
         pass
 
 
+    terms: typing.Any
 def abs(operand):
     """
     Create the `AbsOp` object from the expression.
     
     Args:
         operand: An operand of the abs operator.
```

## Comparing `jijmodeling-1.0.0rc2.dist-info/METADATA` & `jijmodeling-1.0.0rc3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: jijmodeling
-Version: 1.0.0rc2
-Classifier: Development Status :: 3 - Alpha
+Version: 1.0.0rc3
+Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: Other/Proprietary License
+Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: orjson >=3.8.0, <4.0.0
-Requires-Dist: pytest ; extra == 'tests'
-Provides-Extra: tests
+Requires-Dist: pytest ; extra == 'test'
+Requires-Dist: pytest-cov[all] ; extra == 'test'
+Requires-Dist: coverage ; extra == 'test'
+Provides-Extra: test
 License-File: LICENSE.txt
 Summary: Mathematical modeling tool for JijZept
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # JijModeling
```

## Comparing `jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt` & `jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `jijmodeling-1.0.0rc2.dist-info/RECORD` & `jijmodeling-1.0.0rc3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jijmodeling-1.0.0rc2.dist-info/METADATA,sha256=fSd2X1GtPK6PoSf89EL-TL15zhJsLgs_Y6DKiuOkrfA,2702
-jijmodeling-1.0.0rc2.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
-jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt,sha256=llUjgcEN5bUeFlj1RqxJxDMxUnlYvowLsldCF6Lwq8c,3445
+jijmodeling-1.0.0rc3.dist-info/METADATA,sha256=bd0B4Ka_3Ddzsxw14g0LHExIWsFmILfJSJvLA90TsmM,2902
+jijmodeling-1.0.0rc3.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
+jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt,sha256=llUjgcEN5bUeFlj1RqxJxDMxUnlYvowLsldCF6Lwq8c,3445
 jijmodeling/__init__.py,sha256=dTz5lvd2qXlLmjsXX3Pq7v2_dptMkGNTWIf37gSrvwE,127
-jijmodeling/__init__.pyi,sha256=Oz7Eag915tlPXSnkVcQcJPPJrUt12MHQDFFvF3n_mY0,81515
+jijmodeling/__init__.pyi,sha256=SSZHOgCB8V1iH7BaEIh91IrMKYww2okkkzTMd9hjDdg,129449
 jijmodeling/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jijmodeling/jijmodeling.cp39-win_amd64.pyd,sha256=Xx2j5n_4m79uQAj0GsK4sMaIlQIJMKb5-d0E5enTx9g,2157568
-jijmodeling-1.0.0rc2.dist-info/RECORD,,
+jijmodeling/jijmodeling.cp39-win_amd64.pyd,sha256=t6HiyXzvhOOPXTNq590_f1ZcRjuhuWB4u1qeP4MWMhg,2172928
+jijmodeling-1.0.0rc3.dist-info/RECORD,,
```

