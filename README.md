# Crime Hotspot Prediction: A Spatio-Temporal AI Approach

## Project Overview
This project focuses on developing a **Spatio-Temporal framework** to predict urban crime hotspots. By identifying high-risk zones through historical data, the system enables law enforcement to transition from reactive to proactive policing. The study evaluates the effectiveness of merging traditional Machine Learning with Deep Learning architectures.

## Modeling & Methodology
The project implements a comparative analysis between two powerful architectures:
1. **XGBoost (Gradient Boosting):** Leveraged as a high-efficiency baseline to capture spatial trends and temporal patterns.
2. **ConvLSTM (Convolutional LSTM):** An advanced Deep Learning model designed to process grid-based spatio-temporal data, capturing complex dependencies that traditional models might miss.

## 📊 Performance: Spatial Tolerance Analysis
Standard accuracy is often misleading in crime prediction. Therefore, this project evaluates performance using **Spatial Relaxed Accuracy (Neighbor Evaluation)**.
* **Strict Accuracy:** Requires the prediction to be in the *exact* grid cell (Too restrictive).
* **Spatial Accuracy (Used Here):** A prediction is considered **Correct (True Positive)** if the crime occurs in the predicted grid **OR any of its 8 neighboring grids**.

| Metric | XGBoost (Spatial) | ConvLSTM (Spatial) |
| :--- | :--- | :--- |
| **Spatial Precision** | 84% | 73% |
| **Spatial Recall** | 97% | 96% |
| **F1-Score** | 0.90 | 0.83 |

> *Note: The results above demonstrate that using a spatial tolerance window significantly increases the model's practical utility for police patrol planning.*

## Repository Contents
* `Crime_Hotspot_Prediction.ipynb`: The complete Python implementation, including data preprocessing, feature engineering, and model training (XGBoost & ConvLSTM).
* `Crime_Hotspot_Prediction_Report.pdf`: A comprehensive technical report detailing the methodology, mathematical framework, and comparative results.

## Tech Stack
* **Languages:** Python
* **ML/DL Frameworks:** XGBoost, TensorFlow, Keras
* **Data Science:** Pandas, NumPy, Scikit-learn

## Future Directions
* Integrating external datasets (Socioeconomic indicators, Weather, and Urban mobility).
* Implementing **Explainable AI (XAI)** to help law enforcement understand the "Why" behind the predictions.
* Scaling the model for real-time streaming data.

## Author
* **Muhannad Alraddadi** - Data Scientist / ML Developer

## License
This project is licensed under the **MIT License**.
