

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



