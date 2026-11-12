# Bug reports for exercise1.py

Line: 3
Problem: is_even returns True for odd numbers because it checks n % 2 == 1, but the docstring says "true for even numbers".
Example: is_even(4) returns False, expected True.
Fix: return n % 2 == 0

Line: 8
Problem: rectangle_area returns the sum of width and height instead of the product, but the docstring says "area of a rectangle".
Example: rectangle_area(4, 5) returns 9, expected 20.
Fix: return width * height

Line: 13
Problem: double adds 2 instead of multiplying by 2, but the docstring says "twice the number n".
Example: double(5) returns 7, expected 10.
Fix: return n * 2
