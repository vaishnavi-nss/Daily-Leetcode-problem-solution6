# Daily-Leetcode-problem-solution6
PROBLEM

An array is considered special if every pair of its adjacent elements contains two numbers with different parity.
You are given an array of integer nums and a 2D integer matrix queries, where for queries[i] = [from i, to i] your task is to check that 
subarray nums[from i..to i] is special or not.
Return an array of booleans answer such that answer[i] is true if nums[from i..to i] is special.

Intuition

Identify parity violations
Use binary search for query processing

Approach

Iterate through array
Track indices with parity violations.
For each query, use lower_bound to check for violations.
If no violation or violation is outside the sub array then mark as special.

Complexity
Time complexity:

Query processing with binary search: O(q logn)
Preprocessing violations: O(n)
Overall time complexity: O(n + qlogn)

Space complexity:

O(v), v is number of violations
