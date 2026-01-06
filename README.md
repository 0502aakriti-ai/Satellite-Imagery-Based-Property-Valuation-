

# Multimodal Real Estate Price Prediction

This project implements a **multimodal regression pipeline** to predict real estate prices by combining **tabular housing data** with **satellite imagery**.  
The objective is to enhance traditional price prediction models by incorporating visual environmental context such as neighborhood layout, green cover, and surrounding infrastructure.

---

## 📌 Project Overview

Traditional real estate valuation models rely mainly on structured attributes like square footage, number of bedrooms, and location coordinates. However, such features often fail to capture external visual factors that influence property value.

In this project:
- A **tabular-only baseline model** is first developed using structured housing features.
- Satellite images corresponding to property latitude and longitude are programmatically fetched.
- A **Convolutional Neural Network (CNN)** is used to extract visual embeddings from satellite images.
- Tabular and visual features are fused to build a **multimodal regression model**.
- The performance of both approaches is compared using standard regression metrics.

---

## 📂 Repository Structure
├── multimodal_project.ipynb # Downloading satellite images using API, Data Loading, cleaning, EDA, Feature engineering, Model training, multimodal fusion, and evaluation

├── final_predictions.csv # Final predictions on the test dataset

├── images/ # Stored satellite images (optional / sample only)

├── requirements.txt # Python dependencies

└── README.md # Project documentation





---

## 🧠 Methodology

1. **Exploratory Data Analysis (EDA)**  
   - Analysis of price distribution  
   - Correlation analysis of numerical features  
   - Visualization of sample satellite images  

2. **Baseline Model (Tabular Data Only)**  
   - Features: bedrooms, bathrooms, square footage, condition, grade, etc.  
   - Model: Random Forest Regressor  

3. **Image Feature Extraction**  
   - Satellite images processed using a pre-trained CNN  
   - High-level visual embeddings extracted  

4. **Multimodal Fusion**  
   - Concatenation of tabular features and image embeddings  
   - Regression model trained on combined feature space  

5. **Evaluation**  
   - Metrics: RMSE and R² Score  
   - Performance comparison between tabular-only and multimodal models  

---

## 📊 Evaluation Metrics

- **Root Mean Squared Error (RMSE)**
- **R² Score**

| Model | RMSE | R² |
|----|------|------|
| Tabular model | ~215035.95| 0.6315 |
| Multimodal model | 142966.95 | -0.9740 |


The tabular-only model serves as a strong baseline, while the multimodal model demonstrates the feasibility and challenges of integrating visual context into price prediction.

---

## ▶️ How to Run the Project

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-name>



