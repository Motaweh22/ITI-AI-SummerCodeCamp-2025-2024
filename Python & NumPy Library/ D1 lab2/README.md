

```markdown
# Intro to Python Day 02 Lab

Compiled by Ali Heikal

## Overview

This repository contains a collection of Python programs designed to practice basic programming concepts. The code covers various topics such as functions, data structures, classes, and file handling.

## Table of Contents

1. [Problem 1: Addition Function](#problem-1-addition-function)
2. [Problem 2: Sum of List Items](#problem-2-sum-of-list-items)
3. [Problem 3: Count Letters in String](#problem-3-count-letters-in-string)
4. [Problem 4: Print Details of Apes](#problem-4-print-details-of-apes)
5. [Problem 5: Songs Class](#problem-5-songs-class)
6. [Problem 6: Bus Class Inheritance](#problem-6-bus-class-inheritance)
7. [Problem 7: File Handling](#problem-7-file-handling)

## Problem 1: Addition Function

Write a program that implements a function of addition with two arguments that sums those arguments and returns their sum.

```python
def add(a, b):
    return a + b

# Example usage
result = add(5, 10)
print("Sum:", result)
```

## Problem 2: Sum of List Items

Write a program that sums all items in a list.

```python
numbers = [1, 2, 3, 4, 5]

# Sum all items in the list
total_sum = sum(numbers)
print("Sum of all items:", total_sum)
```

## Problem 3: Count Letters in String

Write a program that accepts a string and calculates the number of letters in the inputted string.

```python
string = input("Enter a string: ")

# Calculate the number of letters
num_letters = len(string)
print("Number of letters in the string:", num_letters)
```

## Problem 4: Print Details of Apes

Write a program to print details for each element in a given list of apes.

```python
apes = ["Homo sapiens", "Pan troglodytes", "Gorilla gorilla"]

for ape in apes:
    print(f"{ape} is an ape. Its name has {len(ape)} letters.")
```

## Problem 5: Songs Class

Define a class called `Songs` that shows the lyrics of a song.

```python
class Songs:
    def __init__(self, lyrics):
        self.lyrics = lyrics

    def sing_me_a_song(self):
        for line in self.lyrics:
            print(line)

# Example usage
song = Songs(["Happy birthday to you",
              "Happy birthday to you",
              "Happy birthday dear friend",
              "Happy birthday to you"])
song.sing_me_a_song()
```

## Problem 6: Bus Class Inheritance

Create a child class `Bus` that inherits from the class `Vehicle`.

```python
class Vehicle:
    def __init__(self, name, max_speed, mileage):
        self.name = name
        self.max_speed = max_speed
        self.mileage = mileage

    def vehicle_info(self):
        return f"Vehicle Name: {self.name}, Max Speed: {self.max_speed}, Mileage: {self.mileage}"

class Bus(Vehicle):
    pass

# Example usage
bus = Bus("School Bus", 120, 12)
print(bus.vehicle_info())
```

## Problem 7: File Handling

Create a text file and apply read, write, and append modes.

```python
# Write to a file
with open('example.txt', 'w') as file:
    file.write("This is a line written in write mode.\n")

# Append to the file
with open('example.txt', 'a') as file:
    file.write("This line is appended to the file.\n")

# Read the file
with open('example.txt', 'r') as file:
    content = file.read()

print("File content:\n", content)
```

## Usage

To run each program, simply copy the code snippet into a Python environment or script and execute it.

## Conclusion

This lab provides a hands-on approach to learning fundamental programming concepts in Python. Feel free to modify and expand the programs as you see fit.
```
