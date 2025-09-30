# Business Analytics Model – Price \& Demand Forecasting

## 📌 Overview



This project was developed as part of Module 4: Business Analytics Model Assignment.

It focuses on building and evaluating machine learning models for demand forecasting and price optimization using a retail dataset.



One main modeling approaches were explored:



Revenue simulation → Using predicted demand × price to evaluate optimal pricing and maximize revenue.



The notebook provides a step-by-step workflow, from data preparation to model evaluation and revenue optimization.



## 📂 Contents



Business\_Analytics\_Model.ipynb → Main notebook with code + narration



retail\_pricing\_enhanced.csv → Dataset used for model training and testing



artifacts/ → Saved models and results (best model .joblib, metrics .json,rev\_results\_quantity.json \& model\_metadata.json)



Data\_explanatory.ipynb  → previous EDA notebook



requirements.txt



### ⚙️ Methodology

#### Step 1: Data Preparation



Loaded and reviewed retail\_pricing\_enhanced.csv.



Target variable: Quantity.



Features: product attributes, pricing, and other metadata.



Preprocessing:



Numeric features → median imputation + scaling.



Categorical features → imputation + one-hot encoding.

#### 

#### Step 2: Model Training



Tested a broad set of models:



Linear models: Linear Regression, Ridge, Lasso.



Tree-based ensembles: RandomForest, GradientBoosting, XGBoost.



Neural networks: MLPRegressor.



#### Step 3: Evaluation



Metrics: RMSE, MAE, R².



Cross-validation for robust evaluation.



Comparison across models.



#### Step 4: Demand \& Revenue Curves



Simulated demand curves (quantity vs. price).



Computed revenue curves (price × predicted demand).



Identified optimal price points and revenue-maximizing models.



#### 📊 Results



Best statistical model: XGBoost (lowest RMSE, near-perfect R²).



Best business-oriented model: GradientBoosting/XGBoost (realistic revenue curves, strong predictive performance).



Discarded models: Linear, Ridge, Lasso (unrealistic predictions).



#### Key insights:



Demand decreases with higher prices (law of demand holds).



Revenue maximization occurs at mid-to-high price levels.



#### 🚀 How to Run



Clone this repository:



git clone <your\_repo\_link>

cd <your\_repo\_name>





#### Install dependencies:



pip install -r requirements.txt





#### Launch Jupyter Notebook:



jupyter notebook Business\_Analytics\_Model.ipynb

