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
	def self.__init__(self, height, weight):
    		self.height = height
    		self.weight = weight
  	def self.move(self):
		pass
	def self.eat(self):
		pass
```

To hide information or restrict access to certain attributes or methods, is called **encapsulation**, 
and can be done by adding double underscore prefix ```__``` before a attribute or method

example:
```python:
class Example:
	def self.__init__(self, example):
		self.__example = example
	def self.get_example(self):
		return self.__example
```

here the ```example``` attribute is being encapsulated, and cannot be directly accessed by the user, though is still accessable using the ```get_example()``` method.

To create two methods of the same name but different parameters in the same class is called **overloading**.
To create two methods of the same name but one in the parent class and one in the child class is called **overriding**.
To create multiple methods of the same name in different classes that don't have inheritance, is called **polymorphism**.
Note that there is not overloading in python 3.
Overriding and polymorphism are both achieved by defining functions of the same name.

example:
```python:
# 1 and 2 is overriding, 2 and 3 is polymorphism
class Fruit:
	def self.speak(): #1
		print("I am a fruit")
class Orange(Fruit):
	def self.speak(): #2
		print("I am a Orange")
class Tomato:
	def self.speak(): #3
		print("I am a Tomato")
```
2 important base methods one can override are ```__str__``` and ```__repr__```
They both change the string representation of an object
if only ```__repr__``` is overriden it will be used for str(), print() and repr()
if only ```__str__``` is overriden it will be used for str(), print() and repr()
if both were overriden, str() and print() will use ```__str__``` and repr() will use ```__repr__```
it is good practice to define both as ```__str__``` represents a readable version while ```__repr__``` represents a unambiguous version

example:
```python:
class Pineapple:
	def __str__(self):
		return("pineapple")
	def __repr__(self):
		return("apple



