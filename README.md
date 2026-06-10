# 🚦 Smart City Traffic Forecasting using Machine Learning

## 📌 Project Overview

Traffic congestion is one of the major challenges faced by modern urban environments. Effective traffic forecasting enables city planners and government authorities to optimize traffic signals, improve road infrastructure, reduce congestion, and enhance transportation efficiency.

This project develops a Machine Learning-based traffic forecasting system capable of predicting vehicle volume at different city junctions using historical traffic data. The solution leverages feature engineering, exploratory data analysis, and predictive modeling to identify traffic patterns and forecast future traffic conditions.

---

## 🎯 Problem Statement

As part of Smart City initiatives, governments require intelligent systems capable of analyzing and forecasting traffic behavior across multiple junctions.

The objectives of this project are:

* Analyze historical traffic patterns.
* Identify traffic trends across different junctions and time periods.
* Forecast future traffic volume.
* Support infrastructure planning and traffic management decisions.
* Provide data-driven insights for smarter urban transportation systems.

---

## 📊 Dataset Description

The dataset contains traffic observations collected from multiple city junctions over a period of time.

### Original Features

| Feature  | Description                      |
| -------- | -------------------------------- |
| DateTime | Timestamp of traffic observation |
| Junction | Junction Identifier              |
| Vehicles | Number of vehicles recorded      |

### Engineered Features

To improve model performance, additional time-based features were extracted:

* Hour
* DayOfWeek
* Month
* Year
* IsWeekend

These features help capture temporal traffic patterns and seasonal behavior.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Pickle
* Google Colab
* GitHub

---

## 🔄 Project Workflow

### 1. Data Collection

* Downloaded Smart City Traffic dataset.
* Loaded dataset using Pandas.
* Inspected dataset structure and records.

### 2. Data Preprocessing

* Converted DateTime column into datetime format.
* Generated time-based features.
* Prepared dataset for machine learning.

### 3. Exploratory Data Analysis (EDA)

Traffic trends were analyzed through visualizations:

* Average Traffic by Hour
* Traffic Distribution Across Junctions
* Weekday vs Weekend Traffic Analysis

Key observations:

* Traffic volume varies significantly based on time of day.
* Different junctions experience different traffic intensities.
* Weekend traffic patterns differ from weekday traffic behavior.

### 4. Feature Engineering

Extracted temporal features:

* Hour
* DayOfWeek
* Month
* Year
* IsWeekend

These engineered features significantly improved predictive performance.

### 5. Model Development

The following machine learning algorithms were evaluated:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

The dataset was split into:

* Training Data (80%)
* Testing Data (20%)

---

## 📈 Model Performance

### Evaluation Metrics

| Metric   | Score  |
| -------- | ------ |
| MAE      | 3.70   |
| RMSE     | 6.22   |
| R² Score | 0.9050 |

### Interpretation

* Average prediction error is approximately 3.7 vehicles.
* The model explains 90.5% of traffic variation.
* Low RMSE indicates strong predictive capability.

---

## 🏆 Model Comparison

| Model                   | RMSE  |
| ----------------------- | ----- |
| Linear Regression       | 12.70 |
| Decision Tree Regressor | 6.43  |
| Random Forest Regressor | 6.22  |

### Selected Model

Random Forest Regressor achieved the lowest prediction error and highest overall performance. Therefore, it was selected as the final forecasting model.

---

## 🔮 Future Traffic Forecasting Example

### Input

| Feature   | Value      |
| --------- | ---------- |
| Hour      | 18         |
| DayOfWeek | 4 (Friday) |
| Month     | 6          |
| Year      | 2017       |
| IsWeekend | 0          |
| Junction  | 3          |

### Prediction

Predicted Traffic Volume: **27 Vehicles**

This demonstrates the model's ability to forecast future traffic conditions using historical patterns.

---

## 📊 Visualizations

The following visualizations were generated:

* Traffic by Hour
* Traffic by Junction
* Weekday vs Weekend Analysis
* Actual vs Predicted Traffic
* Feature Importance Analysis (Optional Enhancement)

---

## 💾 Model Persistence

The trained model was saved using Pickle.

```python
pickle.dump(model, file)
```

Saved model file:

```text
traffic_model.pkl
```

This enables future predictions without retraining the model.

---

## 📁 Project Structure

```text
smart-city-traffic-forecasting/
│
├── README.md
├── requirements.txt
├── traffic_forecasting.ipynb
├── traffic_cleaned.csv
├── traffic_model.pkl
│
├── traffic_by_hour.png
├── traffic_by_junction.png
├── weekday_vs_weekend.png
├── model_predictions.png
│
└── assets/
```

---

## 🚀 Future Enhancements

* Hyperparameter Optimization
* Real-Time Traffic Prediction
* Streamlit Dashboard Deployment
* Traffic Congestion Alerts
* Smart Signal Recommendation System
* Integration with Smart City Infrastructure

---

## ✅ Conclusion

This project successfully demonstrates the application of Machine Learning for Smart City Traffic Forecasting.

Through data preprocessing, feature engineering, exploratory data analysis, and predictive modeling, the system effectively learned historical traffic patterns and generated accurate traffic volume forecasts.

The Random Forest Regressor achieved an R² Score of 0.9050 and an RMSE of 6.22, indicating strong predictive performance. Such forecasting systems can support government agencies and urban planners in optimizing traffic management, improving transportation infrastructure, and enhancing overall city efficiency.

---

## 👨‍💻 Author

**Jyothi Pushya**

Computer Science Student | Machine Learning Enthusiast

GitHub: https://github.com/Jyothipushya
