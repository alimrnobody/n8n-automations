# Crypto & Finance News Automation

This n8n workflow fetches financial news from RSS feeds and posts them automatically to a Telegram channel.

Features:
- Fetches RSS feeds from CoinDesk
- Detects category (Crypto / Gold / Finance)
- Prevents duplicate news posts
- Extracts article images
- Automatically posts to Telegram

I built an automated news distribution workflow using n8n that runs every two hours.
The system fetches RSS feeds from trusted sources like CoinDesk, parses the XML data, and extracts the latest article information including the title and link.

The workflow then automatically categorizes the news into crypto, gold, or general finance based on the source and keywords. To avoid reposting the same content, it stores previously published links using workflow static data and checks for duplicates before posting.

After selecting a new article, the automation fetches the article page and extracts the Open Graph image. If no image is available, a predefined fallback image is used to maintain visual consistency.

Finally, the system automatically publishes the news to a Telegram channel with a formatted caption, relevant hashtags, and an image, ensuring the channel stays updated with fresh market news without any manual effort.
