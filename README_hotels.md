# 📊 Hotel Booking Optimization Project

### **Objective**  
Analyze hotel customer and  hotel booking  dataset to build a machine learning model that predicts which booking is likely to be cancelled.  

---

## 💡 Problem Statement 
The cancellation of bookings impact a hotel on various fronts:
* Loss of resources (revenue) when the hotel cannot resell the room.
* Additional costs of distribution channels by increasing commissions or paying for publicity to help sell these rooms.
* Lowering prices last minute, so the hotel can resell a room, resulting in reducing the profit margin.

## Objective
The increasing number of cancellations calls for a Machine Learning based solution that can help in predicting which booking is likely to be canceled. 

## Project Scope
* Analyze the data provided to find which factors have a high influence on booking cancellations
* Build a predictive model that can predict which booking is going to be canceled in advance
* Help in formulating profitable policies for cancellations and refunds

---

## 🔧 Project Pipeline  
1. **Data Cleaning & Preprocessing**  
   - Handled missing values and outliers.
   - Encoded categorical variables (Cancelled and Not Cancelled Class).
   - Scaled numerical features for machine learning compatibility.

2. **Exploratory Data Analysis (EDA)**  
   - Identified trends and patterns in booking data.
   - Analyzed the impact of features like no of adults, children, night of stay, lead time, source of booking, arrival month, average price per room, no of prvious cancellation, and repeated visits.

3. **Model Building**  
   - Built and tuned classification models such as Logistic Regression and Decision Tree.  
   - Selected the best-performing model based on precision, recall, and F1-score.

4. **Recommendations**  
   - Leverage EDA and model insights to provide recommedations that can reduce booking cancelation.

---

## 📂 Repository Contents  
- **`data/`**: Contains raw and cleaned datasets.  
- **`notebooks/`**: Step-by-step Jupyter notebooks for data cleaning, EDA, modeling, and recommendations.  
- **`models/`**: Saved predictive models and preprocessing tools.  
- **`images/`**: Visualizations from EDA and model results.  

---

## 📊 Exploratory Data Analysis Highlights  
- **Key Finding 1**: Online booking was the most common and also is the source of highest cancellation.  
- **Key Finding 2**: More data required to learn booking patterns during the busy months (including October -the busiest), This can provide valuable insights into the reasons behind increased cancellations during this period. 
- **Key Finding 3**: Key variables influencing cancellations included lead time, market segment (online), number of special requests, and average price per room. 

<p align="center">
  <img src="images/feature_importance.png" alt="Feature Importance" width="600">
</p>

---

## 🤖 Model Performance  
The final model - Pruned Decision Tree achieved the following metrics:
- **Accuracy**: 88%  
- **Precision**: 80%  
- **Recall**: 83%  
- **F1-Score**: 81%  

| Model               | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression at 0.37 Threshold | 80%      | 74%       | 67%    | 70%      |
| Pruned Decision Tree       | 88%      | 80%       | 83%    | 81%      |

---

## 📈 Recommendations  
The developed model accurately predicts hotel booking cancellations, achieving a 32.8% accuracy rate. 

Based on the model's insights, the following recommendations were provided:
1. **Promotions**: Introduce seasonal online promotions with locked-in rates can reduce cancellation rates for online bookings.  
2. **B2B Business**: Extend business coverage to cover and leverage B2B business areas. Corporate reservations may result in more reliable booking.  
3. **Measures**: Explore cancellation policy to include penalty payments based on proximity to arrival date, such as 100% of the first night rate for cancellations made one day before, and 75% of the room price for cancellations made two days before, can deter last-minute cancellations  

---

## 🛠 Tools & Technologies  
- **Programming Languages:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- **Visualization:** Matplotlib, Seaborn  
- **Version Control:** Git, GitHub  

---

## 🚀 How to Run the Project  
1. Clone this repository:
   ```bash
   git clone https://github.com/kemmy-dotcom/Visa-Approval-Prediction.git
