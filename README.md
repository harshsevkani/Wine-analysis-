Wine Quality Analysis - Data Science Project

A comprehensive data analysis project focused on exploring and visualizing wine quality patterns using Python data science libraries.

📊 Project Overview

This project analyzes the Wine Quality Dataset (Red Wine) to understand the relationship between physicochemical properties and wine quality ratings. The analysis includes data exploration, statistical analysis, and advanced visualizations.

Dataset: 1,599 wine samples with 12 features (11 physicochemical properties + quality rating)

🛠️ Technologies & Libraries Used
Python 3.13
Data Processing: Pandas, NumPy
Visualization: Matplotlib, Seaborn
Data Analysis: Statistical methods & correlation analysis
📈 Key Features & Analysis
1. Data Exploration
Load and inspect red wine quality dataset
Dataset shape: (1599, 12)
Check for missing values and data types
Descriptive statistics and unique value counts
2. Exploratory Data Analysis (EDA)
Features Analyzed:
Fixed acidity
Volatile acidity
Citric acid
Residual sugar
Chlorides
Free sulfur dioxide
Total sulfur dioxide
Density
pH
Sulphates
Alcohol content
Quality (target variable: 3-9 scale)
3. Visualizations
Count Plot
Distribution of wine quality ratings
Bar chart showing frequency of each quality level
Swarm Plot
Relationship between quality and alcohol content
Individual data points showing outliers
Color-coded by viridis palette
Violin Plot
Probability density distribution of alcohol by quality
Shows distribution shape at each quality level
Semi-transparent overlay for better visualization
Box Plot
Quartile analysis of alcohol content across quality levels
Identify outliers and range of alcohol levels
Box-Enhanced Plot (Boxenplot)
Enhanced box plot for detailed distribution analysis
Better representation of tail distributions
Correlation Heatmap
Comprehensive correlation matrix of all variables
Annotated with correlation coefficients (4 decimal places)
Color-coded using Pastel1 palette
Identifies relationships between physicochemical properties and quality
🔍 Key Insights
Alcohol Content: Strong positive correlation with wine quality
Quality Distribution: Most wines rated 5-6 (average quality range)
Data Patterns: Clear outliers visible in categorical plots
Feature Relationships: Comprehensive correlation analysis reveals inter-feature dependencies
📁 Project Structure
├── lecture_13_09_26.ipynb
│   ├── Data Loading & Exploration
│   ├── Statistical Analysis
│   ├── Visualization Suite
│   └── Correlation Analysis
💡 How to Use
Load the Dataset:
python
   import pandas as pd
   df = pd.read_csv("winequality-red.csv", encoding="latin-1")
Explore Data:
python
   df.head()
   df.info()
   df.describe()
Create Visualizations:
python
   import seaborn as sns
   import matplotlib.pyplot as plt
   
   sns.heatmap(df.corr(), annot=True, cmap='Pastel1')
   sns.violinplot(x="quality", y="alcohol", data=df)
📊 Skills Demonstrated

✅ Data Loading & Preprocessing
✅ Exploratory Data Analysis (EDA)
✅ Statistical Analysis
✅ Data Visualization
✅ Correlation & Relationship Analysis
✅ Python Data Science Stack
✅ Problem Solving & Insights

🎓 Learning Outcomes

This project demonstrates proficiency in:

Handling real-world datasets
Statistical analysis and interpretation
Creating publication-quality visualizations
Using industry-standard Python libraries
Deriving actionable insights from data
📝 Notes
Dataset encoded in Latin-1 for compatibility
Warnings filtered to maintain clean output
Comprehensive analysis suitable for academic and professional use
