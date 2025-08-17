# CryptoAI Backend

Advanced cryptocurrency analysis backend with AI-powered trading insights.

## Features

- **Mini Scalping Analysis**: Ultra-fast trading signals with order book analysis
- **Scalping Analysis**: Short-term trading with pivot points and Fibonacci levels
- **Daily Trading Analysis**: Medium-term analysis with market sentiment
- **Swing Trading Analysis**: Long-term analysis with fundamental data
- **AI-Powered Insights**: DeepSeek AI integration for advanced market analysis

## API Endpoints

- `GET /miniscalping/{symbol}` - Mini scalping analysis
- `GET /scalping/{symbol}` - Scalping analysis  
- `GET /daily/{symbol}` - Daily trading analysis
- `GET /swing/{symbol}` - Swing trading analysis
- `GET /indicators_binance/{symbol}?interval={interval}&limit={limit}` - Technical indicators

## Setup

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Set environment variables:
```bash
export BINANCE_API_KEY="your_api_key"
export BINANCE_SECRET_KEY="your_secret_key"
```

3. Run the server:
```bash
uvicorn main:app --host 0.0.0.0 --port 8000
```

## Render Deployment

This backend is configured for Render.com deployment with automatic scaling and HTTPS support. 