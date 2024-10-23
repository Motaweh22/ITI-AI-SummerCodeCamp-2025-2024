
---

# Intro to Python Day 01 Lab

Compiled by Ali Heikal

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Problems](#problems)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project consists of a collection of Python programs that cover basic programming concepts and operations. Each problem provides a practical exercise designed to help beginners understand Python syntax, data types, and control structures. 

## Installation

To run the code, ensure you have Python installed on your system. You can download Python from [python.org](https://www.python.org/downloads/).

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/python-lab.git
   ```
2. Navigate to the project directory:
   ```bash
   cd python-lab
   ```
3. Run the script:
   ```bash
   python lab.py
   ```

You can also run individual problems in your Python interpreter or IDE.

## Problems

The project includes the following problems:

1. **Hello, World!**: Prints "Hello, World!"
   ```python
   print("Hello, World!")
   ```

2. **Date and Time**: Prints the current date and time.
   ```python
   from datetime import datetime
   print("Current date and time:", datetime.now())
   ```

3. **Python Version**: Prints the Python version and environment info.
   ```python
   import sys
   print("Python Version:", sys.version)
   print("Python Environment Info:", sys.version_info)
   ```

4. **Name Reversal**: Accepts first and last names and prints them in reverse order.
   ```python
   first_name = input("Enter your first name: ")
   last_name = input("Enter your last name: ")
   print(f"{last_name} {first_name}")
   ```

5. **Word Reversal**: Accepts a word and prints it in reverse order.
   ```python
   word = input("Enter a word: ")
   print(word[::-1])
   ```

6. **Value Parsing**: Parses a value to both float and integer.
   ```python
   value = input("Enter a number: ")
   float_value = float(value)
   int_value = int(float_value)
   print("Float:", float_value)
   print("Integer:", int_value)
   ```

7. **Even or Odd**: Accepts an integer and checks if it's even or odd.
   ```python
   n = int(input("Enter an integer: "))
   if n % 2 == 0:
       print("The number is even.")
   else:
       print("The number is odd.")
   ```

8. **N + NN + NNN**: Computes the value of n + nn + nnn.
   ```python
   n = input("Enter an integer (n): ")
   result = int(n) + int(n*2) + int(n*3)
   print("Result:", result)
   ```

9. **Print Hello, World! Thrice**: Prints "Hello, World!" three times without loops.
   ```python
   print("Hello, World!\n" * 3)
   ```

10. **String Operations**: Checks the length of a string and the existence of a word in it.
    ```python
    string = input("Enter a string: ")
    word = input("Enter a word to check: ")
    print("Length of the string:", len(string))
    if word in string:
        print(f"The word '{word}' exists in the string.")
    else:
        print(f"The word '{word}' does not exist in the string.")
    ```

11. **First and Last Characters**: Prints the first two and last two characters of a string.
    ```python
    string = input("Enter a string: ")
    if len(string) < 2:
        print("Empty string")
    else:
        print("Result:", string[:2] + string[-2:])
    ```

12. **Concatenate Lists**: Concatenates two lists index-wise.
    ```python
    list1 = ['a', 'b', 'c']
    list2 = [1, 2, 3]
    result = [str(list1[i]) + str(list2[i]) for i in range(len(list1))]
    print("Concatenated List:", result)
    ```

13. **Square List Items**: Squares every item in a list.
    ```python
    numbers = [1, 2, 3, 4]
    squared_numbers = [x**2 for x in numbers]
    print("Squared List:", squared_numbers)
    ```

14. **Remove Empty Strings**: Removes empty strings from a list of strings.
    ```python
    strings = ["hello", "", "world", "", "python"]
    filtered_strings = [string for string in strings if string]
    print("Filtered List:", filtered_strings)
    ```

15. **Reverse Tuple**: Reverses a tuple.
    ```python
    t = (1, 2, 3, 4)
    reversed_tuple = t[::-1]
    print("Reversed Tuple:", reversed_tuple)
    ```

16. **Tuple to Variables**: Converts a tuple to individual variables.
    ```python
    t = (1, 2, 3)
    a, b, c = t
    print(a, b, c)
    ```

17. **Count Occurrences**: Counts occurrences of an item in a list.
    ```python
    items = [1, 2, 2, 3, 3, 3]
    count = items.count(2)
    print("Count of 2:", count)
    ```

18. **Similar Items in Sets**: Detects similar items between two sets.
    ```python
    set1 = {1, 2, 3}
    set2 = {2, 3, 4}
    similar_items = set1 & set2
    print("Similar items:", similar_items)
    ```

19. **Combine Sets**: Combines two sets while removing duplicates.
    ```python
    set1 = {1, 2, 3}
    set2 = {3, 4, 5}
    combined_set = set1 | set2
    print("Combined Set:", combined_set)
    ```

20. **Remove Similar Values in Sets**: Removes values in one set similar to another.
    ```python
    set1 = {1, 2, 3}
    set2 = {2, 3, 4}
    set1.difference_update(set2)
    print("Set after removing similar values:", set1)
    ```

21. **Convert Lists to Dictionary**: Converts two lists to a dictionary.
    ```python
    keys = ['a', 'b', 'c']
    values = [1, 2, 3]
    dictionary = dict(zip(keys, values))
    print("Dictionary:", dictionary)
    ```

22. **Extract Specific Keys from Dictionary**: Creates a new dictionary from specific keys.
    ```python
    original_dict = {'a': 1, 'b': 2, 'c': 3}
    keys_to_extract = ['a', 'c']
    new_dict = {k: original_dict[k] for k in keys_to_extract}
    print("New Dictionary:", new_dict)
    ```

23. **Remove Keys from Dictionary**: Removes keys from a given dictionary.
    ```python
    dictionary = {'a': 1, 'b': 2, 'c': 3}
    del dictionary['a']
    del dictionary['b']
    print("Updated Dictionary:", dictionary)
    ```

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`
3. Commit your changes: `git commit -m 'Add new feature'`
4. Push the branch: `git push origin feature-branch-name`
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

