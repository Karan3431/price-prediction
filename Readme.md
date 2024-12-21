# **Price Prediction using LSTM**  
[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)  

This repository contains a project on price prediction using Long Short-Term Memory (LSTM) networks. The dataset is sourced from a government website, preprocessed, and used to train an LSTM model for time-series price prediction. The project includes data visualization through heat maps, pair plots, box plots, price trends, rolling means, and distribution plots.

---

## **Table of Contents**
1. [Dataset](#dataset)  
2. [Data Collection and Preparation](#data-collection-and-preparation)  
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
4. [LSTM Model](#lstm-model)  
5. [Results](#results)  
6. [Installation and Usage](#installation-and-usage)  
7. [Project Structure](#project-structure)  
8. [Acknowledgments](#acknowledgments)  

---

## **Dataset**
- The dataset is sourced from a government website and contains historical price data till 2022.  
- It was cleaned and arranged into a suitable format for time-series analysis using Python.

---

## **Data Collection and Preparation**
- The script `datacollecting_and_arranging.ipynb` is used for:  
  1. Loading raw data from the government website.  
  2. Cleaning, handling missing values, and formatting the data.  
  3. Preparing it for exploratory data analysis (EDA) and training.  

---

## **Exploratory Data Analysis (EDA)**
The EDA includes:  
- **Heat Maps**: To visualize correlations between variables.  
- **Pair Plots**: For relationship visualization between features.  
- **Box Plots**: To identify outliers.  
- **Price Trend Analysis**: Visualized using rolling means.  
- **Distribution Plots**: To examine feature distributions.

---

## **LSTM Model**
The LSTM model is designed to predict future prices based on historical data.  

### **Model Details**
- **Input Layer**: Time-series formatted data.  
- **Hidden Layers**: Multiple LSTM layers with dropout for regularization.  
- **Output Layer**: Predicts the price for the next time step. 

### **Training**  
- Trained using a sequential model from Keras.  
- The dataset is split into training and testing sets, with early stopping implemented to prevent overfitting.  
- Model: "sequential"
 Total params: 30,651 (119.73 KB)
 Trainable params: 30,651 (119.73 KB)
 Non-trainable params: 0 (0.00 B)

---

## **Results**
- **Performance**: Achieved **96% accuracy**.  
- **Plots**:  
  1. Training vs Validation Loss graph.  
  2. Predicted vs Actual Prices for the test set.  
  3. Price trends with rolling mean.

---

## **Installation and Usage**
1. Clone the repository:  
   ```bash
   git clone https://github.com/Karan3431/price-prediction.git
   cd price-prediction
