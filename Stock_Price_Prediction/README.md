# **Stock Price Prediction Using Machine Learning and Power BI**  

This project focuses on predicting stock prices using **LSTM-based machine learning models** and visualizing key metrics with **Power BI dashboards**. The primary goal is to achieve actionable insights for stock market trends and provide a dynamic, user-friendly interface for decision-making.

---

## **🔍 Project Overview**  

### Key Objectives:
1. **Stock Price Prediction**: Utilize historical data to predict stock trends using an **LSTM (Long Short-Term Memory)** neural network.  
2. **Dynamic Dashboards**: Visualize predictions, technical data, and news insights in **Power BI**.  
3. **Data Redundancy Reduction**: Employ **EDA (Exploratory Data Analysis)** and feature engineering to optimize the dataset.  
4. **Enhanced Decision-Making**: Deliver actionable insights with over 70% win rate in predictions.

---

## **📊 Tools & Technologies**  
- **Python**: For data preprocessing and building the LSTM model.  
- **Power BI**: For creating interactive dashboards.  
- **Pandas & NumPy**: For data manipulation and analysis.  
- **TensorFlow/Keras**: To design and train the LSTM model.

---

## **📂 Project Structure**  

```plaintext
stock-price-prediction/
│
├── data/
│   ├── stock_prices.csv    # Raw dataset
│   ├── cleaned_data.csv    # Cleaned and preprocessed data
│
├── model/
│   ├── lstm_model.py       # LSTM model training script
│   ├── model_checkpoint/   # Saved model weights
│
├── dashboards/
│   ├── stock_dashboard.pbix    # Power BI dashboard file
│   ├── dashboard_screenshots/  # Visual examples of dashboards
│
├── insights/
│   ├── summary_report.md   # Insights and analysis summary
│
├── README.md
└── LICENSE
```
``` Python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense
from tensorflow.keras.layers import LSTM
     

model = Sequential()
model.add(LSTM(50 , return_sequences = True , input_shape =(100 , 1)))
model.add(LSTM(50 , return_sequences=True))
model.add(LSTM(50))
model.add(Dense(1))
model.compile(loss= 'mean_squared_error' , optimizer = 'adam')
```
## **📊 Power BI Dashboard**
The Power BI dashboard combines:

1. **Stock Price Trends**: Predicted vs. Actual prices over time.
2. **News Analysis**: Sentiment from live stock market news feeds.
3. **Technical Indicators**: RSI, MACD, and other metrics to enhance decision-making.
4. **Preview of the Dashboard**:

   ![image](https://github.com/user-attachments/assets/34c4a05e-f272-4c5d-b1a7-29ab65c87cc7)


## **📝 Insights**
**Prediction Accuracy**: Achieved a 47% model accuracy during back-testing, improving predictions with additional features.
**Win Rate**: Demonstrated a 70% success rate in predicting upward and downward trends.
**Dashboard Impact**: Provided stakeholders with an intuitive interface for stock analysis.
## **🚀 Future Enhancements**
Integrate live stock market data for real-time predictions.
Enhance the model by adding sentiment analysis from news and social media.
Expand dashboards to include industry and sector-specific analytics.
