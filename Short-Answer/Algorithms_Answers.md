#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a)
O(n), Linear time - The first line contains a while loop which goes on for n _ n _ n times. O(n3). But the iterator in the loop counts n \* n times, so it negates it and becomes O(n)

b)
O(nlogn), Linear time - The first for loop goes on for n times. Inside the loop, the next line is an O(1). However, it has a nested while loop which goes on for O(log(n)) times as well. Therefore, n \* O(logn) = O(nlogn).

c)
O(n), Linear time. The pseudocode contains an assignment which is O(1). It also contains a recursive call which will go on until the size of the input decreases to 0. Therefore it is O(n).

## Exercise II
