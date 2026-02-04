# 📊 Spatial-Temporal Deep Learning Model for Predicting PM2.5 in Sri Lankan Urban Cities

## 📌 Overview
Air pollution caused by fine particulate matter (PM2.5) is a major public health concern in Sri Lanka, especially in urban areas. This project presents a **spatial-temporal deep learning framework** to predict PM2.5 concentrations using a combination of **ground-based sensor data** and **satellite imagery**.

The proposed system integrates **temporal modeling (LSTM)** and **spatial feature extraction (CNN)** into a **hybrid CNN–LSTM model**, enabling accurate PM2.5 prediction even in regions without air quality monitoring stations.

---

## 🎯 Objectives
- Develop accurate PM2.5 prediction models using **deep learning techniques**
- Compare traditional statistical models with modern ML/DL approaches
- Integrate **satellite imagery** to estimate PM2.5 in sensor-scarce areas
- Improve air quality forecasting to support **public health and urban planning**

---

## 🗂️ Dataset
### Temporal Data
- Hourly PM2.5 measurements
- Temperature & relative humidity
- Collected from **18 monitoring stations** across Sri Lanka

### Spatial Data
- RGB satellite images (1 km × 1 km resolution)
- Resized to 224 × 224 for CNN input

### Clustering
- Stations grouped into **3 clusters** using Pearson correlation

---

## 🧠 Models Implemented

### Statistical Models
- ARIMA  
- SARIMA  
- ETS  

### Machine Learning / Deep Learning Models
- Random Forest  
- LSTM  
- GRU  
- CNN (VGG16-based transfer learning)  
- **Hybrid CNN–LSTM (Proposed Model)**  

---

## 🔧 Methodology
1. Data collection from sensor networks and satellite sources  
2. Data preprocessing (outlier detection, imputation, normalization)  
3. Station clustering using correlation analysis  
4. Temporal modeling using LSTM  
5. Spatial feature extraction using CNN (VGG16)  
6. Feature enhancement using:
   - Green Index
   - Urban Index
   - Near Road Index
   - Seasonal zone (Dry/Wet)
   - PM2.5 lag history
7. Hybrid model creation using **linear regression fusion** of CNN & LSTM outputs  

---

## 🏗️ Hybrid Model Architecture
- **CNN** extracts spatial features from satellite images  
- **LSTM** captures temporal dependencies from historical PM2.5 data  
- Final PM2.5 prediction obtained by weighted fusion of both models  

---

## 📊 Results

| Model | R² Score |
|------|---------|
| LSTM | 41.13% |
| CNN | 69.84% |
| **Hybrid CNN–LSTM** | **86.86%** |

✔ The hybrid model achieved the **lowest prediction error** and **highest accuracy**, outperforming standalone models.

---

## 🧪 Evaluation Metrics
- Mean Absolute Error (MAE)  
- Root Mean Square Error (RMSE)  
- R² (Coefficient of Determination)  

---

## 🌍 Applications
- Urban air quality monitoring  
- Public health risk assessment  
- Environmental policy planning  
- PM2.5 estimation in areas without monitoring stations  

---

## 🛠️ Technologies Used
- Python  
- TensorFlow / Keras  
- Scikit-learn  
- NumPy, Pandas, Matplotlib  
- Satellite image processing  

---

## 👨‍🎓 Authors
- **Kapilan K.**  
- **Kuganthan N.**  
- **Thanujan I.**  

Department of Electrical and Electronic Engineering  
Faculty of Engineering  
University of Peradeniya, Sri Lanka  

---

## 📌 Acknowledgements
We sincerely thank the University of Peradeniya, our supervisors, and the organizations that provided air quality and satellite datasets for supporting this research.

---

## 📜 License
This project is intended for **academic and research purposes only**.
