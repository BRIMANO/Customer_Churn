# Customer Churn Prediction

## Project Overview
This project focuses on predicting customer churn (attrition) in a telecommunications company. By analyzing customer demographics, service usage, and account details, the model identifies which customers are likely to discontinue their service. This insight is crucial for businesses to implement retention strategies.

The analysis and modeling process is documented in the Jupyter Notebook `Customer Churn.ipynb`.

## Dataset
The dataset used in this project is the **Telco Customer Churn** dataset. It typically contains 7,043 rows and 21 columns, including:

* **Demographics**: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
* **Services**: `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
* **Account Information**: `Contract`, `PaperlessBilling`, `PaymentMethod`
* **Billing**: `MonthlyCharges`, `TotalCharges`
* **Target Variable**: `Churn` (Yes = Customer left, No = Customer stayed)

## Technologies Used
* **Python 3.x**
* **Jupyter Notebook**
* **Pandas**: Data manipulation and cleaning.
* **NumPy**: Numerical operations.
* **Matplotlib / Seaborn**: Data visualization.
* **Scikit-Learn**: Machine learning models and evaluation metrics.

## Project Workflow
The notebook follows these key steps:
1. **Data Loading & Preprocessing**:
    * Handling missing values (e.g., in `TotalCharges`).
    * converting the target variable `Churn` to binary (0 and 1).
    * Encoding categorical variables using One-Hot Encoding or Label Encoding.
2. **Exploratory Data Analysis (EDA)**:
    * Visualizing the churn rate.
    * Analyzing the relationship between features (e.g., Contract type vs. Churn, Monthly Charges vs. Churn).
    * Correlation heatmap.
3. **Data Splitting**:
    * Splitting the dataset into Training and Testing sets (typically 80/20).
4. **Modeling**:
    * Training various classification models such as:
        * Decision Tree Classifier
        * Random Forest Classifier
        * Hyperparameter Tuning with RandomizedSearchCV
5. **Evaluation**:
    * Assessing model performance reporting using **Accuracy**, **Precision**, **Recall**, and **F1-Score**.

## How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/BRIMANO/Customer_Churn.git](https://github.com/BRIMANO/Customer_Churn.git)
2. Navigate to the project directory:
   ```bash
   cd Customer_Churn
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Customer_Churn.ipynb
4. Open `Customer Churn.ipynb` and execute the cells.