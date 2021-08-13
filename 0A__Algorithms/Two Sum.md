https://leetcode.com/problems/two-sum/

Given an array of integers `nums` and an integer `target`, return _indices of the two numbers such that they add up to `target`_.
You may assume that each input would have **_exactly_ one solution**, and you may not use the _same_ element twice.
You can return the answer in any order.

Example 1:
**Input:** nums = [2,7,11,15], target = 9
**Output:** [0,1]
**Output:** Because nums[0] + nums[1] == 9, we return [0, 1].

Example 2:
**Input:** nums = \[3,2,4\], target = 6
**Output:** \[1,2\]

Example 3:
**Input:** nums = [3,3], target = 6
**Output:** [0,1]

**Constraints:**

-   `2 <= nums.length <= 104`
-   `-109 <= nums[i] <= 109`
-   `-109 <= target <= 109`
-   **Only one valid answer exists.**

```py
# base
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
```

```py
# solution

class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        
        num_to_index = {}	# key is number, value is index in nums
        
        for i, num in enumerate(nums):
            if target - num in num_to_index:
                return [num_to_index[target - num], i]
            
            num_to_index[num] = i
        return []  # no sum
		
```