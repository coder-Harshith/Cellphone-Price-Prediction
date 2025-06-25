# 📱 Cellphone Price Prediction

## 🧠 Project Objective

The goal of this project is to predict the **price range** (Low, Medium, High, Very High) of mobile phones using their **technical specifications**. Instead of predicting an exact price, this classification model helps businesses understand where their product might fall in the pricing spectrum, enabling more informed product strategy and market positioning.

---

## 📂 Dataset Overview

**Dataset Source:**
[Cellphone Price Dataset - ZIP Download](https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1009-CellphonePrice.zip)

**Main File Used:**
`datasets_11167_15520_train.csv`

**Target Variable:**

* `price_range` (0 = Low, 1 = Medium, 2 = High, 3 = Very High)

**Key Features:**

* `battery_power`: Battery capacity (mAh)
* `ram`: RAM in MB
* `int_memory`: Internal storage in GB
* `blue`: Bluetooth availability
* `four_g`, `three_g`, `wifi`: Connectivity features
* `pc`, `fc`: Primary and front camera megapixels
* `px_height`, `px_width`: Screen resolution
* `dual_sim`, `touch_screen`: Boolean indicators
* `n_cores`, `clock_speed`: CPU specifications

---

## 📈 Project Workflow

### 1. Data Preprocessing

* Handled missing/null values (if any)
* Checked data types and performed encoding (if needed)
* Feature scaling (StandardScaler)

### 2. Exploratory Data Analysis (EDA)

* Visualized correlations between features and target
* Analyzed distribution of price ranges
* Checked influence of RAM, battery, and connectivity features on price

### 3. Model Building

* Applied classification algorithms:

  * Logistic Regression
  * Random Forest Classifier
  * Support Vector Machine
  * Decision Tree
  * XGBoost

### 4. Model Evaluation

* Used accuracy, precision, recall, F1-score
* Cross-validation for reliable performance measurement
* Visualized confusion matrix and ROC curves (if applicable)

### 5. Feature Importance

* Identified key contributors to price prediction using tree-based models
* RAM, Battery, and Resolution were highly influential

---

## 🏆 Best Performing Model

After testing and comparing all models, **Random Forest Classifier** (or another, if changed) yielded the highest performance in terms of balanced accuracy and interpretability.

---

## 🧩 Business Impact

The model provides insights into which hardware features most strongly influence a phone's pricing tier, helping manufacturers:

* Design optimized phones for targeted price segments
* Prioritize features for specific consumer demands
* Compete effectively with top brands

---

## 🚧 Challenges Faced

* Managing the balance between model complexity and performance
* Avoiding overfitting with models like Decision Trees
* Dealing with similar specification mobiles across different price ranges
* Ensuring scalability of the model for real-world deployment

---

## 🛠️ Tools & Technologies

* Python
* Jupyter Notebook
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* XGBoost

---

## 📌 Conclusion

This project demonstrates how machine learning can be applied to real-world business problems like product pricing. With accurate classification and strategic analysis, businesses can enhance product planning, marketing, and pricing strategies.
