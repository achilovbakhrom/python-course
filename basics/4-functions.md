Function is:
    - Stand-alone blocks of code defined at the global or module level.
    - Do not have an implicit context or “owner” object.
    - Called by name, passing all required data explicitly as parameters.
Example:
```
def add(a, b):
    return a + b
```

Method is:
    - Functions that are associated with a specific type (in statically-typed languages) or class (in object-oriented languages).
    - Have an implicit “receiver” or this/self parameter giving access to the object’s internal state.
    - Invoked on an instance (or on the type itself, if it’s a static or class method).
    - Can modify or read the object’s properties.

Example:

```
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def move(self, dx, dy):
        self.x += dx
        self.y += dy
```

type(5) # returns int
type(5) == int # True

checking is function or not
```
import types

def func1():
  return 123

print(type(func1) == types.FunctionType) # True
print(type(lambda x: x**2) == types.FunctionType) # True
```