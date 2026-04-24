# 🌍 AirCast: Cross-City Air Quality Prediction & Spike Analysis

## 🧠 Problem Statement
Air pollution, especially **PM2.5**, poses serious health risks. Most models perform well only within a single city and fail to generalize.

AirCast addresses these challenges by:
- Building a deep learning model that generalizes across multiple cities  
- Performing spike-aware analysis to better capture high-pollution events 
- Evaluating performance beyond averages using percentile-based metrics

---

## 🧩 Solution Overview

- 📥 **Data Preprocessing**
  - Cleaned and normalized PM2.5 time-series data  
  - Handled missing values  
  - Extracted temporal features (hour, day, trends)

- 🔄 **Sequence Creation**
  - Converted data into sequences using sliding windows  
  - Enabled time-series learning  

- 🧠 **Model Architecture**
  - Implemented LSTM/GRU networks  
  - Captured short-term and long-term dependencies  

- 🌐 **Cross-City Generalization**
  - Trained on one/multiple cities  
  - Tested on unseen cities  
  - Reduced overfitting to city-specific patterns  

- ⚡ **Spike Analysis**
  - Focused on high pollution events:
    - 90th percentile → high spikes  
    - 95th percentile → extreme spikes  
  - Evaluated model performance specifically on these ranges  

- 📊 **Baseline Comparison**
  - Compared with naive baseline (previous timestep prediction)  
  - Ensured meaningful improvement  

- 📈 **Evaluation Metrics**
  - RMSE → overall performance  
  - MAE → robust error  
  - 90th percentile error → high pollution  
  - 95th percentile error → extreme pollution  

- 🔍 **Insights**
  - Single-city models fail on unseen cities ❌  
  - Cross-city training improves robustness ✅  
  - Spike-based evaluation reveals real-world performance
    
---

## ⭐ Key Highlights

- 🌐 Cross-city generalization ensures robust performance on unseen cities  
- ⚡ Spike-focused prediction captures extreme pollution events (90th & 95th percentile)  
- 📊 Evaluation goes beyond averages to focus on high-risk conditions  
- 🧠 LSTM model effectively learn temporal pollution patterns  
- 🔄 Comparative analysis between same-city and cross-city scenarios  
- 📉 Baseline benchmarking validates real model improvements  
- 🚀 Designed for real-world deployment in smart city systems  
- 📈 Improves reliability during critical pollution spikes  

---

## 📥 Dataset & Preprocessing

- Multi-city PM2.5 time-series data used  
- Missing values handled and data normalized  
- Time features (hour/day) extracted  
- Converted to sequences using sliding window  
- Train-test split with cross-city evaluation  

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

## 📈 Model Performance

- Achieved strong performance on unseen cities (cross-city generalization)  
- Reduced prediction error compared to baseline models  
- Maintained accuracy during high pollution events  
- Effectively captured extreme spikes (90th & 95th percentile)  
- Provided more reliable results beyond average metrics  

### 📊 Evaluation Metrics

- RMSE for cross city: 3.5365696953559866
- MAE for cross city: 1.94146450068332 
- R² Score: 0.9839843982219774 

---

## 🔍 Key Insights

- Single-city models fail to generalize to unseen cities  
- Cross-city training significantly improves robustness  
- Average metrics can hide poor performance on spikes  
- Spike-focused evaluation reveals real-world reliability  
- Extreme pollution events are harder but critical to predict  

---

## 📌 Sample Prediction Output
<img src="https://github.com/user-attachments/assets/69b6e9f5-fc17-45ca-ba50-6348e413578e" width="500"/>

<img src="https://github.com/user-attachments/assets/21f67831-d398-4342-b72f-bb7aa5f09af2" width="500"/>

<img src="https://github.com/user-attachments/assets/fcce7fae-9d8b-49e4-91d7-37e34a7a5b24" width="500"/>

<img src="https://github.com/user-attachments/assets/ab4c1376-7a15-49b4-ba0c-2d3c299997fe" width="500"/>

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
Data Preprocessing  
↓  
Feature Engineering  
↓  
Sequence Creation  
↓  
Model Training (LSTM/GRU)  
↓  
Cross-City Evaluation  
↓  
Spike Analysis  
↓  
Performance Evaluation  
↓  
Insights  
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

- Monitor model performance on real-time data  
- Retrain model periodically with new city data  
- Handle data drift and seasonal changes  
- Optimize API latency and scalability  
- Add alert system for high pollution spikes  
  
## 👩‍💻 Author  

**Kushali Gupta**  

---

## ⭐ Support  
If you found this project useful, consider giving it a ⭐ on GitHub!  
