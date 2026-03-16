# Gold & Crypto Live Price Automation

This n8n workflow posts hourly market updates to a Telegram channel.

Data sources:
- CoinGecko API (BTC, ETH, BNB, SOL)
- Investing.com (Gold price)

Output:
Telegram message with formatted market prices.


I built an automated market update system using n8n.
A scheduled trigger runs every hour and fetches live gold prices from Investing.com using an HTTP request and HTML scraping.
At the same time, the workflow calls the CoinGecko API to retrieve live cryptocurrency prices for BTC, ETH, BNB, and SOL.
These two data sources are merged and processed in a JavaScript node where I format the prices, determine price movement using 24-hour change data, and generate a formatted message.
Finally, the workflow automatically posts the market update to my Telegram channel using a Telegram bot

