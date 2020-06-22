#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a)
O(n), Linear time - The first line contains a while loop which goes on for n _ n _ n times. O(n3). But the iterator in the loop counts n \* n times, so it negates it and becomes O(n)

b)
O(nlogn), Linear time - The first for loop goes on for n times. Inside the loop, the next line is an O(1). However, it has a nested while loop which goes on for O(log(n)) times as well. Therefore, n \* O(logn) = O(nlogn).

c)
O(n), Linear time. The pseudocode contains an assignment which is O(1). It also contains a recursive call which will go on until the size of the input decreases to 0. Therefore it is O(n).

## Exercise II

1. We know that an egg will break only if it is thrown off a floor higher than f. Therefore, to minimise the number of eggs wasted, we will start throwing from the middle of the building. We find the middle floor by finding the highest and lowest floors, adding them up and dividing by 2,

2. If an egg breaks when we throw it from the middle, we set the highest floor to the floor underneath the middle floor. If it doesnt break, we set the lowest floor to the floor above the middle floor.

3. We repeat steps 1 and 2 again, and eventually we will be narrowing down the location of floor f.

4. The runtime complexity will be O(logn), as the amount of tasks to be done will be decrease regardless of the number of inputs.
