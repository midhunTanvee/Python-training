# Data Types

> Data Type represent the type of data present inside a variable.

*In Python we are not required to specify the type explicitly*.

Python Contains the following inbuilt data types:

 - int
 - float
 - complex
 - bool
 - str
 - bytes
 - bytearray
 - range
 - list
 - tuple
 - set
 - frozenset
 - dict
 - None

## int

We can use int data type to represent whole numbers (integral values)

```python
a = 10
print(type(a))
```

## float 

We can use float data type to represent floating point values(decimal values)

```python
a=10.9
b=9.01
c=9.0
d=100.00001
print(type(a), type(b), type(c), type(d))
```

## complex

A complex number is of the form `a+bj`. where `a` is real part and `b` is an imaginary part.

```python
a=3+5j
b=4+7j
c=8+9j
```

## bool

We can use this data type to represent boolean values.
The only allowed values are `True` and `False`.

## str

str represents string.

A string is a sequence of characters enclosed within single or double quotes.

```python
a='mithun'
b="narasimha"
c="ac123"
f='a_polk'
```

### Slicing of Strings:
slice means a piece.

`[]` operator is called slice operator.

In python strings have zero based index.

```python
name = "mithun"
print(name[1:3]) # it
print(name[0:4]) # mith
```

## bytes

bytes data type represents a group of byte numbers just like an array.

```python
x = [10,20,30]
print(x[0]) # 10
x[0] = 100 # Not allowed in bytes data type.
```
**Note**:

- The only allowed values for byte data type are `0` to `256`.
- We cannot change its values once it is declared.

## bytearray

bytearray is exactly same as bytes data type except that its elements can be changed.

```python
x = [10,20,30]
print(x[0]) # 10
x[0] = 100 # Allowed in bytearray data type.
```

## list

If we want to represent a group of values as a single entity where insertion order required to preserve and duplicates are allowed then we should go for list data type.

1. Insertion order is preserved
2. heterogeneous objects are allowed.
3. duplicates are allowed.
4. Growable in nature
5. values should be enclosed in square brackets.

```python
a = [10,20,30,40]
b = [10, "20", True, 10.23]
c = [1,1,2,3,3]
c.append(5)
print(c) # [1,1,2,3,3,5]
```

## tuple

tuple is exactly same as list data type except that it is immutable(which cannot be changed).

1. Insertion order is preserved
2. heterogeneous objects are allowed.
3. duplicates are allowed.
4. values should be enclosed within parenthesis `()`.

```python
a=(1,2,3,4)
b=(1, "as", "lk")
```

## set 

If we want to represent without duplicates where order is no important then we should go for set data type.

1. Insertion order is not preserved.
2. duplicates are not allowed.
3. heterogeneous objects are allowed
4. index concept is not applicable.
5. Growable in nature.

```python
s= {1,2,3,4,5}
s.add(45)
print(s) # {1,2,3,4,5,45}
```

## frozenset

it is exactly same as `set` data type except it is immutable..

1. Insertion order is preserved
2. heterogeneous objects are allowed.
3. duplicates are allowed.
4. values should be enclosed in square brackets.


```python
s= {1,2,3,4,5}
fs = frozenset(s)
```

## dict

If we want to represent a group of values as key-value pairs then we should go for dict data type.

```python
d = {"name":"mithun", "class":"IV", "Section":"E"}
print(d.keys()) # name, class, section
print(d.values()) # mithun, IV, E
```
