# Enumerate

Solved

**Suppose we wanted to loop over an array and we needed to access both the index and the element at that index. This is simple to accomplish:**

```python
nums = [2, 7, 9, 2]

for i in range(len(nums)):
    n = nums[i]
    print(i, n)
```

**But the Pythonic way to do this is to use the** `enumerate()` function:

```python
nums = [2, 7, 9, 2]

for i, n in enumerate(nums):
    print(i, n)
```

**The** `enumerate()` function returns a tuple of the index and the element at that index. We can unpack this tuple into two variables in the for loop.

**The main benefit of this approach is the readability improvement, especially if we use good variable names. This allows us to easily write self-documenting code, just like when we use** `for in` loops as shown below.

```python
names = ['Alice', 'Bob', 'Charlie']

# This is more readable than using range()
for name in names:
    print(name)


# This is more readable than using range() 
# and still allows us to access the index 
# of each element
for i, name in enumerate(names):
    print(i, name)
```

## Challenge

**Implement the following functions using** `enumerate()`:

1. `get_index_of_seven(nums: List[int]) -> int` that returns the index of the first occurrence of the number `7` in the list `nums`, or `-1` if `7` is not found.
2. `get_dist_between_sevens(nums: List[int]) -> int` that returns the distance between the first and second occurrence of the number `7` in the list `nums`.
   * You may assume that there will *always be at least two* occurrences of the number `7` in the list.