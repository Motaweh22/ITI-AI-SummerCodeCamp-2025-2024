
---

# Advanced NumPy

Welcome to the advanced notebook in NumPy! If you have comments or suggestions, please don’t hesitate to share them at the end of the session!

![NumPy Logo](S1-pics/NumPy_logo.png)

```python
import numpy as np
```

-----

## Section 1: Broadcasting
Broadcasting allows NumPy to perform operations on arrays of different shapes.

### Rules of Broadcasting

1. **Dimension Padding**: If two arrays differ in dimensions, the shape of the smaller array is padded with ones on the left.
2. **Stretching**: If dimensions do not match, the array with shape equal to 1 in that dimension is stretched to match the other shape.
3. **Error Handling**: If sizes disagree and neither is 1, an error is raised.

---

### Example 1: Adding Arrays

```python
M = np.ones((2, 3))
a = np.arange(3)

# M.shape = (2, 3), a.shape = (3,)
M + a  # Broadcasting happens here
```

### Example 2: Both Arrays Broadcast

```python
a = np.arange(3).reshape((3, 1))
b = np.arange(3)

# Shapes: a.shape = (3, 1), b.shape = (3,)
a + b  # Broadcasting happens here
```

### Example 3: Incompatible Shapes

```python
M = np.ones((3, 2))
a = np.arange(3).reshape((3, 1))

# Attempting to add these will raise an error
# Correct approach
result = M + a  # Broadcasting will work because shapes are compatible
print(result)
```

### Note
Broadcasting rules apply to any binary ufunc, such as `np.logaddexp`.

---

## Section 2: Useful Array Operations

NumPy provides aggregation functions like `max`, `min`, `sum`, `mean`, `prod`, and `std`.

```python
data = np.array([1.0, 2.0, 3.0])
print(data.max())  # Maximum value
print(data.min())  # Minimum value
print(data.sum())  # Sum of elements
```

### Example: Aggregating a 2D Array

```python
a = np.array([[0.45, 0.17, 0.34, 0.55],
              [0.54, 0.05, 0.40, 0.56],
              [0.12, 0.82, 0.26, 0.56]])

# Sum of all elements
sum_all = a.sum()
print("Sum of all elements:", sum_all)

# Minimum value within each column
min_per_column = a.min(axis=0)
print("Minimum value in each column:", min_per_column)
```

---

## Section 3: Creating Matrices

Create a 2-D array using Python lists.

```python
data = np.array([[1, 2], [3, 4], [5, 6]])

# Indexing and Slicing Examples
first_in_second_col = data[0, 1]
elements_from_2nd_row = data[1:]
first_and_second_in_first_row = data[0, :2]
```

### Aggregating Matrices

```python
max_value = data.max()
min_value = data.min()
sum_value = data.sum()
print("Max value:", max_value)
print("Min value:", min_value)
print("Sum of all elements:", sum_value)

# Max across rows and columns
max_across_rows = data.max(axis=1)
max_across_columns = data.max(axis=0)
print("Max across rows:", max_across_rows)
print("Max across columns:", max_across_columns)
```

### Adding Matrices

```python
data = np.array([[1, 2], [3, 4]])
ones = np.array([[1, 1], [1, 1]])
result = data + ones  # Element-wise addition
```

---

## Section 4: Generating Random Numbers

NumPy offers functions like `ones()`, `zeros()`, and `random.Generator` for creating arrays of specified dimensions.

```python
# Generating 1D arrays
np.ones(3)
np.zeros(3)
rng = np.random.default_rng(0)
rng.random(3)

# Generating 2D arrays
np.ones((3, 2))
np.zeros((3, 2))
rng.random((3, 2))
```

---
