# Loop Unpacking

Solved

**We can also use unpacking in loops to iterate over a list of lists. This is useful when we know the size of the inner lists and want to unpack them into variables.**

```python
points = [[0, 0], [2, 4], [3, 6], [5, 10]]

for x, y in points:
    print(f"x: {x}, y: {y}")
```

**We could accomplish this without packing with slightly more code:**

```python
for point in points:
    x, y = point[0], point[1]
    print(f"x: {x}, y: {y}")
```

**You can see we saved a line of code by using unpacking.**

## Challenge

**Implement the following function using unpacking:**
* `best_student(scores: List[Tuple[str, int]]) -> str:` that takes a list of tuples. Each tuple represents the `(name, score)` of a student. Find the student with the highest score and return their `name`.

**You may assume that a** `score` w