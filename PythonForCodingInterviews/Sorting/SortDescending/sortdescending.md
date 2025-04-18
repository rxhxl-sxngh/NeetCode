# Sort Descending

Solved

**The** `.sort()` method also accepts some optional parameters. This is the `.sort()` function signature:

```python
def sort(key=None, reverse=False) -> None:
```

1. **The** `key` parameter allows us to customize the sorting order. We will learn more about this soon.
2. **The** `reverse` parameter is a boolean value that determines whether the list should be sorted in *descending order*. By default, it is set to `False`.

**If we want to sort a list in descending order, we can set the** `reverse` parameter to `True`.

```python
elements = [5, 3, 6, 2, 1]

elements.sort(key=None, reverse=True)

print(elements) # [6, 5, 3, 2, 1]
```

**We can actually omit the** `key` parameter and only pass the `reverse` parameter, by using a feature of Python called *keyword arguments*.

```python
elements.sort(reverse=True)
```

**It's also possible for us to sort the list in ascending order and then manually reverse the result.**

```python
elements = [5, 3, 6, 2, 1]

elements.sort()

elements.reverse()
```

## Challenge

**Implement the following functions:**

1. `sort_words(words: List[str]) -> List[str]` - This function accepts a list of words and returns the list of words sorted in *descending order*.
2. `sort_numbers(numbers: List[int]) -> List[int]` - This function accepts a list of numbers and returns the list of numbers sorted in *descending order*.
3. `sort_decimals(numbers: List[float]) -> List[float]` - This function accepts a list of decimal numbers and returns the list of decimal numbers sorted in *descending order*.