# Time Series Forecasting with Neural Networks

## Project Overview
This project demonstrates forecasting Tesla (TSLA)/Moderna (MRNA) stock prices using two deep learning models:
- A Feedforward Neural Network
- An LSTM Neural Network

It includes step-by-step explanations and an interactive Gradio app for real-time prediction.

## Features
- 📈 Fetches 5 years of stock data using `yfinance`
- 🔄 Preprocesses data using normalization and sliding windows
- 🤖 Trains two models: Dense (Feedforward) and LSTM networks
- 📊 Visualizes actual vs. predicted prices
- 🌐 Includes a Gradio web app for interactive predictions

## How It Works

1. **Data Collection**: Downloads historical TSLA closing prices.
2. **Preprocessing**: Normalizes data and prepares input-output sequences.
3. **Model Training**:
   - **Feedforward Neural Network**: Simple Dense layers for regression.
   - **LSTM Neural Network**: Captures sequential patterns in stock data.
4. **Evaluation**: Plots actual vs. predicted prices to compare performance.
5. **Gradio App**: Lets users input 10 recent closing prices and predicts the next day's closing price.

## Requirements

- numpy
- pandas
- matplotlib
- tensorflow / keras
- yfinance
- gradio

Install dependencies via:

```bash
pip install -r requirements.txt
```

## Usage

1. Run the notebook to train models and visualize results.
2. To launch the Gradio app, uncomment the last line:

```python
iface.launch()
```

## Example Input for Gradio

```
[354.11, 360.56, 354.40, 337.80, 330.53, 302.80, 290.80, 281.95, 292.98, 284.65]
```

## Future Improvements

- Hyperparameter tuning
- Use of additional features (volume, open/high/low prices)
- Deployment of the app online

---

