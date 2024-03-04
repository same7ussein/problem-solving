# Squares of a Sorted Array


### Problem Statement:

The problem statement for "977. Squares of a Sorted Array" can be found on <a href="https://leetcode.com/problems/squares-of-a-sorted-array/description/" style="background-color:#FFA500;color:#fff;padding:10px 20px;text-decoration:none;border-radius:5px;display:inline-block;">LeetCode</a>.


Given an integer array `nums` sorted in non-decreasing order, return an array of the squares of each number sorted in non-decreasing order.

### Example:

**Input:** `nums = [-4,-1,0,3,10]`  
**Output:** `[0,1,9,16,100]`  
**Explanation:** After squaring, the array becomes `[16,1,0,9,100]`. After sorting, it becomes `[0,1,9,16,100]`.

### Constraints:

- 1 <= nums.length <= 10^4
- -10^4 <= nums[i] <= 10^4
- nums is sorted in non-decreasing order.

### Follow-up:

Squaring each element and sorting the new array is very trivial, could you find an O(n) solution using a different approach?

## Solution:

```javascript
var sortedSquares = function (nums) {
  return nums.map((num) => Math.pow(num, 2)).sort((a, b) => a - b);
};
