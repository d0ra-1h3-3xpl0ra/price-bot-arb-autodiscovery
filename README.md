# price-bot-arb-autodiscovery
Queries DEX, Compares Token Prices and highlightes profitable Arbs MVP

This Bot version will first fetch realtime data
and will access the mainnet.

For further testing, I will switch the RPC URL to a Testnet to explore how to best implement FlashLoan Functionality and how to merge the Execution Price Bot with the autodiscover code...
1. Afer initializing the Repo, populate .env file with
   1. Mainnet RPC URL 
   2. Set Port 




Issues / Challenges

Uniswap uses the Factory Model, meaning it uses specific exchanges/contract addresses for each token we want to trade.

Our function exchangeAddress provides the necessary functionality (it passes the token Smart Contract Address to the exchangeAddress function, which then calls the required exchange)  

For that uniswap has factory to find the right exchange...


## Project Extension 

1. Adding More Tokens via checkPair() (easy)
2. Add more Exchanges
   1. Find their ABI 
   2. Look at their SC on eg. Etherscan 
   3. Import them into the Project 
   4. Find then out how to get their prices

3. Compare Prices
   1. Add Logic that evaluates if x is less than y
   2. Perhaps highlights or logs it somehow 
   3. By how much?

4. Execute trades based on the findings of price comparison 
5. BONUS: Implement Flashloans 

