# Laptop-Price-Prediction-Model

## Overview

This project focuses on predicting laptop prices using machine learning techniques. The goal is to build a model that can estimate the price of a laptop based on its specifications such as RAM, CPU, storage, display features, and more.


##  Features

* Data cleaning and preprocessing
* Feature engineering from complex text data
* Exploratory Data Analysis (EDA)
* Machine learning model training and evaluation
* Price prediction using trained model


##  Dataset

The dataset contains information about various laptops, including:

* Company
* TypeName
* RAM
* Weight
* Touchscreen
* IPS Display
* PPI (Pixels Per Inch)
* CPU Type
* GPU Brand
* Storage (SSD/HDD)
* Operating System
* Price (Target Variable)


## Data Preprocessing

The following preprocessing steps were performed:

### 1. Data Cleaning

* Removed unnecessary columns
* Converted RAM from string ("8GB") to integer
* Converted Weight from string ("1.37kg") to float

### 2. Feature Engineering

* Extracted **Touchscreen** and **IPS display** from screen resolution
* Calculated **PPI (Pixels Per Inch)** using resolution and screen size
* Simplified **CPU types** into categories (i3, i5, i7, AMD, Others)
* Extracted **GPU brand**
* Converted storage into **SSD and HDD values (in GB)**

### 3. Handling Categorical Data

* Applied **One-Hot Encoding** to categorical features

### 4. Target Transformation

* Applied **log transformation** to price to reduce skewness


## Models Used

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor


## Model Pipeline

A pipeline was used to:

* Handle preprocessing steps
* Train the model efficiently
* Ensure consistency between training and prediction


##  How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/laptop-price-prediction.git
cd laptop-price-prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Jupyter Notebook

```bash
jupyter notebook
```

Open `Laptop Price Prediction.ipynb` and run all cells.


## Results

* Random Forest performed best among tested models
* Log transformation improved prediction accuracy


##  Tools & Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn
* Jupyter Notebook


## Future Improvements

* Hyperparameter tuning
* Deploy model as a web app
* Use advanced models (XGBoost, Gradient Boosting)


## Author

**Faniiiii**
Computer Science Undergraduate
Interested in AI, Machine Learning, and Data Science


## License

This project is open-source and available under the MIT License.
