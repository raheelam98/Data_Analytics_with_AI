# EDA Fundamentals

This document explains the basic types of data and how to analyze them using **Univariate** and **Bivariate** analysis techniques in Exploratory Data Analysis (EDA).

---

## 1. Types of Data

### Quantitative Data (Numeric)
Values that can be **measured or counted**.

- **Continuous:** Infinite values within a range  
  *Example: height, weight*  
- **Discrete:** Fixed, countable values  
  *Example: shoe size, number of siblings*

### Qualitative Data (Categorical)
Values that are **descriptive and non-numeric**.

- **Nominal:** Categories with no order  
  *Example: blood type, gender*  
- **Ordinal:** Ordered categories  
  *Example: grades, satisfaction levels*

## 2. Data Distributions

The shape of a dataset shows how values are spread.  

- **Normal Distribution**  
  - Symmetrical, bell-shaped  
  - Mean = Median = Mode  
  - Example: heights, exam scores  

- **Skewed Distribution**  
  - Asymmetrical, one tail is longer  
  - **Right (Positive):** e.g. income  
  - **Left (Negative):** e.g. age at retirement  

- **Bimodal Distribution**  
  - Two distinct peaks  
  - Example: test scores (students who studied vs. didn’t)  

- **Uniform Distribution**  
  - All values are equally likely  
  - Example: rolling a fair dice

## 3. Univariate Analysis
**Analyze one column at a time** to understand its properties.

### Numerical Columns
- Calculate: mean, median, mode, std, min, max  
- Visualize: histogram, boxplot, density (KDE) plot  
- Check: outliers (boxplot, IQR, Z-score), skewness  
- Conclusion: summarize key patterns and issues

### Categorical Columns
- Calculate: frequency counts  
- Visualize: bar plot, pie chart  
- Check: missing values and handle them (impute or drop)  
- Conclusion: note most frequent categories and data quality

## 4. Bivariate Analysis
**Analyze relationships between two columns.**

- **Numerical vs Numerical**  
  - Use scatterplots, 2D histplots, correlation  

- **Numerical vs Categorical**  
  - Use barplots, boxplots, violinplots, KDEplots  

- **Categorical vs Categorical**  
  - Use crosstabs, heatmaps, stacked barplots  

**Goal:** Understand how two features affect each other and extract meaningful insights.

## 5. Summary

| Type of Analysis       | Purpose                    | Example Plots         |
|--------------------------|------------------------------|------------------------------|
| Univariate (1 column)    | Understand one feature       | Histogram, Boxplot            |
| Bivariate (2 columns)    | Understand relationships     | Scatterplot, Heatmap           |

---

## **Steps of Doing Univariate Analysis on Numerical Columns**

### **1. Descriptive Statistics**
- Compute basic summary statistics for the column, such as:
  - Mean  
  - Median  
  - Mode  
  - Standard Deviation  
  - Variance  
  - Minimum & Maximum  

### **2. Visualizations**
- Create visualizations to explore the distribution of the data.  
- Common visualizations include:
  - Histograms  
  - Boxplots  
  - Density plots (KDE plots)  

### **3. Identifying Outliers**
- Identify and examine any outliers in the data.  
- Methods for detecting outliers:
  - Visualization (Boxplots, Scatterplots)  
  - Statistical methods (IQR, Z-score)  

### **4. Skewness**
- Check for skewness in the data.  
- If skewness is significant, consider:
  - Data transformations (log, square root, Box-Cox, etc.)  
  - Using robust statistical methods  

### **5. Conclusion**
- Summarize the findings of the Exploratory Data Analysis (EDA).  
- Make decisions about how to proceed with further analysis.  


## **Steps of Doing Univariate Analysis on Categorical Columns**

### **1. Descriptive Statistics**
- Compute the frequency distribution of the categories in the column.  
- This gives insights into how often each category appears.

### **2. Visualizations**
- Create visualizations to explore the distribution of the categories.  
- Common visualizations include:
  - Bar plots  
  - Pie charts  

### **3. Missing Values**
- Check for missing values in the data and decide how to handle them.  
- Missing values can be:
  - Imputed (filled with a placeholder or most frequent value)  
  - Dropped (remove rows with missing values)  

### **4. Conclusion**
- Summarize the findings of the Exploratory Data Analysis (EDA).  
- Make decisions about how to proceed with further analysis.  


## **Steps of Doing Bivariate Analysis**

### **1. Select 2 Columns**

### **2. Understand the Type of Relationship**

#### **Numerical – Numerical**
- You can plot graphs like:
  - Scatterplot (regression plots)
  - 2D histplot
  - 2D KDEplots
- Check correlation coefficient to analyze linear relationship.

#### **Numerical – Categorical**
- Create visualizations that compare the distribution of numerical data across categories.
- Example plots:
  - Barplot
  - Boxplot
  - KDEplot
  - Violinplot
  - Scatterplots

#### **Categorical – Categorical**
- You can create:
  - Cross-tabulations or
  - Contingency tables (distribution of values in one category relative to another) check
- Example plots:
  - Heatmap
  - Stacked barplots
  - Treemaps

#### **Write Conclusion**
