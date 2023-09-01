# List Comprehensions and Generator Expressions

# Introduction
Python provides powerful tools like list comprehensions and generator expressions to simplify complex tasks and make your code more concise. These features allow you to create lists and iterable objects with minimal code, enhancing code readability and efficiency.

# List Comprehensions

List comprehensions are a concise way to create lists by applying an operation to each item in an existing iterable and optionally filtering items based on a condition.

Syntax
python
Copy code
new_list = [optional_operation(item) for item in old_list if optional_condition == True]
Example 1: Creating a list of squares minus one:

python
Copy code
squared_minus_one = [(n ** 2) - 1 for n in range(1, 11)]
# Result: [0, 3, 8, 15, 24, 35, 48, 63, 80, 99]
Example 2: Filtering even numbers from a list:

python
Copy code
even_numbers = [x for x in num_list if x % 2 == 0]

# Generator Expressions

Generator expressions are similar to list comprehensions but create generator objects instead of lists. These objects are memory-efficient and ideal for processing large datasets.

Syntax
python
Copy code
generator_expression = (optional_operation(item) for item in old_list if optional_condition == True)
Example: Creating a generator for squares:

python
Copy code
squared_generator = (n ** 2 for n in range(1, 11))

# When to Use List Comprehensions vs. Generator Expressions

* List Comprehensions: Use when you need a complete list and want fast access to the data. Suitable for small to moderately sized datasets.

* Generator Expressions: Use when memory efficiency is crucial, especially for large datasets. Generators are lazy and only compute values as needed.

Practice
In the list_comprehension.py file, you can find practice exercises for creating lists using list comprehensions:

return_evens(): Returns a list of even elements from a sequence of integers.
Example:

python
Copy code
return_evens([0, 1, 3, 5, 7, 8, 9])  # Result: [0, 8]
make_exclamation(): Adds exclamation marks at the end of sentence strings in a list.
Example:

python
Copy code
make_exclamation(["Hello", "I'm doing great", "Python is fun"])
# Result: ["Hello!", "I'm doing great!", "Python is fun!"]
Ensure all tests pass using pytest -x before submitting your work.

Remember that list comprehensions and generator expressions can greatly improve your Python coding skills by simplifying complex operations and enhancing code readability.

When all of your tests are passing, submit your work using `git`.

***

## Resources

- [Python - List Comprehension](https://www.geeksforgeeks.org/python-list-comprehension/)
- [When to Use a List Comprehension in Python](https://realpython.com/list-comprehension-python/)
- [PEP 289 - Generator Expressions](https://peps.python.org/pep-0289/)
- [Python | Generator Expressions](https://www.geeksforgeeks.org/generator-expressions/)

## Resources

- [Python - List Comprehension](https://www.geeksforgeeks.org/python-list-comprehension/)
- [When to Use a List Comprehension in Python](https://realpython.com/list-comprehension-python/)
- [PEP 289 - Generator Expressions](https://peps.python.org/pep-0289/)
- [Python | Generator Expressions](https://www.geeksforgeeks.org/generator-expressions/)
