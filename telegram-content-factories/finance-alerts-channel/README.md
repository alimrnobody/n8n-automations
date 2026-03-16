# Finance Alerts Channel Automation

This project contains automation workflows built with **n8n** to run a fully automated Telegram channel that posts financial updates and market news.

The system automatically fetches **live asset prices and financial news** and publishes formatted updates to a Telegram channel.

---

## Automation Features

* Automated financial news posting
* Live crypto price updates
* Live gold price tracking
* Multi-source market news aggregation
* Duplicate news prevention
* Automated Telegram posting

---

## Included Workflows

### 1. Gold & Crypto Live Price Automation

Posts hourly market updates including:

* BTC price
* ETH price
* SOL price
* BNB price
* Gold price

Data Sources:

* CoinGecko API
* Investing.com

---

### 2. Crypto & Finance News Automation

Fetches and posts the latest crypto and finance news from RSS feeds.

Features:

* RSS feed parsing
* Automatic category detection (Crypto / Gold / Finance)
* Image extraction from article pages
* Duplicate news protection

Data Source:

* CoinDesk RSS

---

### 3. Market News Aggregator

Fetches financial news from multiple APIs and publishes the latest market updates.

Features:

* Multi-API news fetching
* Duplicate article prevention
* Automated Telegram posting with image

Data Sources:

* MarketAux API
* GNews API

---

## Technologies Used

* n8n (Workflow Automation)
* Telegram Bot API
* CoinGecko API
* MarketAux API
* GNews API
* Web Scraping
* RSS Parsing

---

## Telegram Channel

Example automation output is published to:

**@financealerts0**

---

## Project Goal

This project demonstrates how **workflow automation can be used to build a fully automated financial news and market alert system using n8n.**
