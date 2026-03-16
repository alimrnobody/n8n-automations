# Market News Aggregator

This n8n workflow automatically fetches market news from multiple APIs and posts them to a Telegram channel.

Sources:
- MarketAux API
- GNews API

Features:
- Scheduled news fetching
- Duplicate detection
- Automatic Telegram posting

I built an automated financial news distribution workflow using n8n that continuously monitors global market news and publishes updates to a Telegram channel.

The system runs on scheduled intervals and fetches the latest articles from two different news sources — MarketAux API and GNews API — ensuring reliable and diverse coverage of crypto, commodities, and global market events.

Each news item is processed and formatted into a clean Telegram-ready message with hashtags and channel branding.

To prevent reposting the same article, the workflow uses workflow static data to track previously posted links, ensuring that only new and unique news updates are published.

When a new article is detected, the automation extracts the article title, link, and image, formats the caption, and automatically posts the update to the Telegram channel with an image and structured message.

This system allows the channel to stay consistently updated with crypto, gold, oil, inflation, and broader market news without requiring any manual content management.
