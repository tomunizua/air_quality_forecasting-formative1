# PM2.5 Air Quality Prediction Using LSTM

This project leverages a Recurrent Neural Network (RNN) architecture, specifically a Bidirectional Long Short-Term Memory (LSTM) model, to predict air pollution levels (PM2.5) based on multivariate time series data.

## 📌 Project Overview

Air pollution, particularly fine particulate matter (PM2.5), poses severe risks to public health. Accurate forecasting of PM2.5 levels can empower individuals and policymakers to take preventive measures. This project aims to build a deep learning model that learns temporal patterns in environmental data to forecast PM2.5 concentrations.

---

## 🧠 Model Architecture

The final model is a multi-layer Bidirectional LSTM network, designed to capture temporal dependencies in both directions. Key components include:

- **Input Layer**: Accepts sequences of historical environmental data.
- **2 Bidirectional LSTM Layers**: Capture complex temporal relationships.
- **Dense Layers**: Process the extracted features for final prediction.
- **Output Layer**: Returns a single PM2.5 value.

I performed **15+ experiments** varying:
- Number of LSTM units
- Dropout rates
- Dense layer units
- Optimizers
- Learning rates
- Batch sizes

---

## 📁 Repository Structure

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/tomunizua/air_quality_forecasting-formative1.git
   cd air_quality_forecasting-formative1.git

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt

3. **Run notebook**
   Navigate to the Google Colab notebook and run the cells accordingly

## Evaluation Metric

We use Root Mean Squared Error (RMSE) as the primary evaluation metric.
Formula:
RMSE = sqrt( (1/n) * Σ (y_i - ŷ_i)² )
Lower RMSE indicates better model performance.

## Key Findings

   
