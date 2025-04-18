# Unpacking

Solved

**The biggest advantage of using Python for coding interviews is its simplicity and readability. In this section we will learn some of the shortcuts Python provides to make our code easy to read and write.**

**One of these shortcuts is unpacking.**

```python
point1 = [0, 0]
point2 = [2, 4]

x1, y1 = point1 # x1 = 0, y1 = 0
x2, y2 = point2 # x2 = 2, y2 = 4

slope = (y2 - y1) / (x2 - x1)

print(slope) # Output: 2.0
```

1. **Above, we have code that calulates the slope of a line given two points.**
2. **Each point is a list of two integers.**
3. **Notice how we have two variables on the left side of the assignment operator, with a list on the right side. This is called unpacking. We know** `point1` and `point2` are lists of size `2`, so we can unpack them into two variables each.

**The below code accomplishes the same without unpacking but with slightly more code:**

```python
x1, y1 = point1[0], point1[1]
x2, y2 = point2[0], point2[1]
```

**If we attempt unpacking with not enough variables on the left-side, we will get a** `ValueError`.

```python
x, y = [0, 0, 0] # ValueError: too many values to unpack (expected 2)
```

**Unpacking also works with tuples and sets with the same syntax.**

## Challenge

**Implement the following functions using unpacking:**

1. `sum_3_integers(triplet: List[int]) -> int` that takes a list of 3 integers and returns the sum of the integers.
2. `compute_volume(box_dimensions: Tuple[int, int, int]) -> int` that takes a list of 3 integers representing `[width, height, depth]` of a box and returns the volume of it.

*That's it?*

You may think that these small shortcuts don't make a difference. But after you master the arts of Pythonic code, you will be able to save several lines of code as opposed to a more verbose language.

**For example, a 30 line function in Java may only be 15 lines in Python.**