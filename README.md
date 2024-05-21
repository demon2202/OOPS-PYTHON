# Object-Oriented Programming in Python

Object-oriented programming (OOP) is a method of structuring a program by bundling related properties and behaviors into individual objects. In this tutorial, you'll learn the basics of object-oriented programming in Python with an example of vehicles.

## Table of Contents

- What Is Object-Oriented Programming in Python?
- What Is a Class in Python?
- How Do You Define a Class in Python?
- How Do You Instantiate a Class in Python?
- What Are Class and Instance Attributes?
- What Is an Instance Method?
- How Do You Inherit From Another Class in Python?
- Example: Vehicles and Subclasses
- What Are Parent Classes and Child Classes?
- What Is Method Overriding?
- Conclusion
- Exercise: Create a Bicycle Class

---

## What Is Object-Oriented Programming in Python?

Object-oriented programming (OOP) is a method of structuring a program by bundling related properties and behaviors into individual objects. In this tutorial, you’ll learn the basics of object-oriented programming in Python with an example of vehicles.

### Questions:

- What are the main principles of object-oriented programming?
- How does OOP differ from procedural programming?

---

## What Is a Class in Python?

In Python, a class is like a blueprint for creating an object. A class defines attributes (variables) and methods (functions) that the object will have.

### Questions:

- What is a class attribute?
- What is an instance attribute?

---

## How Do You Define a Class in Python?

Here's an example of a `Vehicle` class:

```python
class Vehicle:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year

    def description(self):
        return f"{self.year} {self.make} {self.model}"
```

### Questions:

- What does the `__init__()` method do in a class?
- Can you give an example of a class attribute and an instance attribute?

---

## How Do You Instantiate a Class in Python?

To create an object from a class, you use the class name followed by parentheses. Here's how you can create a `Vehicle` object:

```python
car = Vehicle("Toyota", "Camry", 2020)
```

---

## What Are Class and Instance Attributes?

Attributes can belong to the class itself or to instances of the class. Class attributes are shared by all instances, while instance attributes are unique to each instance.

### Questions:

- What is the difference between class and instance attributes?
- How do you access class and instance attributes?

---

## What Is an Instance Method?

Instance methods are functions that belong to instances of a class. They can access and modify instance attributes.

### Questions:

- What is an instance method?
- How do you define and call an instance method?

---

## How Do You Inherit From Another Class in Python?

Inheritance allows you to create a new class based on an existing class. The new class inherits attributes and methods from the existing class.

### Questions:

- What is inheritance?
- How do you define a subclass?

---

## Example: Vehicles and Subclasses

Let's create subclasses for different types of vehicles, such as cars, trucks, and motorcycles.

```python
class Car(Vehicle):
    def drive(self):
        return "Driving a car"

class Truck(Vehicle):
    def load(self):
        return "Loading cargo"

class Motorcycle(Vehicle):
    def ride(self):
        return "Riding a motorcycle"
```

### Questions:

- What does the `drive()` method do in the `Car` class?
- How would you override the `description()` method in the `Car` class to include the type "Car"?

---

## What Are Parent Classes and Child Classes?

Inheritance introduces the concepts of parent classes (superclasses) and child classes (subclasses). A child class inherits attributes and methods from its parent class.

### Questions:

- What is a parent class?
- What is a child class?

---

## What Is Method Overriding?

Child classes can override methods defined in the parent class to provide specialized behavior.

### Questions:

- What is method overriding?
- How do you override a method in a child class?

---

## Conclusion

Object-oriented programming in Python allows you to create organized, reusable code by using classes and objects. Inheritance and method overriding are powerful features that enable you to create specialized classes based on existing ones.

---

## Exercise: Create a Bicycle Class

Try creating a `Bicycle` class that inherits from `Vehicle` and adds a `ride()` method. Then instantiate a `Bicycle` object and call its `description()` and `ride()` methods.

### Questions:

- What output do you expect when you call the `description()` and `ride()` methods on a `Bicycle` object?

---

I hope this README.md file helps you understand object-oriented programming in Python better! Feel free to try out the exercise and let me know if you have any questions or suggestions.
