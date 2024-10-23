
---

# NumPy Basics

Welcome to the beginner’s guide to NumPy! This document will help you get started with NumPy, a powerful library for numerical computing in Python.

![NumPy Logo](S1-pics/NumPy_logo.png)

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Importing NumPy](#importing-numpy)
4. [About Arrays](#about-arrays)
5. [Creating Arrays](#creating-arrays)
6. [Array Operations](#array-operations)
7. [Array Attributes](#array-attributes)
8. [Reshaping Arrays](#reshaping-arrays)
9. [Increasing Dimensions](#increasing-dimensions)
10. [Conclusions](#conclusions)

## Introduction

NumPy is an open-source library for the Python programming language that provides support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays. 

## Installation

To install NumPy, you can use pip. Open your terminal or command prompt and run the following command:

```bash
pip install numpy
```

## Importing NumPy

Before using NumPy in your code, you need to import it. The convention is to import it as `np` to keep your code concise:

```python
import numpy as np
```

## About Arrays

An **array** is a central data structure of the NumPy library. It is a grid of values that can be indexed in various ways, and all elements in an array are of the same type, referred to as the array `dtype`.

### Example of Arrays

**1-D Array:**

```python
a = np.array([1, 2, 3, 4, 5, 6])
```

**2-D Array:**

```python
a = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]])
```

### Accessing Array Elements

You can access elements in the array using square brackets `[]`. Remember that indexing in NumPy starts at `0`.

```python
element = a[0]
```

## Creating Arrays

This section covers several ways to create NumPy arrays, including:

### Basic Array

```python
a = np.array([1, 2, 3])
```

### Array of Zeros

Create an array filled with `0`s:

```python
z = np.zeros((4, 3))
```

### Array filled with 1’s

Create an array filled with `1`s:

```python
s = np.ones(2)
```

### Empty Array

Create an array whose initial content is random:

```python
e = np.empty(3)
```

### Array within Range

You can create an array with a range of elements:

```python
r = np.arange(4)
i = np.arange(2, 10, 2)
```

### Specifying Data Type

Specify the data type of the array elements:

```python
x = np.ones(2, dtype=np.float64)
```

## Array Operations

### Sorting Arrays

You can sort an array with:

```python
arr = np.array([2, 1, 5, 3, 7, 4, 6, 8])
sorted_arr = np.sort(arr)
```

### Concatenating Arrays

To concatenate two arrays:

```python
a = np.array([1, 2, 3, 4])
b = np.array([5, 6, 7, 8])
concatenated = np.concatenate((a, b))
```

## Array Attributes

You can learn about the properties of an array using its attributes:

- **Number of Dimensions:** `ndarray.ndim`
- **Total Number of Elements:** `ndarray.size`
- **Shape of the Array:** `ndarray.shape`

### Example

```python
array_example = np.array([[[0, 1, 2, 3], [4, 5, 6, 7]], [[0, 1, 2, 3], [4, 5, 6, 7]], [[0, 1, 2, 3], [4, 5, 6, 7]]])
dimensions = array_example.ndim
total_elements = array_example.size
shape = array_example.shape
```

## Reshaping Arrays

You can reshape an array without changing the data:

```python
a = np.arange(6)
b = a.reshape(3, 2)
```

## Increasing Dimensions

To increase the dimensions of your existing array, you can use `np.newaxis` or `np.expand_dims`:

```python
a = np.array([1, 2, 3, 4, 5, 6])
a2 = a[np.newaxis, :]  # Converts to a 2D array
```

## Conclusions

This guide has provided you with the basics of using NumPy, covering how to create and manipulate arrays, sort them, and understand their properties. For more in-depth knowledge, refer to the official [NumPy documentation](https://numpy.org/doc/stable/).

Feel free to reach out with comments or suggestions!

--- 
