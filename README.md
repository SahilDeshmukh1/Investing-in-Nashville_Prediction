## Project Overview
This project focuses on analyzing and predicting property values in the Nashville area to guide real estate investment decisions. Using a combination of machine learning models, the goal is to classify properties as overvalued or undervalued and identify key factors influencing their valuation. The project delivers insights to optimize real estate investment strategies.

Key Objectives:
- Analyze property data to identify trends and patterns.
- Build predictive models (Decision Tree, Random Forest, and Gradient Boosting) to classify properties.
- Recommend the best model for accurate and actionable real estate valuation.

---

## Dataset
- **Description**: A real estate dataset for Nashville properties containing features like building value, acreage, neighborhood, and finished area.
- **Key Features**:
  - `Building Value`: Monetary value of the building.
  - `Finished Area`: Total finished square footage of the property.
  - `Acreage`: Land size of the property in acres.
  - `Neighborhood`: Location-based categorical variable.
- **Target Variable**: Classification of properties as `Overvalued` (Class 0) or `Undervalued` (Class 1).

---

## Methodology
1. **Data Cleansing**:
   - Handled missing values using median and mean imputation.
   - Renamed columns for better clarity and removed irrelevant features.
   - Addressed outliers using IQR-based filtering.

2. **Exploratory Data Analysis (EDA)**:
   - Visualized distributions and relationships between variables.
   - Checked feature importance across models to identify key factors.

3. **Machine Learning Models**:
   - **Decision Tree**: Built for simplicity and interpretability.
   - **Random Forest**: Tested for robust predictions using ensemble methods.
   - **Gradient Boosting**: Applied for high-accuracy predictions with iterative improvements.

4. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, F1-score, and ROC curve.

---

## Technologies Used
- **Python**: Data analysis, visualization, and machine learning.
- **Libraries**:
  - `pandas`, `numpy` for data manipulation.
  - `matplotlib`, `seaborn` for visualization.
  - `scikit-learn` for predictive modeling.
  - `xgboost` for Gradient Boosting implementation.

---

## Results
### Decision Tree:
- **Accuracy**: 70%
- **Key Features**: `Building Value`, `Finished Area`, `Acreage`.

### Random Forest:
- **Accuracy**: 75%
- **Key Features**: `Parcel ID`, `Legal Reference`, `Sold As Vacant`.

### Gradient Boosting:
- **Accuracy**: 76%
- **Key Features**: `Finished Area`, `Neighborhood`, `Building Value`.

### Model Recommendation:
- **Gradient Boosting** is the preferred model due to its superior balance between precision (74.91%) and recall (98.97%) for undervalued properties. It identifies `Finished Area`, `Building Value`, and `Neighborhood` as the most influential factors, making it a reliable tool for real estate investment strategy.
