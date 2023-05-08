# Session 9 Tasks
## Task 1
for the following code
```python
class A:
    x = 1

class B:
    x = 2

class C:
    x = 3

class D(A, B, C):
    pass

ob = D()
ob.x
```
it will print `1`.

How to make it print 2 (from `B`), or 3 (from `C`)
### Solution
```python
class A:
    x = 1

class B:
    x = 2

class C:
    x = 3

class D(A, B, C):
    def print_x(self):
        print(super(A, self).x)   # Output: 2

ob = D()
ob.print_x()
```

When you call `super(A, self).x`, It returns the` x` attribute of the next class in the method resolution order (MRO) after `A`, which is `B`. Since `B` defines an x attribute with a value of 2, this is the value that gets printed.

The MRO is determined at runtime by a depth-first search of the inheritance tree, following the order in which the classes are listed in the parentheses when defining the subclass. In this case, since `A` is listed first, followed by `B` and then `C`, the MRO of `D` is `[D, A, B, C, object]`.

Therefore, when `super(A, self)` is called, it returns a temporary object representing the next class in the MRO after `A`, which is `B`. The `x` attribute of this object is then accessed and printed, resulting in the output 2.

More information could be found [here](https://stackoverflow.com/questions/3277367/how-does-pythons-super-work-with-multiple-inheritance).