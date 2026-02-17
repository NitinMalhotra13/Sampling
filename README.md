# Sampling Assignment – Credit Card Fraud Analysis

---

## Objective
The objective of this assignment is to understand the importance of sampling techniques in handling imbalanced datasets and to analyze how different sampling strategies affect the performance of various machine learning models.

---

## Dataset
The dataset `Creditcard_data.csv` contains records of credit card transactions:

- **Class = 0 → Normal Transaction**
- **Class = 1 → Fraud Transaction**

The dataset is highly imbalanced, meaning fraud cases are very few compared to normal transactions. This imbalance can significantly reduce model performance if not handled properly.

---

## Data Preprocessing
To address class imbalance, **Random Undersampling** was applied:

- Majority class samples were reduced.
- Minority class samples were retained.
- The final dataset became balanced with an equal number of normal and fraud transactions.

---

## Sampling Methods Used
Five sampling techniques were applied to the balanced dataset:

- **Simple Random Sampling**
- **Systematic Sampling**
- **Stratified Sampling**
- **Cluster Sampling**
- **Bootstrap Sampling**

Each sampling method generated a separate dataset for training and evaluation.

---

## Machine Learning Models Applied
The following five machine learning models were used:

- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**

---

## Methodology
1. Load the dataset.  
2. Balance the dataset using Random Undersampling.  
3. Apply five sampling techniques to the balanced dataset.  
4. Split each sampled dataset into training and testing sets.  
5. Train five machine learning models on each sampled dataset.  
6. Evaluate model performance using **Accuracy**.  
7. Store the results in a comparison table.  
8. Generate a visualization graph using average accuracy.  

---

## Result Table

| Model | Simple Random | Systematic | Stratified | Cluster | Bootstrap |
|------|--------------|-----------|-----------|---------|-----------|
| **Logistic Regression** | 80.00 | 66.67 | 60.00 | 100.00 | 100.00 |
| **Decision Tree** | 80.00 | 33.33 | 60.00 | 100.00 | 100.00 |
| **Random Forest** | 60.00 | 33.33 | 20.00 | 66.67 | 100.00 |
| **KNN** | 60.00 | 33.33 | 20.00 | 100.00 | 66.67 |
| **SVM** | 60.00 | 33.33 | 60.00 | 100.00 | 66.67 |

---

## Result Visualization
A bar chart was created using the average accuracy of all models for each sampling method.  
The visualization is saved as `results.png` in the repository.

---

## Observations
- **Cluster Sampling** achieved the highest accuracy for most models.  
- **Bootstrap Sampling** showed strong and stable performance.  
- **Systematic Sampling** consistently produced the lowest accuracy.  
- **Simple Random Sampling** provided moderate and stable results.  
- Logistic Regression and Decision Tree were the most consistent models overall.  

---

## Conclusion
This assignment demonstrates that sampling techniques significantly influence machine learning performance when working with imbalanced datasets.  
Balancing the dataset before applying sampling methods ensures a fair comparison among models.  

Among all techniques, **Cluster Sampling** and **Bootstrap Sampling** produced the most reliable and higher accuracies, while **Systematic Sampling** yielded the weakest performance. Selecting an appropriate sampling strategy is therefore crucial in fraud detection and other imbalanced classification problems.

---

## Repository Contents
- `sampling.ipynb` – Jupyter Notebook with full implementation  
- `Creditcard_data.csv` – Dataset  
- `results.png` – Accuracy visualization graph  
- `README.md` – Project documentation  

---
