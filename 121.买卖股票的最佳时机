#121.买卖股票的最佳时机

class Solution:
    # 动态规划
    def maxProfit(self, prices: List[int]) -> int:
        n = len(prices)
        if n == 0: return 0
        dp = [0] * n
        minprice = prices[0] 
        for i in range(1, n):
            minprice = min(minprice, prices[i])
            dp[i] = max(dp[i - 1], prices[i] - minprice)
        return dp[-1]
