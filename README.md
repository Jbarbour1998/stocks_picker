# Stock Dashboard

A Streamlit web app for visualizing stock price data, technical indicators, and real-time prices using data from Yahoo Finance.

## Screenshot Of the dashboard
<img width="1906" height="914" alt="image" src="https://github.com/user-attachments/assets/0afe97c3-5d5f-490e-a2cd-8f985b485b4a" />

## Features

- **Interactive charting** — view any stock ticker as a candlestick or line chart
- **Configurable time periods** — 1 day, 1 week, 1 month, 1 year, or max history
- **Technical indicators** — overlay Simple Moving Average (SMA 20) and Exponential Moving Average (EMA 20)
- **Key metrics** — last price, price change, percent change, high, low, and volume
- **Historical data table** — view the underlying OHLCV data and indicator values
- **Real-time sidebar** — live price snapshots for AAPL, GOOGL, AMZN, and MSFT

## Requirements

- Python 3.9+
- streamlit
- plotly
- pandas
- yfinance
- pytz
- ta

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Jbarbour1998/stocks_picker.git
   cd stocks_picker
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv stock_picker_venv
   # Windows
   stock_picker_venv\Scripts\activate
   # macOS/Linux
   source stock_picker_venv/bin/activate
   ```

3. Install dependencies:

   ```bash
   pip install streamlit plotly pandas yfinance pytz ta
   ```

   Or, if a `requirements.txt` is present:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the app with:

```bash
streamlit run stock_dashboard.py
```

This starts a local server and opens the dashboard in your browser at `http://localhost:8501`.

### Using the dashboard

1. Enter a stock ticker in the sidebar (default: `ADBE`).
2. Choose a time period and chart type.
3. Optionally select technical indicators to overlay on the chart.
4. Click **Update** to fetch data and render the chart, metrics, and historical data tables.
5. Real-time prices for a fixed watchlist (AAPL, GOOGL, AMZN, MSFT) are shown in the sidebar automatically.

## Project Structure

```
stock_picker/
├── stock_dashboard.py     # Main Streamlit application
├── requirements.txt       # Python dependencies
└── README.md               # This file
```

## Notes

- Data is sourced live from Yahoo Finance via the `yfinance` package, so results depend on market data availability and may be delayed.
- Time data is localized to US/Eastern for consistency.

## Project Contniuation

- This project is a carry on in progress for my personal and will continue to be improved and updated 
