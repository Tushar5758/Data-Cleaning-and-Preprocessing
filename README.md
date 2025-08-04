# Titanic Dataset - Data Cleaning and Preprocessing

This project demonstrates how to clean and preprocess raw data for Machine Learning using the Titanic dataset.

---

## Objective

Learn to handle missing values, encode categorical features, scale numerical data, remove outliers, and engineer new features — all essential steps before applying any ML algorithm.

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

---

## Steps Performed

### 1. Load Dataset
- Load `titanic.csv` using Pandas.
- Display basic info and missing values.

### 2. Handle Missing Values
- `Age`: Filled using median.
- `Embarked`: Filled using mode.
- `Cabin`: Dropped if present due to too many missing values.

### 3. Encode Categorical Variables
- `Sex`: Label encoded (`male` → 0, `female` → 1).
- `Embarked`: One-hot encoded (with `drop_first=True` to avoid multicollinearity).

### 4. Feature Engineering
- `FamilySize` = `SibSp` + `Parch` + 1
- `IsAlone` = 1 if passenger has no family on board, else 0

### 5. Drop Unnecessary Columns
- `PassengerId`, `Name`, `Ticket` removed as they're not useful for ML.

### 6. Scale Numerical Features
- Used `StandardScaler` to normalize `Age` and `Fare`.

### 7. Remove Outliers (Optional)
- Outliers in `Fare` removed using IQR method.

### 8. Visualize Correlations
- Heatmap created using Seaborn to check feature relationships.

---

## Sample Output

- Cleaned dataset 
- Correlation heatmap to visualize relationships
- Final shape of the dataset

---

## Final Dataset

The cleaned dataset is now ready for:
- Model training
- Exploratory data analysis (EDA)
- Feature importance analysis
- Deployment-ready pipelines

---

## Learning Outcomes

- Handling missing values
- Encoding techniques (Label and One-hot)
- Feature scaling using `StandardScaler`
- Simple feature engineering
- Outlier detection and removal
- Correlation analysis for ML readiness

---

