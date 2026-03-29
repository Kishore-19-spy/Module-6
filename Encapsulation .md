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
<img width="386" height="160" alt="image" src="https://github.com/user-attachments/assets/13bd1379-0401-48f1-ad5c-9ae89558fb41" />

## Result
Thus the program to implement encapsulation using private variables in a Rectangle class has been executed successfully. The private member values are accessed and displayed using a class method.

