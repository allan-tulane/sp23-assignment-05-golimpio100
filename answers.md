# CMPS 2200 Assignment 5
## Answers

**Name:**__Griffin Olimpio____________


Place all written answers from `assignment-05.md` here for easier grading.





- **1a.**

Greedy Algorithm for producing as few coins as possible that sum to N:

Sort the denominations in descending order (2^k, 2^(k-1), ..., 2^0)
Initialize an empty list for the coins to be used.
For each denomination, repeat:
While the current denomination is less than or equal to the remaining amount, subtract the denomination from the remaining amount and add it to the list of coins to be used.
Return the list of coins to be used.

This algorithm is optimal for this specific problem because the denominations are powers of 2, which guarantees that any amount can be represented as a sum of these denominations without any gaps or overlaps. The greedy algorithm selects the largest possible coin at each step, ensuring the minimum number of coins is used.


Work: O(k), as we loop through each denomination once.
Span: O(1), there is no parallelism in the algorithm.






- **2b.**

Create a memoization table dp of size N+1, with dp[0] = 0 and the rest initialized to infinity.
For each denomination, loop from the denomination value to N+1:
a. Update dp[i] to be the minimum between dp[i] and dp[i-denomination]+1.
If dp[N] is still infinity, there is no solution. Otherwise, return dp[N].
Work: O(kN), as we loop through all the denominations and for each denomination, we loop through all values from the denomination to N.
Span: O(1), there is no parallelism in the algorithm.



- **3a.**






- **3b.**






- **3c.**



