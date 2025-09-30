# Stroke Prediction – Logistic Regression Model

## Project Workflow
The notebook covers:
- Reading and exploring the dataset
- Data description (head, shape, statistics, info)
- Handling missing and duplicated values
- Dropping unnecessary columns
- Encoding categorical variables
- Feature normalization and scaling
- Data visualization
- Splitting dataset into train/test
- Handling **class imbalance** to reduce bias in prediction
- Training a Logistic Regression model
- Evaluating with accuracy, metrics, and confusion matrix

## Dataset
Dataset: **healthcare-dataset-stroke-data.csv**  
Features include:
- Gender, Age, Hypertension, Heart Disease
- Marital Status, Work Type, Residence Type
- Average Glucose Level, BMI, Smoking Status  
Target: whether the person had a stroke.

## Handling Imbalance
Since the dataset is highly imbalanced (very few stroke cases compared to non-stroke),  
techniques were applied to balance the data before training.  
This improved the fairness of predictions and reduced bias.

## Results
The model was evaluated using:
- Accuracy score
- Classification metrics
- Confusion matrix  

Accuracy was reported after solving the imbalance issue, showing improved performance compared to training on raw imbalanced data.

## Requirements
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

Install with:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```
