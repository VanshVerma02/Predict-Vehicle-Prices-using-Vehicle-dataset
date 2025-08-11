🚗 Vehicle Price Prediction
A beginner-friendly machine learning project that predicts vehicle prices using specifications like make, model, mileage, fuel type, and more.
Built in Python with Random Forest Regressor for improved accuracy.

📌 Objective
To develop a system that can predict vehicle prices using key features from a dataset of various cars.
The goal is to explore the data, handle missing values, and train a regression model to make price predictions.

📊 Dataset Description
The dataset contains vehicle specifications, features, and prices.

Column Name	Description
name	Full name of the vehicle (make, model, trim)
description	Short description of the vehicle
make	Manufacturer (e.g., Toyota, Ford, BMW)
model	Model name
year	Year of manufacture
price	Price in USD (target variable)
engine	Engine details and specifications
cylinders	Number of engine cylinders
fuel	Fuel type (Gasoline, Diesel, Electric, etc.)
mileage	Vehicle mileage
transmission	Transmission type (Automatic, Manual, etc.)
trim	Trim level
body	Body style (SUV, Sedan, etc.)
doors	Number of doors
exterior_color	Exterior color
interior_color	Interior color
drivetrain	Drivetrain type (AWD, FWD, etc.)

🛠️ Steps Performed
1. Data Cleaning & Preprocessing
Dropped rows with missing price (target variable).

Filled missing numeric columns with their mean.

Filled missing categorical columns with most frequent value (mode).

Created a new feature vehicle_age = current_year - year.

Encoded categorical variables using Label Encoding.

2. Model Selection
Started with Linear Regression → R² score = 0.35 (low accuracy).

Upgraded to RandomForestRegressor → R² score = 0.77 (much better).

3. Model Evaluation
Mean Squared Error (MSE): 68,860,248

R² Score: 0.7745

Interpretation: Model explains ~77% of the variation in vehicle prices.


# 1️⃣ Install dependencies
pip install pandas scikit-learn

# 2️⃣ Run the Python script
python vehicle_price_prediction.py
📈 Results
✅ Improved accuracy from 0.35 → 0.77 using Random Forest.
✅ RMSE reduced from ~14,000 USD to ~8,300 USD.

🧠 Future Improvements
Extract numerical engine size from engine text column.

Add brand popularity scores.

Use Gradient Boosting (XGBoost, LightGBM) for further performance gains.

Normalize skewed numerical features like mileage and price.

📌 Tech Stack
Python

Pandas

Scikit-learn
