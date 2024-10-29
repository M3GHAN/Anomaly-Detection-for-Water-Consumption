# Anomaly Detection on Water Consumption

## Project Overview
This project applies advanced machine learning and deep learning techniques to detect anomalies in water consumption patterns over time. By identifying irregular usage events, this project aims to support effective water resource management, detecting issues such as leaks, unauthorized usage, or operational anomalies.

## Dataset Information
The dataset is time-series data that records water consumption at regular intervals. Key features include:
- **Totalizer**: The cumulative measurement of water usage over time.
- **Consumption**: The incremental usage between two time intervals, derived from the difference in totalizer values.

## Objectives
1. **Data Preparation**: Clean and preprocess water consumption data for reliable analysis.
2. **Exploratory Data Analysis (EDA)**: Examine trends, seasonal patterns, and potential outliers in water usage data.
3. **Anomaly Detection Models**:
   - Unsupervised KNN to identify outliers without labeled data.
   - Supervised KNN to classify known patterns when labeled data is available.
   - Convolutional Neural Network (CNN) for deep learning-based anomaly detection, leveraging spatial and temporal features.

## Methodology
### 1. Data Preprocessing
   - Data cleaning and missing value handling.
   - Calculation of `Consumption` values based on `Totalizer` differences to get accurate interval-based usage.

### 2. Exploratory Data Analysis (EDA)
   - Visualizations of water consumption and cumulative usage over time.
   - Identification of outliers using:
     - Box plots for detecting extreme values.
     - Rolling averages for analyzing short-term trends and variations.
     - Seasonal decomposition to capture underlying patterns in consumption.

### 3. Anomaly Detection Approaches
   - **K-Nearest Neighbors (KNN)**:
      - **Unsupervised KNN** for detecting outliers in unlabeled data based on proximity metrics.
      - **Supervised KNN** to classify labeled data into normal and anomalous classes for comparison.
   - **Convolutional Neural Network (CNN)**:
      - Applied to learn complex patterns within the water consumption data, leveraging deep learning to identify anomalies based on spatial and temporal dependencies in the dataset.

## Results and Visualization
- **Trend Analysis**: Visualized cumulative consumption to track overall usage patterns and predict future water usage.
- **Anomaly Detection**: 
   - The KNN models highlighted significant outliers and classified known patterns effectively.
   - CNN detected nuanced anomalies by learning complex data patterns, enabling more granular identification of unusual consumption.

## Conclusion
This project successfully applies both traditional machine learning and deep learning techniques to detect anomalies in water consumption, which can be critical in proactive water management, leak detection, and operational monitoring.

---

## How to Run the Project
1. Clone this repository.
2. Install the required packages listed in `requirements.txt`.
3. Open and run the Jupyter Notebook `Anomaly_Detection_on_Water_Consumption.ipynb` to see the full workflow for data analysis and anomaly detection using both KNN and CNN models.
