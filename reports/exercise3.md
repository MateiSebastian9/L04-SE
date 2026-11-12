# Bug reports for exercise3.py

Line: 3
Problem: average divides by len(numbers), which crashes on an empty list, but the docstring says an empty list has average 0.
Example: average([]) raises ZeroDivisionError, expected 0.
Fix: return sum(numbers) / len(numbers) if numbers else 0

Line: 8
Problem: first_word crashes on an empty text, but the docstring says it returns "" if the text is empty.
Example: first_word("") raises IndexError, expected "".
Fix: return text.split()[0] if text.strip() else ""

Line: 12
Problem: percent divides by total, which crashes on total = 0, but the docstring says the result is 0 if total is 0.
Example: percent(5, 0) raises ZeroDivisionError, expected 0.
Fix: return part / total * 100 if total != 0 else 0
