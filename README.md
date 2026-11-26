# TradeVision AI — RNN Stock Predictor

An exploratory Streamlit app for training a recurrent neural network on historical stock prices and inspecting its predictions. Use it to compare settings and review model errors. It is a learning project for time-series modeling.

## 🚀 Features
- **RNN forecasting**: Uses 3-layer SimpleRNN architecture.
- **Dynamic Hyperparameters**: Adjust training epochs, input window, and forecast horizon.
- **Interactive Technical Analysis**: RSI, Bollinger Bands, and Volume charts.
- **Model Performance Metrics**: RMSE, Residual tracking, and Actual vs Predicted scatter plots.
- **Financial Insights**: Fundamental data, News headlines, and Analyst recommendations.

## 🛠️ Setup
1. Create a virtual environment:
   ```bash
   python -m venv tv_env
   # macOS / Linux
   source tv_env/bin/activate
   # Windows PowerShell: .\tv_env\Scripts\Activate.ps1
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the app:
   ```bash
   streamlit run app.py
   ```

## 📄 Project Structure
- `app.py`: Main Streamlit application and UI logic.
- `data_loader.py`: Fetches market data using `yfinance`.
- `preprocessing.py`: Data scaling and sequence creation.
- `model.py`: RNN model architecture.
- `train.py`: Training logic.
- `predict.py`: Prediction and forecasting functions.
- `requirements.txt`: Python package dependencies.

## Evaluation notes

Use the RMSE and residual views to compare runs. For stronger evidence of forecasting value, compare against a last-price baseline on an untouched chronological test period before drawing conclusions.
