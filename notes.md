# Object Oriented Programming Notes 1

**Object Oriented Programing is simulating logic in reality:**

For example, as a human,
we have **attributes** like weight, height, gender, hair color,
we have **methods** like eat, move, play, think
and we are all **objects** of a human **class**.

Conceptual Differentiation between Precedure-Oriented and Object-Oriented
**"OOP focuses on how to manipulate the data of the object rather than the logic required to manipulate them"**

Definition of an **object**: An identifier of a location of memory that contains a value,
or an instance of a class. It is a combination of data(fields) and functional code(methods). An object is an instance.

Definition of a **class**: An abstract description of all objects that can be made from this set class where an object can be instantiated from. Classes have attributes which devide into Fields and Methods

To define a class, use the ```class``` keyword
Code inside classes should be indented
To initialize Attributes, use the ```__init__()``` method

example:
```python:
#height and weight are fields, move() and eat() are methods
class Human:
	def __init__(self, height, weight):
    		self.height = height
    		self.weight = weight
  	def move():
		pass
	def eat():
		pass
```

To hide information or restrict access to certain attributes or methods, is called **encapsulation**, 
and can be done by adding double underscore prefix ```__``` before a attribute or method

example:
```python:
class Example:
	def __init__(example):
		self.__example = example
	def get_example():
		return self.__example
```

here the ```example``` attribute is being encapsulated, and cannot be directly accessed by the user, though is still accessable using the ```get_example()``` method.

To create two methods of the same name but different parameters in the same class is called **overloading**.
To create two methods of the same name but one in the parent class and one in the child class is called **overriding**.
To create multiple methods of the same name in different classes that don't have inheritance, is called **polymorphism**.
Note that there is not overloading in python 3.
Overriding and polymorphism are both achieved by defining functions of the same name.

example:





