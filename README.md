# Crop Recommendation System using Machine Learning

## Overview

This project aims to develop a **Crop Recommendation System** that leverages machine learning models to assist farmers in making data-driven decisions for crop selection. By analyzing key agricultural factors such as soil properties (nitrogen, phosphorus, potassium) and climatic conditions (temperature, humidity, rainfall, pH level), the system recommends the most suitable crops for a given set of conditions. The system utilizes two machine learning algorithms: **K-Nearest Neighbours (KNN)** and **Random Forest**, to provide accurate and reliable crop recommendations.

## Key Features

- **Data-Driven Decision Making**: Empowers farmers to make informed decisions based on objective data analysis.
- **Improved Yield and Profitability**: Recommends crops with high yield potential under specific conditions, leading to increased productivity and farm income.
- **Sustainable Farming Practices**: Promotes sustainable agriculture by recommending crops that are well-suited to the soil and climate, reducing the need for excessive fertilizers or amendments.

## Dataset

The dataset used in this project contains **2200 records** (before preprocessing) with the following features:

1. **Target Label (Crop)**: Represents the type of crop grown in a specific instance.
2. **Soil Properties**:
   - Nitrogen (N)
   - Phosphorus (P)
   - Potassium (K)
3. **Climatic Conditions**:
   - Temperature (°C)
   - Humidity (%)
   - Rainfall (mm)
   - pH Level

## Data Preprocessing

Before training the machine learning models, the dataset undergoes the following preprocessing steps:

- **Handling Missing Values**: No null values were present in the dataset.
- **Outlier Detection and Handling**: Outliers were identified and addressed to ensure data quality.
- **Feature Scaling**: Normalization or standardization was applied to ensure all features are on a common scale.

## Machine Learning Models

The project employs two machine learning algorithms for crop recommendation:

### 1. K-Nearest Neighbours (KNN)
- **Core Functionality**:
  - Calculates the distance between a new data point and each data point in the training set.
  - Identifies the K closest data points (neighbours) based on the chosen distance metric.
  - Predicts the crop class based on a majority vote among the K nearest neighbours.
- **Advantages**:
  - Interpretable and less prone to overfitting.
- **Challenges**:
  - Sensitive to the curse of dimensionality.
  - Requires careful selection of the K value.

### 2. Random Forest
- **Core Functionality**:
  - Constructs multiple decision trees during training, each built on a random subset of features and data points.
  - Predicts the crop class based on a majority vote of the individual tree predictions.
- **Advantages**:
  - High accuracy and reduced overfitting.
  - Handles missing data effectively.

## Model Performance

The performance of the machine learning models was evaluated based on their accuracy:

- **K-Nearest Neighbours (KNN)**: Achieved an accuracy of **96.34%**.
- **Random Forest**: Outperformed KNN with an accuracy of **99.69%**.

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/crop-recommendation-system.git
   cd crop-recommendation-system
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**:
   - Open the Jupyter notebook `Crop_Recommendation_System.ipynb` to explore the dataset, preprocessing steps, and model training.
   - Follow the instructions in the notebook to train the models and make crop recommendations.

4. **Run the Web Application**:
   - Navigate to the `web_app` directory.
   - Run the Flask application:
     ```bash
     python app.py
     ```
   - Access the web application in your browser at `http://127.0.0.1:5000/` to input soil and climatic conditions and receive crop recommendations.

## Future Work

- **Expand Dataset**: Include more crops and additional features such as soil texture, irrigation methods, and pest information.
- **Model Optimization**: Experiment with hyperparameter tuning and other machine learning algorithms to further improve accuracy.
- **Mobile Application**: Develop a mobile app for easier access and usability by farmers in remote areas.

## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The dataset used in this project was sourced from [Kaggle](https://www.kaggle.com/).
- Special thanks to the open-source community for providing valuable resources and tools.

---

## Author
Chaithanya Nadithoka
