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
<img width="446" height="268" alt="image" src="https://github.com/user-attachments/assets/ea8051fa-94ec-45ab-a9b7-0f3f27080b48" />

## Result
Thus the program to demonstrate polymorphism using Beans and Mango classes has been executed successfully. The type and color of each object are displayed using a generic function.

