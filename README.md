# 📈 Quantitative Trading AI – Multi-Country Stock Price Prediction

## 🌍 Overview
**Quantitative Trading AI** is a Python-based intelligent system that predicts stock price movements in real-time using advanced **machine learning** and **sentiment analysis**.  

The app allows users to:  
- Select a **country** (e.g., India, USA, UK, Japan, etc.)  
- Search for a **stock** by name  
- Get **real-time predictions** and **sentiment insights**  
- Visualize historical trends and model outputs through a user-friendly web interface  

This project is designed to be **scalable**, **memory-efficient**, and **production-ready**, using parallel processing and modular code design.

---

## 🚀 Features
✅ **Multi-Country Support:**  
Choose a country and fetch real-time data from the relevant market automatically.  

✅ **Real-Time Stock Data:**  
Pulls live OHLCV (Open, High, Low, Close, Volume) data using APIs like `yfinance` or `nsetools`.  

✅ **Smart Sentiment Analysis:**  
Analyzes **global, domestic, and industry-specific news** to refine stock predictions.  

✅ **Parallel Processing:**  
Optimized computation to minimize latency and handle multiple model components simultaneously.  

✅ **User-Friendly Interface:**  
Deployed as a **Streamlit web app** (and later expandable to a mobile interface).  

✅ **Memory-Efficient Architecture:**  
Designed to scale across multiple markets without bloating memory usage.

---

## 🧠 Architecture Overview

```
User Interface (Web App)
    │
    ▼
Country Selection Engine  →  Fetches relevant stock data per country
    │
    ▼
Feature Engineering & Model Pipeline  →  ML/DL-based price prediction
    │
    ▼
Sentiment Analysis Layer  →  News, media, and trend sentiment
    │
    ▼
Visualization Layer  →  Price charts, signals, and insights
```

---

## 🗂️ Project Structure

```
quant_trading_ai/
│
├── data/
│   ├── india/
│   ├── usa/
│   ├── uk/
│   └── ...
│
├── models/
│
├── src/
│   ├── __init__.py
│   ├── country_config.py       # Country → API mapping
│   ├── data_loader.py          # Dynamic data fetching logic
│   ├── features.py             # Technical indicators & preprocessing
│   ├── model.py                # Machine learning/deep learning models
│   ├── sentiment.py            # News sentiment extraction & scoring
│   └── app.py                  # Streamlit app (UI + backend)
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/quant_trading_ai.git
cd quant_trading_ai
```

### 2️⃣ Create and Activate Virtual Environment
```bash
python -m venv venv
source venv/Scripts/activate    # (Windows Git Bash)
# or
venv\Scripts\activate           # (Windows Command Prompt)
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application
```bash
python src/app.py
```

---

## 🌐 Data Sources
| Country | Data Source | Python Library | Example |
|----------|--------------|----------------|----------|
| 🇮🇳 India | NSE/BSE | `yfinance` (`.NS` / `.BO`) | RELIANCE.NS |
| 🇺🇸 USA | Yahoo Finance | `yfinance` | AAPL |
| 🇬🇧 UK | Yahoo Finance | `yfinance` (`.L`) | BARC.L |
| 🇯🇵 Japan | Yahoo Finance | `yfinance` (`.T`) | 7203.T |
| 🇩🇪 Germany | Yahoo Finance | `yfinance` (`.DE`) | BMW.DE |

---

## 🧮 Planned Enhancements (Phase 2)
- 🪙 **Add cryptocurrency and commodity support** (e.g., BTC, Gold, Oil)  
- 🧾 **Portfolio optimization** based on model outputs  
- 💹 **Backtesting engine** for historical simulation  
- ☁️ **Cloud deployment** (AWS / GCP / Azure)  
- 📱 **Mobile app interface** for real-time monitoring  

---

## 🧑‍💻 Contributing
1. Fork this repo  
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
5. Open a **Pull Request**

---

## 🧾 License
This project is licensed under the **MIT License** — free to use and modify with attribution.

---

## 📬 Author
**Ameya Pradhan**  
M.Sc FinTech | B.Tech Computer Science Engineering (Data Science)
📧 ptadhanameya27@gmail.com 
💼 https://github.com/ameyapradhan2799

