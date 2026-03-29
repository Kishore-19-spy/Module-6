# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC,abstractmethod
class Shape(ABC):
 def __init__(self):
  pass
 @abstractmethod
 def calculate_area(self):
  pass
class Rectangle(Shape):
 def __init__(self,l=5,b=3):
  self.l=l
  self.b=b
 def calculate_area(self):
  return self.l*self.b
class Circle(Shape):
 def __init__(self,r=2):
  self.r=r
 def calculate_area(self):
  return 3.14*self.r*self.r
r=Rectangle()
c=Circle()
print(r.calculate_area())
print(c.calculate_area())
```
## Output
<img width="398" height="187" alt="image" src="https://github.com/user-attachments/assets/7daf8502-af24-4347-9830-e768b16cdbd9" />

## Result
Thus the program to create an abstract class Shape and implement area calculation in Rectangle and Circle has been executed successfully.
The areas for the given dimensions are displayed as output.

# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
 def __init__(self,l=5,b=3):
  self.__length=l
  self.__breadth=b
 def display(self):
  print(self.__length,self.__breadth)
r=Rectangle()
r.display()
```

## Output
<img width="386" height="160" alt="image" src="https://github.com/user-attachments/assets/bbf815a4-9a0f-4ff5-a0f9-0b4b22593094" />

## Result
Thus the program to implement encapsulation using private variables in a Rectangle class has been executed successfully.
The private member values are accessed and displayed using a class method.

# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```
class Fish:
 def type(self):
  print("fish")
class Shark(Fish):
 def type(self):
  print("shark")
obj_goldfish=Fish()
obj_hammerhead=Shark()
for i in (obj_goldfish,obj_hammerhead):
 i.type()
```

## OUTPUT
<img width="450" height="203" alt="image" src="https://github.com/user-attachments/assets/4acb8d47-9dee-44f4-9f61-52f014e205a6" />

## RESULT
Thus the program to demonstrate inheritance and method overriding using Fish and Shark classes has been executed successfully.
The output shows "fish" and "shark" as expected.

# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```
class A:
 def __init__(self,a):
  self.a=a
 def __lt__(self,o):
  if self.a<o.a:
   return "ob1 is less than ob2"
  else:
   return "ob2 is less than ob1"
ob1=A(5)
ob2=A(10)
print(ob1<ob2)
```
## Output
<img width="363" height="161" alt="image" src="https://github.com/user-attachments/assets/07561fed-cdf9-44f5-9a64-451c64241fd6" />

## Result
Thus the program to demonstrate operator overloading using the less than operator has been executed successfully.
The comparison result between the two objects is displayed as output.

# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```
class Beans:
 def type(self):
  print("Vegetable")
 def color(self):
  print("Green")
class Mango:
 def type(self):
  print("Fruit")
 def color(self):
  print("Yellow")
def func(obj):
 obj.type()
 obj.color()
b=Beans()
m=Mango()
func(b)
func(m)
```

## Output
<img width="446" height="268" alt="image" src="https://github.com/user-attachments/assets/d8718d1b-1556-4c58-971f-93fe8a605cae" />

## Result
Thus the program to demonstrate polymorphism using Beans and Mango classes has been executed successfully.
The type and color of each object are displayed using a generic function.

