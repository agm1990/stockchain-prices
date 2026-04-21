# stockchain-prices

自动化股价数据源，给 StockChain 桌面 App 使用。

- **更新频率**：每 15 分钟一次（由 macOS launchd 定时任务触发）
- **数据来源**：Yahoo Finance（通过 Python `yfinance` 库）
- **数据格式**：`{ ticker: { price, change }, ..., _updated: "YYYY-MM-DD HH:MM:SS" }`
- **App 拉取 URL**：https://raw.githubusercontent.com/agm1990/stockchain-prices/main/prices.json

由 StockChain 主项目的 `scripts/fetch_prices.py` 自动生成并推送。
