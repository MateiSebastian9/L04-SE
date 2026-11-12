# Bug reports for exercise2.py

Line: 3
Problem: is_passing returns False for a grade of exactly 5, but the docstring says "5 or more".
Example: is_passing(5) returns False, expected True.
Fix: return grade >= 5

Line: 8
Problem: is_valid_password requires at least 8 characters but uses > 8, so it fails for passwords of exactly 8 characters, which violates "at least 8".
Example: is_valid_password("abcdefgh") returns False, expected True.
Fix: return len(password) >= 8 and any(c.isdigit() for c in password)

Line: 13
Problem: clamp uses max(low, min(x, low)) which simplifies to low, so it always returns low, not the correct clamping to [low, high].
Example: clamp(10, 5, 15) returns 5, expected 10.
Fix: return max(low, min(x, high))
