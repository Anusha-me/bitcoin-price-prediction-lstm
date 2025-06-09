🧠 LSTM Model Summary – Bitcoin Price Forecasting

> 📌 This repository focuses on Bitcoin price forecasting from a stock market perspective using LSTM, covering the period **2017–2024**.  
> A separate version treating Bitcoin as a **currency** will be provided in a future repository.

---

📦 Model Architecture:

- Input Shape: (60, 1)  → sequences of 60 daily prices
- 🧩 Layer 1: LSTM (tunable units: 32–128), return_sequences=True
- 🔽 Dropout (tunable rate: 0.1–0.5)
- 🧩 Layer 2: LSTM (same unit config), return_sequences=False
- 🔽 Dropout (same rate)
- 🔢 Dense Layer: (tunable units: 16–64), ReLU activation
- 🎯 Output Layer: Dense(1) → predicted price

---

🛠 Tunable Hyperparameters:

- `lstm_units`: [32, 64, 96, 128]
- `dropout_rate`: [0.1 to 0.5]
- `dense_units`: [16, 32, 48, 64]
- `learning_rate`: [0.0001 to 0.01] (log scale)

---

🧪 Loss Function:
- Mean Squared Error (MSE)

🚀 Optimizer:
- Adam (tunable learning rate)

🎯 Target:
- Predict the next day's Bitcoin price in USD

---

🔗 Real-time Integration:
- Fetches live Bitcoin price using CoinGecko API (used in validation or to compare with predictions)

📊 Sequence Length Used:
- 60-day window to predict the 61st value

This architecture is designed to balance complexity and generalization by using dropout, sequence-aware layers, and flexible hyperparameter search via KerasTuner.
