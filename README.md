# 📌 Intelligent Learning and Decision-Making Project

## 📖 Overview
This project was developed as part of the "Intelligent Learning and Decision-Making" course at the University of Minho. The primary objective was to apply machine learning techniques to two different datasets: **Madrid Climate** and **Salary Classification**. The project follows the **CRISP-DM methodology**, covering data exploration, preprocessing, modeling, and evaluation.

## 📁 Datasets
### 🌦 Madrid Climate
- **Description:** This dataset contains climate-related data collected in Madrid between **07/01/2008 and 04/20/2019** (3946 records).
- **Key Features:**
  - Date and time
  - Temperature (Min, Max, Feels Like, Dew Point, etc.)
  - Humidity, Wind speed, and Cloud cover
  - UV index, Precipitation, and Pressure

### 💰 Salary Classification
- **Description:** This dataset consists of **48,842 records** and includes demographic and professional information.
- **Key Features:**
  - Age, Education, Work class, Occupation
  - Relationship, Race, Sex, and Native Country
  - Capital Gain/Loss, Hours per Week
  - **Target Variable:** Whether an individual earns more than **$50,000/year** or not

## 🔍 Methodology
The **CRISP-DM methodology** was applied:
1. **Data Understanding** – Studied the datasets and their characteristics.
2. **Data Preparation** – Processed and cleaned the data, including:
   - Handling missing values
   - Creating new features (e.g., thermal amplitude for climate data)
   - Normalization and encoding categorical variables
3. **Modeling** – Built machine learning models for classification and regression.
4. **Evaluation** – Assessed the models' performance using accuracy metrics.

## 🚀 Machine Learning Approaches
### 🌿 Madrid Climate Dataset
#### **Classification Task:** Predicting the Season
- **Objective:** Determine the season (Winter, Spring, Summer, or Fall) based on climate variables.
- **Models Used:**
  - **Decision Tree Classifier** (Supervised Learning)
  - **Clustering (k-means & Hierarchical Clustering)** (Unsupervised Learning)
- **Results:**
  - Summer and Winter were well-defined, but Spring and Fall had overlapping characteristics.
  - The hypothesis that "Madrid has four well-defined seasons" was refuted.

#### **Regression Task:** Predicting Daily Temperature
- **Objective:** Predict daily temperature based on weather conditions.
- **Model Used:**
  - **Linear Regression**
- **Results:**
  - Achieved **100% accuracy (R² = 1.0, RMSE = 0)**
  - Showed strong correlation between temperature and other climate variables

### 📊 Salary Classification Dataset
#### **Classification Task:** Predicting Salary Range
- **Objective:** Predict whether an individual earns more than **$50,000/year**.
- **Models Used:**
  - **Decision Tree Classifier**
    - Gini Index (without pruning)
    - Gain Ratio (with MDL pruning)
  - **Artificial Neural Network (Feedforward MLP)**
- **Results:**
  - **Decision Tree (Gain Ratio with Pruning)** performed the best (**Accuracy: 83.39%**)
  - **Neural Network** had lower performance (**Accuracy: 81.77%**) due to feature complexity

## 📝 Key Takeaways
- **Data preprocessing is crucial:** Cleaning and transforming data significantly impact model performance.
- **Feature selection matters:** Selecting the right features improves accuracy and reduces computation.
- **Simple models can outperform complex ones:** Decision Trees outperformed Neural Networks in salary classification.
- **Unsupervised learning helps understand data:** Clustering techniques provided valuable insights.

## 🎯 Future Work
- Implement **feature selection techniques** to improve Neural Network performance.
- Explore **ensemble methods** (Random Forest, Gradient Boosting) for better salary classification.
- Use **deep learning models** for more complex relationships in the datasets.

