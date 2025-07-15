# 🪙 Gold Price Prediction (1833–2024)

This project aims to predict future gold prices using historical monthly data and compare different modeling techniques including:

- 🔹 Linear Regression  
- 🔹 Random Forest Regressor  
- 🔹 LSTM (Deep Learning)

---

## 📊 Dataset
- **Source**: Historical monthly gold prices
- **Time range**: 1833–2024
- **Columns**: `Date`, `Price`

---

## ⚙️ Features
- Lag features: `Price_1`, `Price_2`, `Price_3`  
- LSTM input: sequences of last 3 months  
- Data normalized for deep learning  
- 80/20 time-series train/test split (no shuffle)

---

## 🧠 Models & Evaluation

| Model             | MAE ↓    | RMSE ↓   | R² ↑     | MAPE ↓   |
|------------------|----------|----------|----------|----------|
| LinearRegression | **24.1** | **38.9** | Good     | —        |
| RandomForest     | 431.7    | 693.8    | ❌ -0.179 | 29.5%    |
| LSTM             | Medium   | Medium   | OK       | OK       |

---

## 📈 Visualizations
All models’ predictions were plotted against real prices.  
- Linear Regression performed best overall.  
- Random Forest struggled with variance (flat predictions).  
- LSTM showed promise and can improve with more sequence length or features.

---

## 📦 Libraries Used
- `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `tensorflow.keras`

---

## 🔧 Future Improvements
- Increase sequence length (e.g. 12 months)
- Add technical indicators or external economic data
- Use models like XGBoost, ARIMA, or Transformer-based models

---



# 🪙 پیش‌بینی قیمت طلا (1833 تا 2024)

این پروژه با هدف پیش‌بینی قیمت آینده طلا طراحی شده و سه مدل مختلف روی داده‌های ماهانه تاریخی مقایسه شده‌اند:

- 🔹 رگرسیون خطی (Linear Regression)  
- 🔹 جنگل تصادفی (Random Forest Regressor)  
- 🔹 شبکه عصبی LSTM (یادگیری عمیق)

---

## 📊 دیتاست
- **منبع**: قیمت ماهانه تاریخی طلا  
- **بازه زمانی**: 1833 تا 2024  
- **ستون‌ها**: `Date`، `Price`

---

## ⚙️ ویژگی‌ها
- استفاده از ویژگی‌های گذشته: `Price_1`، `Price_2`، `Price_3`  
- ورودی LSTM شامل ۳ ماه آخر  
- نرمال‌سازی داده برای مدل‌های یادگیری عمیق  
- تقسیم داده به نسبت 80/20 بدون تصادفی‌سازی (شبه سری زمانی)

---

## 🧠 مدل‌ها و ارزیابی

| مدل               | MAE ↓     | RMSE ↓    | R² ↑       | MAPE ↓   |
|-------------------|-----------|-----------|------------|----------|
| LinearRegression  | **24.1**  | **38.9**  | خوب        | —        |
| RandomForest      | 431.7     | 693.8     | ❌ منفی     | 29.5٪    |
| LSTM              | متوسط     | متوسط     | قابل قبول  | قابل قبول|

---

## 📈 نمودارها
پیش‌بینی‌های تمام مدل‌ها با قیمت واقعی مقایسه و رسم شده‌اند.  
- **Linear Regression** بهترین عملکرد را داشته  
- **Random Forest** در پیش‌بینی نوسانات ضعف نشان داده  
- **LSTM** پتانسیل بالایی داشته و با داده یا ویژگی بیشتر بهتر خواهد شد

---

## 📦 کتابخانه‌های استفاده شده
`pandas`، `numpy`، `matplotlib`، `scikit-learn`، `tensorflow.keras`

---
