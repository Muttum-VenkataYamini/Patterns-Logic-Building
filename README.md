# Patterns-Logic-Building

**1.	Sliding Window  **: 
Used in Linear Structure . Arrays & Strings . 
Basic Concept: What’s a Window?
•	Imagine an array: [1, 2, 3, 4, 5]. You want the maximum sum of any 3 consecutive elements (subarray of size 3).
•	Brute force: Loop through every possible subarray and calculate – slow!
•	Sliding window: Take a fixed-size window (here, size=3), start from the beginning, and slide it forward.
o	First: Window = [1,2,3] → sum=6
o	Slide: [2,3,4] → sum=9 (subtract 1, add 4)
o	Slide: [3,4,5] → sum=12
•	Key Idea: When moving the window, remove the leftmost element (subtract it) and add the new right one (add it). No need to recalculate the whole sum each time!
There are two main types:
•	Fixed Size Window: Window length is constant (e.g., k=3). Like the example above.
•	Variable Size Window: Size changes based on a condition (e.g., expand until sum > target, then shrink).
When to Use Sliding Window? (Pro Tips for Depth)
•	Common Problems: Subarrays/substrings with constraints (e.g., max sum, min length for a sum, no duplicates, must contain all unique chars).
•	Spot It: Keywords like "consecutive elements", "subarray", "longest/shortest with condition".
•	LeetCode Classics: #3 (Longest Substring No Repeat), #209 (Min Size Subarray Sum >= Target), #239 (Sliding Window Maximum).
•	Pros: Fast time (O(n)), low space (O(1) or O(k) for tracking).
•	Cons: Need to handle fixed vs. variable logic carefully; watch edge cases (empty array, k > n).
