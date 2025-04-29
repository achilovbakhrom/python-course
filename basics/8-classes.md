class keyword for using class

class Rectangle:
    def __init__(self, width, height):
        self.width = width
        self.height = height
    
    @property # getter
    def width(self):
        return self._width

    @width.setter # setter
    def width(self, width):
        if width <= 0:
            raise ValueError('Width must be positive')
        else:
            self.width = width

    @height.setter # setter
    def height(self, height):
        if height <= 0:
            raise ValueError('Height must be positive')
        else:
            self.height = height

    @property
    def height(self): # getter
        return self._height


    
    def area(self):
        return self.width * self.height
    
    def perimeter(self):
        return 2 * (self.width + self.height)
    
    def to_string(self): # this works only for Java
        return "Rectangle: width={0}, height={1}".format(self.width, self.height)
    
    def __str__(self):
        return "Rectangle: width={0}, height={1}".format(self.width, self.height)
    
    def __repr__(self):
        return "Rectangle({0}, {1})".format(self.width, self.height)

    def __eq__(self, other):
        if  isinstance(other, Rectangle):
            return self.width == other.width and self.height == other.height
        else:
            return False
    
    
    

__init__ - method is constructor

ri = Rectangle(10, 20)
ri.width = 100

ri.area()
ri.perimeter()

hex(id(ri)) - shows address of ri in hexidecimal format

print(ri)

__ - donder (double underscore)

__str__ - will be called when object will be converted to string
__repr__ - usually shows how can we rebuild the object

r1 == r2 - compares using __eq__
r1 is r2 - compares addresses (something like === in js)

__lt__ - less than
__lte__ - less than or equal
__gt__ - greater than
__gte__ - greater than or equal
