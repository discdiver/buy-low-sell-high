## Backtesting Long-Term S&amp;P 500 Investment Strategies for Dollar Cost Averaging, PE, and Shiller PE Ratio Triggers

### "Buy low and sell high" is standard investment advice. 

However, investors buy when they think the price is going to rise and sell when they think the price is going to fall lower. Often times investors are chasing the market. They sell when fear has taken over and prices have already fallen. They buy when everyone is euphoric and prices are already high. 

In Nate Silver's book, *The Signal and the Noise*, he discusses how buying stocks when the 10 Year PE ratio (Shiller PE) is under 15 results in much better long term returns (pp. 346-350 paperback edition). 

Buying when stocks are valued cheaply - when one dollar of earnings is cheap relative to the historical average - should be a good investment strategy. But the proof is in the pudding, the devil is in the details, and the code needs written and run.

I'm certainly not the first person to test a value investment strategy like this one, but I'll look at various triggers for buying and selling. This is also a good exercise in building a basic back-testing process with python, pandas, and numpy.

Dollar cost averaging is another recommended investment strategy. Let's use that as a baseline. 

Rough plan:

1. Import S&P 500, PE, and Shiller PE monthly data, from [Quandl](https://www.quandl.com). 
2. Build DataFrames.
3. Code strategies to buy and sell based on triggers related to PE or Shiller PE ratios.  
4. Evaluate.
5. Iterate.
