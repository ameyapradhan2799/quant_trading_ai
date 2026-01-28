📈 Quantitative Trading AI – Multi-Country & Multi-Asset Price Prediction System

🌍 Overview  
Quantitative Trading AI is a Python-based intelligent system that predicts **price movements in real time** across **multiple countries and asset classes**, using advanced **machine learning**, **technical analysis**, and **sentiment analysis**.

The application supports both **stocks** and **commodities** (such as Gold and Silver) and allows users to:

- Select a country (e.g., India, USA, UK, Japan, etc.)
- Select an asset type (Stock or Commodity)
- Search for a stock or commodity by name
- Get real-time predictions and sentiment insights
- Visualize historical trends and model outputs through a user-friendly web interface

This project is designed to be **scalable**, **memory-efficient**, and **production-ready**, using **parallel processing** and **modular system design**.

---

🚀 Features

✅ Multi-Country Support  
Choose a country and automatically fetch market data, trading hours, and relevant news for that region.

✅ Multi-Asset Support (Stocks & Commodities)  
- Equities: Stocks and shares across global markets  
- Commodities: Gold, Silver, Oil, and other major commodities  

Each asset is processed using the same unified prediction pipeline.

✅ Real-Time Market Data  
Pulls live OHLCV (Open, High, Low, Close, Volume) data using APIs such as:
- `yfinance`
- NSE/BSE-compatible tickers for Indian markets

✅ Smart Sentiment Analysis  
Incorporates sentiment from:
- Global financial news
- Domestic (country-specific) news
- Industry- or commodity-specific news  
to refine and contextualize price predictions.

✅ Parallel Processing  
Optimized computation to reduce latency by running data ingestion, feature engineering, and inference tasks in parallel.

✅ User-Friendly Interface  
Designed as a web application (Streamlit-based initially), with future expansion planned for mobile interfaces.

✅ Memory-Efficient Architecture  
Built to support multiple countries and assets without unnecessary memory overhead.

---

🧠 Architecture Overview

User Interface (Web App)  
&nbsp;&nbsp;&nbsp;&nbsp;│  
&nbsp;&nbsp;&nbsp;&nbsp;▼  
Country & Asset Selection Engine  
&nbsp;&nbsp;&nbsp;&nbsp;│  
&nbsp;&nbsp;&nbsp;&nbsp;▼  
Market Data Ingestion Layer  
&nbsp;&nbsp;&nbsp;&nbsp;│  
&nbsp;&nbsp;&nbsp;&nbsp;▼  
Feature Engineering & Model Pipeline  
&nbsp;&nbsp;&nbsp;&nbsp;│  
&nbsp;&nbsp;&nbsp;&nbsp;▼  
Sentiment Analysis Layer (News & Media)  
&nbsp;&nbsp;&nbsp;&nbsp;│  
&nbsp;&nbsp;&nbsp;&nbsp;▼  
Prediction & Visualization Layer  

---

🗂️ Project Structure

quant_trading_ai/  
│  
├── data/  
│   ├── india/  
│   ├── usa/  
│   ├── uk/  
│   ├── commodities/  
│   └── ...  
│  
├── models/  
│  
├── src/  
│   ├── __init__.py  
│   ├── country_config.py       # Country → market & API mapping  
│   ├── asset_config.py         # Stock vs Commodity configuration  
│   ├── data_loader.py          # Dynamic data fetching logic  
│   ├── features.py             # Technical indicators & preprocessing  
│   ├── model.py                # Machine learning / deep learning models  
│   ├── sentiment.py            # News sentiment extraction & scoring  
│   └── app.py                  # Web app (UI + backend logic)  
│  
├── requirements.txt  
└── README.md  

---

⚙️ Setup Instructions

1️⃣ Clone the Repository  
```bash
git clone https://github.com/ameyapradhan2799/quant_trading_ai.git
cd quant_trading_ai
````

2️⃣ Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/Scripts/activate    # Windows Git Bash
# or
venv\Scripts\activate           # Windows Command Prompt
```

3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

4️⃣ Run the Application

```bash
python src/app.py
```

---

🌐 Data Sources

| Country / Asset | Data Source        | Python Library | Example Ticker |
| --------------- | ------------------ | -------------- | -------------- |
| 🇮🇳 India      | NSE / BSE          | yfinance       | RELIANCE.NS    |
| 🇺🇸 USA        | Yahoo Finance      | yfinance       | AAPL           |
| 🇬🇧 UK         | Yahoo Finance      | yfinance       | BARC.L         |
| 🇯🇵 Japan      | Yahoo Finance      | yfinance       | 7203.T         |
| 🪙 Gold         | Global Commodities | yfinance       | GC=F           |
| 🪙 Silver       | Global Commodities | yfinance       | SI=F           |

---

🧮 Planned Enhancements (Phase 2)

* Portfolio optimization based on model outputs
* Backtesting engine for historical simulation
* Advanced deep learning models (LSTM, Transformers)
* Cloud deployment (AWS / GCP / Azure)
* Mobile app interface for real-time monitoring

---

🧑‍💻 Contributing

1. Fork this repository
2. Create a new branch:

```bash
git checkout -b feature/new-feature
```

3. Commit your changes:

```bash
git commit -m "Added <feature-name>"
```

4. Push to your branch:

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

🧾 License

This project is licensed under the **MIT License** — free to use and modify with attribution.

---

📬 Author

**Ameya Pradhan**
M.Sc FinTech | B.Tech Computer Science Engineering (Data Science)

📧 Email: [ptadhanameya27@gmail.com](mailto:pradhanameya27@gmail.com)
💼 GitHub: [https://github.com/ameyapradhan2799](https://github.com/ameyapradhan2799)
