# Molecular Property Prediction Using Machine Learning

This project applies regression algorithms to predict molecular properties from their **SMILES (Simplified Molecular Input Line Entry System)** representations.

## 📁 Project Structure

├── DATA/                      
│   ├── Only_qy_data_ML.csv
│   ├── Only_wl_data_ML.csv
│   └── Data.csv
│
├── Models/                     # Trained models and scalers
│   ├── QY_Random.pkl
│   ├── WL_Random.pkl
│   ├── scaler_model-QY.pkl
│   └── scaler_modelwl.pkl
│
├── Data_Creation.ipynb         # Data preprocessing notebook
├── Prevision.ipynb             # Prediction using trained models
├── Regression.ipynb            # Model training and learning curves
└── .gitattributes              # Git configuration


## 💡 Objective

Develop machine learning regression models to predict two molecular properties:

- **QY** (Quantum Yield)  
- **WL** (Wavelength)

The model input is only the molecule’s **SMILES** representation, enabling predictions without the need for costly quantum simulations or additional molecular descriptors.

## 🧪 Dataset

The molecular data was sourced from the public database:

🔗 [Deep4Chem Database](https://deep4chem.com/database)

## ⚙️ Models

The trained models use **Random Forest Regressors** and were saved using `joblib`:

- `QY_Random.pkl`: model for predicting QY  
- `WL_Random.pkl`: model for predicting WL  
- `scaler_model-QY.pkl` and `scaler_modelwl.pkl`: scalers used for data normalization prior to prediction

## 📊 Notebooks

- `Data_Creation.ipynb`: Preprocessing of the raw molecular data  
- `Regression.ipynb`: Model training, evaluation, and generation of learning curves  
- `Prevision.ipynb`: Loading and using the trained models to make predictions based on new SMILES inputs

## 🚀 How to Use

1. Clone this repository:

    ```bash
    git clone https://github.com/Quimica-Teorica-IME/Predicting-Fluorescence-Emission-Wavelengths-and-Quantum-Yields-via-Machine-Learning.git
    cd Predicting-Fluorescence-Emission-Wavelengths-and-Quantum-Yields-via-Machine-Learning
    ```

2. Open the Jupyter notebooks to explore data, train models, and make predictions.

## 📚 Reference & Citation

This code and data pipeline are associated with the following publication:

**Predicting Fluorescence Emission Wavelengths and Quantum Yields via Machine Learning**  
*Journal of Chemical Information and Modeling*, **2025**, *65* (7), 3270–3281  
🔗 https://doi.org/10.1021/acs.jcim.4c02403  
Published: March 20, 2025  
© 2025 The Authors. Published by the American Chemical Society. Licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0)

> If you use this repository in your work, please cite the paper accordingly.
