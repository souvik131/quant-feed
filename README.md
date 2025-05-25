# Quant Feed MCP Integration Guide

**Get powerful financial analysis tools directly in Claude Desktop with just one simple configuration!**

## 🎥 Setup Video Tutorial

**Watch the complete setup process: [Setup Tutorial](https://www.youtube.com/watch?v=OT9SbKe19Cg)**

## What is Quant Feed?

Quant Feed is a comprehensive financial analysis API that provides 17 advanced tools for:

- 📈 Historical data analysis
- 📊 Technical indicators (RSI, MACD, Bollinger Bands, etc.)
- 🎯 Risk metrics (Sharpe ratio, VaR, drawdown analysis)
- 💼 Portfolio optimization and allocation
- 🔍 Correlation analysis and seasonal patterns
- ✅ Data quality validation

## 🚀 Quick Setup (2 Minutes)

### Step 1: Install Claude Desktop

Download and install Claude Desktop from [claude.ai](https://claude.ai/download)

### Step 2: Configure Claude Desktop

1. Open Claude Desktop
2. Go to **Settings → Developer → Edit Config**
3. Add the following configuration to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "quant-feed": {
      "command": "npx",
      "args": ["mcp-remote", "https://quant-feed-ln4o5.ondigitalocean.app/sse"],
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

### Step 3: Start Using!

That's it! Restart Claude Desktop and you can now use powerful financial analysis directly in Claude.

## 💡 Example Usage

Once configured, you can ask Claude things like:

### 📊 Basic Analysis

```
"Get historical data for AAPL for the last 100 days"

"Calculate RSI for Tesla stock"

"Show me correlation between Apple and Microsoft"
```

### 📈 Advanced Analysis

```
"Analyze risk metrics for my portfolio: AAPL:40, GOOGL:30, MSFT:30"

"Optimize a portfolio with AAPL, GOOGL, MSFT, TSLA"

"Show seasonal patterns for SPY over the last year"

"Calculate Bollinger Bands for Bitcoin"
```

### 💼 Portfolio Management

```
"What's the Sharpe ratio for AAPL?"

"Analyze the correlation matrix for tech stocks: AAPL,GOOGL,MSFT,AMZN"

"Show me the efficient frontier for a 3-stock portfolio"
```

## 🛠️ Available Tools

### 📊 Basic Analysis (6 tools)

- **Historical Data**: Get OHLCV data for any symbol
- **Symbol Search**: Find stocks, crypto, forex symbols
- **Statistics**: Calculate return statistics automatically
- **Correlation**: Compare two assets
- **Technical Indicators**: SMA, EMA, RSI, ATR
- **Data Quality**: Validate data integrity

### 📈 Medium Analysis (5 tools)

- **Risk Metrics**: Sharpe, Sortino, Max Drawdown, VaR, CVaR
- **Portfolio Metrics**: Beta, Alpha vs benchmark
- **Advanced Technical**: Bollinger Bands, MACD, Stochastic
- **Distribution**: Skewness, Kurtosis analysis
- **Correlation Matrix**: Multi-asset correlation

### 🎯 Advanced Analysis (5 tools)

- **Seasonal Patterns**: Day-of-week, month-of-year effects
- **Trend Analysis**: Linear, polynomial, moving averages
- **Portfolio Optimization**: Mean-variance optimization
- **Portfolio Allocation**: Custom weight analysis
