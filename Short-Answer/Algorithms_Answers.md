#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)
-- just one loop; a increases at the same rate with each iteration

b) O(n log(n))
-- The outer loop increments linearly at the same rate -- O(n)
-- The inner loop doubles the index with each iteration -- O(log(n))
-- Therefore, because the loops are nested, we multiply them resulting in a time complexity of O(n log(n))

i
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19]
    j

5 = 3 for each = 15
10 = 4 for each = 40
20 = 5 for each = 100
40 = 6 for each = 240

c) O(n)
-- recursion, but increases at a rate of two with each input

## Exercise II

1. Find the middle floor of the building and drop an egg.  
 - If it breaks, we know that the value of f is either this floor or a floor below (thus we can eliminate all the floors above).
 - If it doesn't break, we know that the value of f is higher than this floor (thus we can eliminate all the floors below).

2. We'll continue the process described in step 1 (eliminating half the floors) until we find the lowest floor where the egg breaks (f).

---> This should produce a runtime complexity of O(log n)
