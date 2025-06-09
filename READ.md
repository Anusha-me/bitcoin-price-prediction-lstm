# 📈 Bitcoin Price Forecasting with LSTM & Real-Time Data

> 📌 This project is part of a larger research study analyzing Bitcoin from **two perspectives**:
> 
> - 📈 **As a Stock** – influenced by trading volume, technical indicators, market sentiment  
> - 💱 **As a Currency** – influenced by exchange rates, transaction volumes, and lag time
> 
> 🧠 This notebook trains an LSTM model on the **currency perspective dataset**, but the architecture is generalizable across both perspectives and timeframes (2017–2024).

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
📊 Bitcon_Research_Dataset.xlsx    #Cleaned dataset representing the currency perspective (2017–2024), used for LSTM training.Other versions (stock/time-split) are compatible with this code structure.

README.md                          # Project overview (this file)
