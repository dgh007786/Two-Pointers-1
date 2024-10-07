# Two-Pointers-1

## Problem1 (https://leetcode.com/problems/sort-colors/)
time and space: O(n) and O(1) 
# Dutch National Flag Algorithm

class Solution:
    def sortColors(self, nums: List[int]) -> None:
        """
        Do not return anything, modify nums in-place instead.
        """
        low = 0
        mid = 0 
        high = len(nums) - 1

        while mid <= high:
            # if mid is 0 swap low and mid and increment low and mid
            if nums[mid] == 0:
                nums[mid], nums[low] = nums[low], nums[mid]
                mid+=1
                low+=1
            # if mid is on mid do nothing
            elif nums[mid] == 1:
                mid+=1
            # if mid is 1 swap high and mid and decrement high
            else:
                nums[mid], nums[high] = nums[high], nums[mid]
                high-=1

        return nums
        

## Problem2 (https://leetcode.com/problems/3sum/)




## Problem3 (https://leetcode.com/problems/container-with-most-water/)

