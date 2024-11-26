# Enhancing-Data-Center-Operations-with-Machine-Learning-Addressing-Missing-Resource-Usage-Data

## Project Overview
This project focuses on predicting and classifying resource usage data in a data center using machine learning. The dataset contains information about jobs, resource consumption, and usage patterns. The aim is to develop predictive models to classify resource usage accurately, which can help in monitoring and optimizing data center operations.

The project involves:
- Data preprocessing and feature engineering to handle missing values and ensure data integrity.
- Application of classification algorithms, including Logistic Regression, Random Forest, and Support Vector Machines (SVM).
- Visualization of results to evaluate and compare model performance.
- Analysis of the most effective model based on accuracy, recall, precision, F1-score, and AUC-ROC curves.

---

## Dataset Details
The dataset contains the following columns:
- **`job_id`**: Unique identifier for each job.
- **`host`**: The host machine on which the job ran.
- **`timestamp`**: Timestamp of the resource usage log.
- **`block`**: Block ID associated with the job.
- **`cpuuser`**: CPU usage by the user.
- **`gpu_usage`**: GPU usage during the job execution.
- **`memused`**: Total memory used.
- **`memused_minus_diskcache`**: Memory used excluding disk cache.
- **`nfs`**: Network file system usage.
- **`ts_delta`**: Time difference between consecutive entries.
- **`row_id`**: Row identifier.

The target variable for this project was created to classify resource usage patterns.

---

## Methodology
### 1. Data Preprocessing
- Merged multiple datasets to form a unified dataset.
- Addressed missing values using imputation techniques.
- Scaled features for better performance with machine learning models.

### 2. Exploratory Data Analysis
- Visualized data distributions using histograms and scatter plots.
- Plotted feature correlations to understand relationships.

### 3. Modeling
- Three machine learning models were implemented: Logistic Regression, Random Forest, and Support Vector Machine (SVM).
- Training and testing accuracies were calculated to assess performance and generalization.
- AUC-ROC curves were plotted to visualize model performance in distinguishing between classes.

### 4. Evaluation Metrics
- **Accuracy**
- **Precision, Recall, F1-Score**
- **AUC-ROC Curve**

---

## Results

### Logistic Regression
- **Accuracy**: 97%
- **Classification Report**:
  - Precision: 97% (weighted average)
  - Recall: 97% (weighted average)
  - F1-Score: 97% (weighted average)

### Random Forest
- **Accuracy**: 100%
- **Classification Report**:
  - Precision: 100% (weighted average)
  - Recall: 100% (weighted average)
  - F1-Score: 100% (weighted average)

### Support Vector Machine (SVM)
- **Accuracy**: 99%
- **Classification Report**:
  - Precision: 99% (weighted average)
  - Recall: 99% (weighted average)
  - F1-Score: 99% (weighted average)

---

## Model Comparison
- **Random Forest** outperformed other models with perfect accuracy and classification metrics. It exhibited no overfitting and provided excellent generalization.
- **SVM** achieved 99% accuracy and showed robust performance across metrics.
- **Logistic Regression** demonstrated strong performance with 97% accuracy, making it a simpler and efficient model for real-time applications.

### AUC-ROC Curves
AUC-ROC curves for each model were plotted to compare their performance in distinguishing between classes. Random Forest had the highest AUC, followed by SVM and Logistic Regression.

---

## Business Use Case
Efficient resource usage management is critical for data centers, as it directly impacts operational costs, performance, and sustainability. This project provides significant business value in the following ways:

1. **Operational Efficiency**:
   - Accurate classification of resource usage enables proactive management of workloads, preventing resource bottlenecks and over-utilization.

2. **Cost Optimization**:
   - Identifying underutilized or overutilized resources helps in reallocation and scaling decisions, reducing unnecessary operational expenses.

3. **Improved Decision-Making**:
   - Data-driven insights into resource patterns support better scheduling and allocation strategies, improving the reliability of data center services.

4. **Sustainability**:
   - Efficient resource utilization reduces energy consumption and carbon footprint, aligning operations with environmental goals.

5. **Fault Prevention**:
   - Predicting abnormal usage patterns allows for early detection of potential issues, minimizing downtime and maintaining service-level agreements (SLAs).

By implementing the models developed in this project, businesses can achieve enhanced resource management, better service delivery, and significant cost savings.

---

## Conclusion
The project successfully implemented and evaluated multiple classification models for resource usage prediction in data centers. Random Forest emerged as the best-performing model, offering a balance of simplicity, robustness, and accuracy.



## Repository Contents
- **`data/`**: Contains the dataset used in the project.
- **`notebooks/`**: Jupyter notebooks with code for preprocessing, EDA, modeling, and visualization.
- **`results/`**: Contains the output metrics, plots, and AUC-ROC curves.
- **`README.md`**: Project documentation.

Feel free to explore the repository and contribute!
