# 📈 Bitcoin Price Forecasting with LSTM & Real-Time Data

This project forecasts Bitcoin prices using a Long Short-Term Memory (LSTM) neural network. It combines historical Excel-based datasets with real-time data fetched via the CoinGecko API and applies rigorous cleaning, outlier removal, and sequence modeling to build accurate time-series predictions.

---

## 🧠 Objective

- Clean and unify historical price data from multiple sources
- Interpolate missing values and remove outliers using IQR
- Create sequences for LSTM using a rolling window approach
- Build an LSTM model with tunable hyperparameters via KerasTuner
- Integrate real-time Bitcoin price fetching (CoinGecko API)
- Forecast the next Bitcoin price point

---

## ⚙️ Key Features

- 📅 Multi-sheet Excel ingestion with smart merging
- 🧹 Full pipeline: datetime parsing, median aggregation, IQR-based outlier removal
- 🔗 Real-time API integration with fallback handling
- 🔁 Sequence creation for time-series forecasting
- 🧪 KerasTuner for LSTM architecture optimization

---

## 🧾 Files Included

```plaintext
📄 Bitcoins_forecasting_code.ipynb      # Main Jupyter notebook with code
📘 Bitcon_explaination.pdf        # Explanation of methodology and code
📦 requirements.txt                # Required Python libraries
🧠 model_summary.txt               # Architecture and training process
📊 Bitcon_Research_Dataset.xlsx    #Cleaned and interpolated dataset of Bitcoin stock prices from 2017 to 2024 (no weekends), used for LSTM training.

README.md                          # Project overview (this file)
