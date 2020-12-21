#263.丑数

class Solution:
    def isUgly(self, num: int) -> bool:
        if num <= 0:
            return False
        nums = [2,3,5]
        for i in nums:
            while num % i == 0:
                num //= i
        return num == 1
