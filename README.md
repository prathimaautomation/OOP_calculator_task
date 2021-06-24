# Functional Calculator
- Timings
- 30 - 60 Minutes

## Summary
### Amazing you now know functions, lets make a functional calculator.

### Tasks
#### Complete the core tasks
```python

Create a class called Calculator
functions
practice using, defining and calling functions
Build a basic functional
Core 1: build function containing
# add,
# subtract,
# multiply,
# divide.
Create a file for child class called Functional_calculator
import calculator class and inherit all the functionality
Core 2: Build more functions for
# area of a circle
# area of a square
# area of a triangle (just find the easiest way)
```
```python
# Create a class called Calculator
# functions
# practice using, defining and calling functions
# Build a basic functional
class Calculator:

# Core 1: build function containing
     # add
     def add(self, num1, num2):
         return num1 + num2

     # subtract
     def subtract(self, num1, num2):
         return num1 - num2

     # multiply
     def multiply(self, num1, num2):
         return num1 * num2

     # divide
     def divide(self, num1, num2):
         return num1 / num2

```
```python
# Create a file for child class called Functional_calculator
# import calculator class and inherit all the functionality
from calculator import Calculator
import math

class Functional_calculator(Calculator):
        def __init__(self):
            super().__init__()

        # Core 2: Build more functions for
        # area of a circle
        def area_of_a_circle(self, radius):
            return  3.14 * self.multiply(radius, radius)

        # area of a square
        def area_of_a_square(self, side):
            return self.multiply(side, side)

        # area of a triangle (just find the easiest way)
        def area_of_a_triangle(self, base, height):
            return 0.5 * self.multiply(base, height)

function_calc = Functional_calculator()
operation = input("Which area would like to find out?\nCircle, Square, Triangle? ")

if operation.strip().lower() == "circle":
    radius =int(input("What is radius of the circle? "))
    print(function_calc.area_of_a_circle(radius))
elif operation.strip().lower() == "square":
    side = int(input("What is the length of side? "))
    print(function_calc.area_of_a_square(side, side))
elif operation.strip().lower() == "triangle":
    base = int(input("What is the base of triangle? "))
    height = int(input("What is the height of triangle? "))
    print(function_calc.area_of_a_triangle(base, height))

```