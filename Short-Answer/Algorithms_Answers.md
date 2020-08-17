#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) Runtime is O(n): n^3/n^2 = n. The problem is asking to solve for a being greater than n^3 but we're also given that a goes up n^2 each pass of the while loop. 


b) This is a while loop within a for loop. For loop runtime is O(n), while loop runtime is O(log n). With the the two together, you would multiply giving a runtime of O(n log n).


c) def bunnyEars is a recursive function with a base case of bunnies == 0. Every time we call we're subtracting 1 to get closer and closer to the base case. This is O(n) runtime.

## Exercise II

Use a binary search function to get f the soonest with the least amount of floors climbed and eggs broken. Best is recursive for DRY, clear code, reduced runtime and better tree traversal.

1) determine top floor and bottom floor
2) go to the middle and drop the first egg
3) determine if the egg is broken or not
    a) if the egg breaks, repeat the binary search function using the lower half of the floors
    b) if the egg doesn't break, repeat the search using the upper half of floors
Runtime for this would be O(log n)
