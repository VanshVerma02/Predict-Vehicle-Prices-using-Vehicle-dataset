
# 🚗 Vehicle Price Prediction

**Predict vehicle prices** based on specifications like make, model, mileage, fuel type, and more —
built in Python with **Random Forest Regression** for accurate results.

---

## 📌 Project Overview

This project aims to **estimate the market price of a vehicle** using historical listings and technical specifications.
It walks through the **complete ML pipeline** — from **data cleaning** to **model evaluation** — making it an excellent beginner project.

---

## 📊 Dataset Features

| Column Name      | Description                                  |
| ---------------- | -------------------------------------------- |
| `name`           | Full name of the vehicle (make, model, trim) |
| `description`    | Brief description of the vehicle             |
| `make`           | Manufacturer (e.g., Toyota, BMW)             |
| `model`          | Model name                                   |
| `year`           | Manufacturing year                           |
| `price`          | Price in USD *(target)*                      |
| `engine`         | Engine type & specifications                 |
| `cylinders`      | Number of cylinders                          |
| `fuel`           | Fuel type (Gasoline, Diesel, Electric, etc.) |
| `mileage`        | Mileage in miles                             |
| `transmission`   | Transmission type                            |
| `trim`           | Trim level                                   |
| `body`           | Body style                                   |
| `doors`          | Number of doors                              |
| `exterior_color` | Exterior color                               |
| `interior_color` | Interior color                               |
| `drivetrain`     | Drivetrain type (AWD, FWD, etc.)             |

---

## 🛠️ Workflow

### **1️⃣ Data Cleaning**

* Removed rows with missing `price`.
* Filled missing **numeric values** with the mean.
* Filled missing **categorical values** with the mode.

### **2️⃣ Feature Engineering**

* Created `vehicle_age` = `current_year` - `year`.
* Dropped `year` column after transformation.

### **3️⃣ Encoding**

* Used **Label Encoding** for categorical columns.

### **4️⃣ Model Training**

* Started with **Linear Regression** → R² ≈ 0.35 (low accuracy).
* Switched to **Random Forest Regressor** → R² ≈ 0.77 (high accuracy).

### **5️⃣ Evaluation**

* **MSE:** `68,860,248`
* **R² Score:** `0.7745` (model explains \~77% of price variation)
* **RMSE:** \~`8,300 USD`

---

## 📈 Results

✅ **Accuracy improved from 35% to 77%** after switching to Random Forest.
✅ **Prediction error reduced by \~6,000 USD** compared to the first model.
✅ Ready for further tuning with gradient boosting models.

---


## 🔮 Future Enhancements

* Extract **engine size** and convert to numeric for better predictions.
* Incorporate **brand popularity** or resale value index.
* Test **XGBoost** or **LightGBM** for performance improvements.
* Normalize skewed features like `mileage` and `price`.

---

## 🧠 Tech Stack

* **Python**
* **Pandas**
* **Scikit-learn**


