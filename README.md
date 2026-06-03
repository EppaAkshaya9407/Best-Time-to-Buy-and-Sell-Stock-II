# Best-Time-to-Buy-and-Sell-Stock-II
prices = list(map(int,input("Enter stock prices: ").split()))
profit = 0
for i in range(1, len(prices)):
    if prices[i] > prices[i - 1]:
        profit += prices[i] - prices[i - 1]
print("Maximum Profit:", profit)
