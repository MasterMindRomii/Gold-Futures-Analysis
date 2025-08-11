# 🚀 Day 14: Gold Futures Analysis 📈

Welcome to **Day 14** of my data exploration journey!  
Today, we're diving deep into the world of **Gold Futures** to uncover valuable insights and trends in the gold market.

---

## 📝 Project Overview

Our primary focus is to analyze Gold Futures data —  
a comprehensive dataset that offers a great opportunity to explore historical price trends and market behavior.

**Key Steps:**  
- **Data Preprocessing:** Handle missing values and format data for analysis  
- **Data Visualization:** Create informative charts to visualize trends  

By exploring this dataset, we aim to reveal interesting patterns, price fluctuations, and other valuable insights related to Gold Futures.

---

## ✨ Key Takeaways

- **Data Preprocessing:** Practiced handling missing data and proper formatting  
- **Visual Insights:** Created visualizations to grasp price trends and market behavior  
- **Drawing Conclusions:** Extracted meaningful insights from complex financial data  

---

## 💻 Essential Code Snippets

```python
# 1. Library Imports
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# 2. Data Import
df = pd.read_csv(r'C:\\Users\\Dell\\OneDrive\\Desktop\\75 Day\\EDA-DAY14\\GOLDdata.csv', encoding='unicode_escape')

# 3. Initial Data Exploration
df.head()
df.describe()
df.shape
df.columns
df.info()

# 4. Data Cleaning & Preparation
df['Date'] = pd.to_datetime(df['Date'])

# 5. Value Analysis
print("Max High:", df['High'].max())
print("Min High:", df['High'].min())
print("Min Low:", df['Low'].min())
print("Max Low:", df['Low'].max())
print("Min Price:", df['Price'].min())
print("Max Price:", df['Price'].max())
print("Missing Values:\n", df.isnull().sum())
