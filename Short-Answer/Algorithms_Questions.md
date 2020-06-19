# Analysis of Algorithms

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```

```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

1. We know that an egg will break only if it is thrown off a floor higher than f. Therefore, to minimise the number of eggs wasted, we will start throwing from the middle of the building. We find the middle floor by finding the highest and lowest floors, adding them up and dividing by 2,

2. If an egg breaks when we throw it from the middle, we set the highest floor to the floor underneath the middle floor. If it doesnt break, we set the lowest floor to the floor above the middle floor.

3. We repeat steps 1 and 2 again, and eventually we will be narrowing down the location of floor f.

4. The runtime complexity will be O(logn), as the amount of tasks to be done will be decrease regardless of the number of inputs.
