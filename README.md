# 📞 Call Center Data Analysis

## 📊 Overview

This repository presents an end-to-end data analysis project focused on customer interactions with a call center. Using Power BI, we've developed interactive dashboards to visualize key metrics, uncover trends, and evaluate performance indicators that drive call center efficiency and customer satisfaction.

---

## 🧾 Dataset Description

The dataset consists of **32,941** records capturing various aspects of customer interactions. Each row represents an individual call record with detailed information including call timing, customer location, reason for the call, response performance, and sentiment.

### 🔑 Key Attributes:
- `Id`: Unique identifier for each call.
- `Call Timestamp`: Date and time of the call.
- `Call-Centres City`: City where the call center is located.
- `Channel`: Mode of interaction (e.g., Call Center, Chatbot).
- `City`: Customer’s city of residence.
- `Customer Name`: Name of the customer.
- `Reason`: Reason for the call (e.g., Billing Question, Payments).
- `Response Time`: Service level (e.g., Within SLA, Above SLA).
- `Sentiment`: Customer sentiment (e.g., Neutral, Negative, Very Positive).
- `State`: Customer’s state of residence.
- `Call Duration In Minutes`: Duration of the call.
- `Csat Score`: Customer Satisfaction Score (1–10; includes missing values).

---

## 🧭 Dashboard Structure

### 🏠 Home Dashboard

#### 🔢 Key Metrics:
- **Total Calls**: 32.9K
- **Total Call Duration (Hours)**: 13.74K
- **Average Call Duration (Minutes)**: 25.02
- **Response Time (% within SLA)**: 75.26%

#### 📊 Visualizations:
- **Calls by Day**: Bar chart showing number of calls by weekday
- **Calls by City**: Line chart showing call distribution across cities
- **Calls by Reason**: Stacked bar chart categorizing reasons for calls
- **Calls by Channel**: Pie chart showing distribution by communication medium
- **Calls by Sentiment**: Bar chart showing customer sentiment distribution

---

### 🧮 Grid Dashboard

#### 🔢 Key Metrics:
- **Total Calls**: 16.3K
- **Total Call Duration (Hours)**: 6.84K
- **Average Call Duration (Minutes)**: 25.07
- **Response Time (% within SLA)**: 75.43%

#### 📋 Tabular View:
An interactive table displaying call records with:
- Customer Name
- Channel
- State
- Reason
- Response Time
- City
- Call Duration

---

## 🔄 Data Transformations & DAX Queries

### 🔧 Transformations:
- **Slicers** for:
  - Date
  - Channel
  - City
- **Calculated Fields** for:
  - Total Calls
  - Total Call Duration
  - Average Call Duration
  - SLA Response Rate

### 🧠 Sample DAX Query:
```DAX
AvgCallDurationByChannel =
CALCULATE(
    AVERAGE('Call Details'[Avg Call Duration]),
    VALUES('Call Details'[Channel])
)
```

## 🖱️ Interactive Features

### 🎛️ Filters:
- **Date Range**  
- **Channel Type**  
- **Customer City**  

### 💡 Key Insights:
- **Peak days and call volumes**  
- **City-level call traffic**  
- **Most common call reasons**  
- **Sentiment trends**  
- **SLA performance**  

---

## ✅ Conclusion

This Power BI dashboard provides a comprehensive view of call center performance and customer interactions. With interactive filters and insightful visualizations, users can:
- **Monitor call volume trends**
- **Analyze sentiment and reasons for contact**
- **Improve service levels based on SLA metrics**

The dashboards help stakeholders make informed, data-driven decisions to improve operational efficiency and customer satisfaction.


---
## Dashboard Images

### Home Dashboard
![Call Center Data Analysis Dashboard](./Call%20Centre%20Analysis%20-%20Home%20Dashboard.png)

### Grid Dashboard
![Call Center Data Analysis Dashboard](./Call%20Centre%20Analysis%20-%20Grid%20Dashboard.png)
