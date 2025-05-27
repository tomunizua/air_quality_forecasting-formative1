# PM2.5 Air Quality Prediction Using LSTM

This project leverages a Recurrent Neural Network (RNN) architecture, specifically a Bidirectional Long Short-Term Memory (LSTM) model, to predict air pollution levels (PM2.5) in Beijing based on multivariate time series data.

## 📌 Project Overview

Air pollution, particularly fine particulate matter (PM2.5), poses severe risks to public health. Accurate forecasting of PM2.5 levels can empower individuals and policymakers to take preventive measures. This project aims to build a deep learning model that learns temporal patterns in environmental data to forecast PM2.5 concentrations.

---

## 🎯 Objective

To predict future PM2.5 concentrations using historical multivariate time series data through a Bidirectional LSTM model, improving forecasting accuracy with experimentation and tuning.

---

## 📊 Dataset

The dataset used for this project is the **Beijing PM2.5 Data Set**, which includes hourly air quality and meteorological data (temperature, pressure, dew point, wind speed, etc.) in csv format.

- **Features used**: PM2.5, temperature, dew point, pressure, wind speed, wind direction, and others.
- **Target variable**: PM2.5 concentration.

---

## 🧠 Model Architecture

The final model is a multi-layer Bidirectional LSTM network, designed to capture temporal dependencies in both directions. Key components include:

- **Input Layer**: Accepts sequences of historical environmental data.
- **2 Bidirectional LSTM Layers**: Capture complex temporal relationships.
- **Dense Layers**: Process the extracted features for final prediction.
- **Output Layer**: Returns a single PM2.5 value.

I performed **16 experiments** varying:
- Number of LSTM units
- Dropout rates
- Dense layer units
- Optimizers
- Learning rates
- Batch sizes

---

## 📁 Repository Structure
├── data/ # Contains the raw and preprocessed air quality datasets
├── model/ # Stores the saved model
├── outputs/ # Contains generated predictions for each experiment
├── README.md # Project overview and setup instructions
├── air_quality_forecasting_assignment.ipynb # Main notebook with code, experiments, and results
├── requirements.txt # List of Python dependencies needed to run the project

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/tomunizua/air_quality_forecasting-formative1.git
   cd air_quality_forecasting-formative1.git

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt

3. **Run notebook**
   Navigate to the Google Colab notebook and run the cells step-by-step

---

## Evaluation Metric

We use Root Mean Squared Error (RMSE) as the primary evaluation metric.
Formula:
RMSE = sqrt( (1/n) * Σ (y_i - ŷ_i)² )
Lower RMSE indicates better model performance. The goal was to reach an RMSE under 4000, though the final model fell slightly short of this benchmark.

---

### 🧪 Key Results
The best model configuration achieved an RMSE of 4358.

Systematic tuning of LSTM units, dropout, and learning rates led to gradual improvement.

Kaggle submission RMSE differed slightly due to possible differences in preprocessing or test data size.

---

## 👨‍💻 Contributors
Theodora Omunizua

---

## 📄 License
This project is for academic use. For inquiries about further use or collaboration, please contact the contributor.



