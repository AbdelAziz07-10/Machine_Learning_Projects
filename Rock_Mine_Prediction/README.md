# Sonar Rock vs Mine Classification

A machine learning project that classifies underwater objects as rocks or mines using sonar signal data.

## Overview

This project uses logistic regression to analyze sonar frequency data and distinguish between rocks and metal mines. The model processes 60 frequency band measurements to make predictions.

## Dataset

- **Source**: Sonar dataset with 208 samples
- **Features**: 60 numerical columns representing sonar frequency bands (0.0-1.0)
- **Target**: Binary classification (R = Rock, M = Mine)
- **Classes**: 111 Rocks, 97 Mines

## Features

- Data preprocessing with outlier detection and removal using IQR method
- Feature standardization using StandardScaler
- Logistic regression classification model
- Comprehensive model evaluation with accuracy metrics
- Data visualization including PCA, feature importance, and confusion matrix
- Sample prediction functionality

## Requirements

```
numpy
pandas
scikit-learn
matplotlib
seaborn
```

## Usage

1. **Install dependencies**:
   ```
   pip install numpy pandas scikit-learn matplotlib seaborn
   ```

2. **Run the main classification script**:
   ```
   python sonar_classification.py
   ```

3. **Generate visualizations**:
   ```
   python sonar_visualization.py
   ```

## Model Performance

- Training Accuracy: ~85-90%
- Test Accuracy: ~80-85%
- Uses 80/20 train-test split with stratification

## Key Components

**Data Preprocessing**:
- Duplicate removal
- IQR-based outlier detection and removal
- Feature standardization

**Model Training**:
- Logistic regression with 1000 max iterations
- Stratified train-test split
- Feature importance analysis

**Visualizations**:
- Class distribution
- Frequency response patterns
- Confusion matrix heatmap
- PCA 2D projection
- Feature importance ranking
- Model performance comparison

## How It Works

1. Load sonar frequency data (60 measurements per sample)
2. Clean data by removing duplicates and outliers
3. Standardize features for optimal model performance
4. Train logistic regression classifier
5. Evaluate model accuracy and generate predictions
6. Visualize results and feature importance

## Sample Prediction

The model can classify new sonar readings by:
1. Scaling input data using the trained scaler
2. Making prediction using the trained model
3. Providing confidence scores for the classification
