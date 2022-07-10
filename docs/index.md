# Welcome to pointers.py`s documentation!

## Bringing the hell of pointers to Python

-   [Repository](https://github.com/ZeroIntensity/pointers.py)
-   [PyPI](https://pypi.org/project/pointers.py)

### Example

```py
from pointers import to_ptr, Pointer, decay

a: str = '123'
b: str = 'abc'

@decay
def move(ptr_a: Pointer[str], ptr_b: Pointer[str]):
    ptr_a <<= ptr_b

move(a, b)
print(a, b) # abc abc
```

### Features

-   Fully type safe
-   Pythonic pointer API
-   Bindings for the entire C standard library
-   Segfaults

### Why does this exist?

The main purpose of pointers.py is to simply break the rules of Python, but has some other use cases:

-   Can help C/C++ developers get adjusted to Python
-   Provides a nice learning environment for programmers learning how pointers work
-   Makes it very easy to manipulate memory in Python
-   Why _not_?
