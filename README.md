# Stock Price Prediction Using AI 📈

## 🚀 Project Overview
This project predicts the **future stock prices of Reliance Industries** using **Linear Regression**, a supervised machine learning algorithm. The model is trained on historical stock data fetched from **Yahoo Finance** and forecasts the closing price for the upcoming week.

## 🧠 AI Model Used: **Linear Regression**
Linear Regression is a fundamental machine learning algorithm used for predictive modeling. It establishes a relationship between **time (independent variable)** and **closing stock prices (dependent variable)** using the equation:

y = mx + c  
where:
- **y** = Predicted stock price
- **m** = Slope of the regression line (rate of change)
- **x** = Date in numerical format
- **c** = Y-intercept (base value of stock price when x = 0)

### 🔍 **How This Model Works**
1. **Data Collection**: Fetches **5 years of historical stock data** for Reliance Industries from Yahoo Finance.
2. **Data Preprocessing**: Converts dates into numerical format for model compatibility.
3. **Training the Model**: Uses **80% of the dataset** for training and 20% for testing.
4. **Prediction**: The model predicts the **next 7 days' stock prices** based on the historical trend.
5. **Visualization**: The results are plotted to compare **actual vs. predicted prices**.

## 📌 Key Features
✅ **Fetches real-time stock data** using Yahoo Finance API  
✅ **Applies machine learning (Linear Regression)** for prediction  
✅ **Splits data for training and testing** using Scikit-Learn  
✅ **Generates a 7-day future price forecast**  
✅ **Visualizes stock trends using Matplotlib**  

## 🔥 Challenges Faced & Solutions
### **1️⃣ Handling API Data Fetching Errors**
**Problem**: Sometimes, Yahoo Finance returns an empty dataset due to API limits.  
**Solution**: Implemented a validation check to ensure data retrieval before processing.

### **2️⃣ Date Format Compatibility**
**Problem**: The model cannot process date values directly.  
**Solution**: Converted dates into an **ordinal format** using `pd.Timestamp.toordinal()`.

### **3️⃣ 2D vs. 1D Array Error in Pandas**
**Problem**: Encountered a `ValueError` while creating the predictions dataframe.  
**Solution**: Used `.flatten()` to reshape the predictions into a 1D array.

### **4️⃣ Accuracy Improvement**
**Problem**: Basic Linear Regression may not always give accurate stock predictions.  
**Solution**: Future improvements could include **LSTM, ARIMA, or Facebook Prophet** for better forecasting.

## 📚 Learning Outcomes
By working on this project, I gained experience in:
✔ **Financial data analysis** using Python libraries (Pandas, NumPy)  
✔ **Supervised learning (Linear Regression)** and its real-world applications  
✔ **Data preprocessing and feature engineering** for AI models  
✔ **Time-series forecasting** for stock market trends  
✔ **Debugging and handling real-time API data issues**  
✔ **Building AI-based projects for portfolio and job applications**  

## 💡 Future Enhancements
🔹 Implement **LSTM (Long Short-Term Memory)** for better deep learning-based predictions  
🔹 Add **Sentiment Analysis on news articles** for improved stock forecasts  
🔹 Develop a **web app with Flask or Streamlit** for real-time stock price predictions  

## 📂 Installation & Setup
### **1️⃣ Install Dependencies**
Run the following command to install the required libraries:
```bash
pip install yfinance pandas numpy scikit-learn matplotlib
```

### **2️⃣ Run the Script**
```bash
python stock_price_prediction.py
```

## 👨‍💻 Author
**[Your Name]** – AI & ML Enthusiast | Data Scientist | Software Engineer  
📌 **GitHub**: [Your GitHub Profile](https://github.com/yourgithub)  
📌 **LinkedIn**: [Your LinkedIn Profile](https://www.linkedin.com/in/yourlinkedin)  

## ⭐ Like This Project?
If you found this project helpful, consider giving it a ⭐ on GitHub! 🚀

