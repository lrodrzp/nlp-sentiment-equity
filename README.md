# nlp-sentiment-equity
Why stocks move using AI-powered news analysis

# News Attribution Pipeline

Automatically explains why stocks move using AI-powered news analysis.

When a stock jumps or drops significantly, this pipeline:
1. Detects the abnormal price movement
2. Fetches relevant news from multiple sources
3. Uses AI to identify which articles explain the move
4. Generates a summary with sentiment analysis

### Output
```
STOCK: INTC
Price Change: +10.19%
Sentiment: Positive (0.904)

SUMMARY:
Intel surged on CEO change announcement. Analysts upgraded 
citing improved execution outlook in data center segment.
```

## Get API Keys (Free)
- [NewsAPI](https://newsapi.org/register) - 100 requests/day free
- [Groq](https://console.groq.com/) - Fast LLM inference

## How It Works
```
Stock Moves ±5% → Fetch News → AI Filters Relevant Articles 
→ Generate Summary → Sentiment Analysis → Report
```

**Technologies:**
- Price data: `yfinance`
- News: NewsAPI, Google News, Yahoo Finance
- AI: Llama 3.1 (via Groq) + FinBERT

## Limitations

- Free tier: ~5 stocks per day
- Processes daily moves (not real-time)
- Misses paywalled news (Bloomberg, etc.)

## License

This project is for educational purposes.
