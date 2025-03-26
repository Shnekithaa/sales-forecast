# Walmart Sales Forecasting 📈

## 📌 Overview
This project analyzes Walmart sales trends, explores correlations with economic factors, and forecasts future sales using **SARIMA**. The analysis is done using **Python**, with a focus on exploratory data analysis (EDA), correlation analysis, and time series forecasting.

## 📂 Dataset
- The dataset used: `Walmart DataSet.csv`
- Contains sales, unemployment, CPI, and temperature data across multiple Walmart stores.

## 🛠 Technologies Used
- **Python**
- **Pandas, NumPy** – for data manipulation
- **Matplotlib, Seaborn** – for data visualization
- **Statsmodels** – for statistical modeling & time series forecasting
- **Scikit-learn** – for regression analysis
- **SciPy** – for statistical correlation analysis

## 📊 Data Processing & Analysis
### **1️⃣ Data Cleaning & Preprocessing**
- Converted `Date` column to datetime format.
- Handled missing values by filling them with the median.

### **2️⃣ Exploratory Data Analysis (EDA)**
- Identified correlations between `Weekly_Sales` and factors like:
  - **Unemployment Rate**
  - **Temperature**
  - **CPI (Consumer Price Index)**
- Plotted scatterplots to visualize relationships.

### **3️⃣ Sales Trends Analysis**
- Aggregated sales data over time.
- Used `seasonal_decompose` to analyze **seasonal patterns**.

### **4️⃣ Store Performance Analysis**
- Ranked stores based on total sales.
- Identified **top-performing** and **worst-performing** stores.
- Calculated the difference between the best and worst store.

## 🔮 Sales Forecasting Using SARIMA
### **1️⃣ Stationarity Test**
- Conducted **Augmented Dickey-Fuller (ADF) Test** to check stationarity.
- Differenced data to make it stationary.

### **2️⃣ SARIMA Model**
- Used **Seasonal ARIMA (SARIMA)** with parameters `(1,1,1) x (1,1,1,52)`.
- Trained the model on historical data.
- Forecasted sales for the next **12 weeks**.

### **3️⃣ Forecast Visualization**
- Plotted historical vs. forecasted sales.
- Highlighted predicted trends.

## 📈 Results & Insights
- **Unemployment & Sales:** Weak correlation (-0.2 to 0.1)
- **CPI & Sales:** Slight positive correlation (~0.3)
- **Temperature & Sales:** No significant correlation.
- **Top Store vs. Worst Store:** Huge sales difference.
- **Forecasting:** Sales expected to follow seasonal patterns in the next 12 weeks.

## 🚀 How to Run the Project
1. **Clone the repository:**
   ```sh
   git clone https://github.com/YourGitHubUsername/walmart-sales-forecast.git
   cd walmart-sales-forecast
   ```
2. **Install dependencies:**
   ```sh
   pip install pandas numpy matplotlib seaborn statsmodels scikit-learn scipy
   ```
3. **Run the Python script (Jupyter Notebook or .py file):**
   ```sh
   jupyter notebook
   ```
   Open the notebook and execute the cells.

## 🔗 References
- Walmart Sales Dataset: [Kaggle](https://www.kaggle.com/datasets/)
- SARIMA Documentation: [Statsmodels](https://www.statsmodels.org/)

## 💡 Future Enhancements
- Incorporate external economic indicators.
- Improve SARIMA model with hyperparameter tuning.
- Deploy as an interactive dashboard.


