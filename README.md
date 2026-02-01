# Crime Hotspot Prediction: A Spatio-Temporal AI Approach

## Project Overview
This project focuses on developing a **Spatio-Temporal framework** to predict urban crime hotspots. By identifying high-risk zones through historical data, the system enables law enforcement to transition from reactive to proactive policing. The study evaluates the effectiveness of merging traditional Machine Learning with Deep Learning architectures.

## Modeling & Methodology
The project implements a comparative analysis between two powerful architectures:
1. **XGBoost (Gradient Boosting):** Leveraged as a high-efficiency baseline to capture spatial trends and temporal patterns.
2. **ConvLSTM (Convolutional LSTM):** An advanced Deep Learning model designed to process grid-based spatio-temporal data, capturing complex dependencies that traditional models might miss.

## Performance & Insights
* **Top Performer:** In the hotspot evaluation ($K=15\%$), **XGBoost** demonstrated superior predictive power and computational speed, making it the optimal choice for real-world deployment.
* **Spatial Intelligence:** The models successfully identified risk clusters, providing a data-driven map for resource allocation and patrol planning.
* **Balanced Evaluation:** Performance was measured using spatial metrics to ensure the results align with actual law enforcement requirements.

## Repository Contents
* `Crime_Hotspot_Prediction.ipynb`: The complete Python implementation, including data preprocessing, feature engineering, and model training (XGBoost & ConvLSTM).
* `Crime_Hotspot_Prediction_Report.pdf`: A comprehensive technical report detailing the methodology, mathematical framework, and comparative results.

## Tech Stack
* **Languages:** Python
* **ML/DL Frameworks:** XGBoost, TensorFlow, Keras
* **Data Science:** Pandas, NumPy, Scikit-learn
* **Analysis:** Spatio-Temporal Evaluation Metrics

## Future Directions
* Integrating external datasets (Socioeconomic indicators, Weather, and Urban mobility).
* Implementing **Explainable AI (XAI)** to help law enforcement understand the "Why" behind the predictions.
* Scaling the model for real-time streaming data.

## Author
* **Your Name** - Data Scientist / ML Developer

## License
This project is licensed under the **MIT License**.
