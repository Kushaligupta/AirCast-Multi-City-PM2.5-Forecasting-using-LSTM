# 🌫️ AirCast  
## Intelligent Multi-City PM2.5 Forecasting using LSTM  

> A deep learning system that forecasts air pollution trends across Indian cities, enabling data-driven environmental insights and proactive decision-making.

---

## 🧠 Problem Statement
Air pollution—especially PM2.5—is a critical public health issue in India.  
Most systems today are **reactive**, monitoring pollution after it rises.

This project focuses on **predicting PM2.5 levels in advance**, helping in:
- Early warnings  
- Policy decisions  
- Health risk reduction  

---

## 💡 Solution Overview
AirCast is an end-to-end machine learning pipeline that:
- Cleans and preprocesses raw air quality data  
- Handles missing values using **KNN Imputation**  
- Uses **LSTM (Long Short-Term Memory)** for time-series forecasting  
- Predicts PM2.5 levels across multiple cities  

---
## 🔥 Key Highlights

✔ Built a **deep learning-based time-series forecasting model (LSTM)**  
✔ Implemented **KNN Imputation** to handle missing real-world data  
✔ Designed an **end-to-end ML pipeline** from preprocessing to prediction  
✔ Worked with **multi-city air quality dataset**  
✔ Focused on a **real-world problem (air pollution)**  
✔ Structured project for **scalability and future deployment**  

---
## 📊 Dataset & Preprocessing

- Multi-city air quality dataset (India)
- Key features:
  - PM2.5, PM10  
  - NO₂, SO₂, CO  
  - Environmental indicators  

### ⚙️ Data Engineering
- Missing values handled using **KNN Imputer**  
- Data cleaned and normalized  
- Time-series structure prepared for LSTM input  

📁 Dataset Access:  
Due to GitHub size limits, the dataset is hosted externally: 
https://drive.google.com/file/d/14gHe798D0oA34RJvUI-gAFzGdyES0Fm3/view?usp=sharing

---
## 🤖 Model Architecture

- **Model Used:** LSTM (Long Short-Term Memory)
- Designed for **time-series forecasting**
- Captures **temporal dependencies** in air quality data  

### Why LSTM?
Traditional models fail to capture sequential patterns effectively.  
LSTM networks are specifically designed to:
- Learn long-term dependencies  
- Handle sequential data efficiently  
- Improve forecasting accuracy for time-series problems  

---

## 📈 Model Performance & Results

- Successfully predicted **PM2.5 trends across multiple cities**  
- Captured **seasonal and temporal variations** in pollution levels  
- Demonstrated strong generalization on unseen data  

### 📊 Evaluation Metrics

- RMSE: 3.5365696953559866
- MAE: 1.94146450068332 
- R² Score: 0.9839843982219774 

---

## 🔍 Key Insights

- Pollution levels show **strong temporal patterns**  
- Certain cities exhibit **higher volatility in PM2.5 levels**  
- Model effectively learns **trend + seasonality**  

---

## 📌 Sample Prediction Output
<img width="863" height="561" alt="image" src="https://github.com/user-attachments/assets/69b6e9f5-fc17-45ca-ba50-6348e413578e" />
<img width="887" height="475" alt="image" src="https://github.com/user-attachments/assets/21f67831-d398-4342-b72f-bb7aa5f09af2" />
<img width="859" height="487" alt="image" src="https://github.com/user-attachments/assets/fcce7fae-9d8b-49e4-91d7-37e34a7a5b24" />
<img width="653" height="433" alt="image" src="https://github.com/user-attachments/assets/ab4c1376-7a15-49b4-ba0c-2d3c299997fe" />

## ⚙️ Tech Stack

| Category        | Tools & Technologies |
|----------------|---------------------|
| Programming    | Python |
| Data Handling  | Pandas, NumPy |
| Visualization  | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Deep Learning  | TensorFlow / Keras |
| Model Type     | LSTM (Time-Series Forecasting) |

---

## 🏗️ Project Workflow

```text
Data Collection 
   ↓
Data Cleaning & Preprocessing
   ↓
Handling Missing Values (KNN Imputation)
   ↓
Feature Engineering
   ↓
Data Normalization / Scaling
   ↓
Time-Series Data Preparation
   ↓
LSTM Model Building
   ↓
Model Training & Validation
   ↓
Performance Evaluation
   ↓
PM2.5 Forecasting
```
## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
https://github.com/Kushaligupta/AirCast-Multi-City-PM2.5-Forecasting-using-LSTM.git
```

### 2️⃣ Install Dependencies
pip install -r requirements.txt

### 3️⃣ Run the Project
-Open AirCast.ipynb in:
-Jupyter Notebook
-OR VS Code
-Run all cells to reproduce results and predictions

## 📁 Project Structure  

```text
AirCast/
│
├── AirCast.ipynb              # Main notebook (data → model → results)
├── README.md                  # Project documentation
├── requirements.txt           # Dependencies
└── Dataset (external link)    # Hosted separately (Google Drive / Kaggle)
```

## 🌍 Real-World Applications  

- Air Quality Monitoring Systems  
- Smart City Analytics  
- Health Risk Prediction Platforms  
- Environmental Policy Planning  

---

## 🚀 Future Enhancements  

- Deploy using Streamlit for real-time predictions  
- Integrate live AQI APIs  
- Improve model using GRU / Transformer architectures  
- Build interactive dashboard for visualization
  
## 👩‍💻 Author  

**Kushali Gupta**  

---

## ⭐ Support  
If you found this project useful, consider giving it a ⭐ on GitHub!  
