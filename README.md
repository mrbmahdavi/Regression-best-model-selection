# Regression-best-model-selection

## 🔍 Overview
This project compares the performance of five different regression algorithms on a dataset to determine the best-performing model based on R² scores. The algorithms evaluated include Multiple Linear Regression, Polynomial Linear Regression, Support Vector Regression, Decision Tree Regression, and Random Forest Regression.

## 📁 Dataset
- **Source**: UCI Machine Learning Repository
- **Features**: 
  - AT: Ambient Temperature
  - V: Exhaust Vacuum
  - AP: Ambient Pressure
  - RH: Relative Humidity
  - PE: Net Hourly Electrical Energy Output (Target Variable)
- **Characteristics**: 
  - 9568 entries
  - No missing values
  - No categorical data requiring encoding
  - All features are numerical (float64)

## 🤖 Algorithms Compared
1. **Multiple Linear Regression**
2. **Polynomial Linear Regression** (Degree = 4)
3. **Support Vector Regression** (RBF kernel)
4. **Decision Tree Regression**
5. **Random Forest Regression** (10 estimators)

## ⚙️ Implementation
The project is implemented in a Jupyter Notebook with the following structure:

1. **Data Loading and Preparation**
   - Import necessary libraries (NumPy, Pandas, Matplotlib, Scikit-learn)
   - Load and inspect the dataset
   - Prepare dataset based on the model used(e.g. using standard scaler for SVR)
   - Split data into training and testing sets (80/20 split)

2. **Model Training and Evaluation**
   - Each model is trained on the training data
   - Performance is evaluated using R² score on the test set
   - Results are stored for comparison

3. **Conclusion**
   - Comparison of R² scores across all models
   - Identification of the best-performing algorithm

## 📊 Results
The R² scores obtained for each algorithm:
- Multiple Linear Regression: 0.9301
- Polynomial Linear Regression: 0.9436
- Support Vector Regression: 0.9461
- Decision Tree Regression: 0.9288
- Random Forest Regression: 0.9606

## 🎯 Conclusion
Based on the R² scores, the **Random Forest Regression** algorithm performed the best on this dataset and should be selected for this particular regression task.

## 📋 Requirements
- Python 3
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## 🚀 Usage
1. Ensure all required libraries are installed
2. Run the Jupyter Notebook cells sequentially
3. The notebook will automatically:
   - Load and preprocess the data
   - Train and evaluate all models
   - Display the R² scores
   - Identify the best-performing algorithm

## Note
This comparison is specific to the provided dataset. For other datasets, a similar approach can be followed, but results may vary based on data characteristics.
