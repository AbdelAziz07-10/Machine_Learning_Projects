# Breast Cancer Logistic Regression

This project applies Logistic Regression to the Breast Cancer Wisconsin dataset for binary classification (Benign vs Malignant).

## Project Structure
- **Data Preprocessing**  
  - Check for null values and duplicates  
  - Drop unnecessary columns (`id`, `Unnamed: 32`)  
  - Encode target variable (`diagnosis`: M=1, B=0)  
  - Standardize features  

- **Exploratory Data Analysis (EDA)**  
  - Dataset statistics and distributions  
  - Outlier detection using IQR  
  - Class distribution visualization  

- **Model Training**  
  - Logistic Regression with training and testing split  
  - Performance metrics: Accuracy, Classification Report  

- **Evaluation**  
  - Residual analysis  
  - Confusion Matrix visualization  
