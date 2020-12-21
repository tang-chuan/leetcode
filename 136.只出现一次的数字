#136.只出现一次的数字

class Solution:
    def singleNumber(self, nums: List[int]) -> int:
        if len(nums)==1:
            return nums[0]   
        nums.sort()
        for i in range(1,len(nums),2):
            if nums[i-1] != nums[i]:
                return nums[i-1]
            if (i+2) == len(nums):
                return nums[-1]
