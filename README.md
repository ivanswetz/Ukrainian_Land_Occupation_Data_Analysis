# Ukrainian Land Occupation Data Analysis

## 📌 Project Overview
This project analyzes the rate of Ukrainian land occupation during the Russo-Ukrainian War (2022– ).  
The dataset includes land occupied (measured in km²) from **January 2024 to February 2025** — a total of **59 weekly measurements**.  

The goal is to perform **descriptive data analysis** to understand trends, variability, and distribution of occupied land.  

---

## 📊 Dataset
- **Variable:** `LO` (land occupied in km²)  
- **Observations:** 58 (weekly data points)  
- **Period:** January 2024 – February 2025  

Example of the dataset:

| Week | LO   |
|------|------|
| 1    | 4    |
| 2    | 4    |
| 3    | 20   |
| 4    | 12   |
| 5    | 12   |
| 6    | 13   |

---

## 🔎 Data Analysis

### Descriptive Statistics
- Mean = 64.26  
- Median = 53.5  
- Mode = 4  
- Range = 196  
- Standard Deviation = 50.83  
- IQR = 70  

Since **Mean > Median > Mode**, the data is **right-skewed**.

### Visualizations
- Histogram (distribution shape)  
- Boxplot (spread & outliers)  
- Density Plot (continuous distribution)  
- Q-Q Plot (normality check)  

### Normality Test
- **Shapiro-Wilk test:** p-value = 0.00014  
- Conclusion: Data is **not normally distributed**.  

### Outlier Detection
- IQR method found one potential outlier: **200 km²**.  


---

## 🛠️ Tools Used
- **Excel** → initial descriptive statistics  
- **R (4.4.2)** → deeper analysis & visualizations  
  - `hist()` – histogram  
  - `boxplot()` – spread and outliers  
  - `density()` – distribution curve  
  - `shapiro.test()` – normality check  
  - Custom mode function – most frequent value  

---

## 📈 Key Insights
- The dataset is **right-skewed** (not symmetric).  
- High variability → predictions are less reliable.  
- The **Three Sigma Rule** is **not suitable** due to skewness and extreme values.  
- Normality is rejected by both visual and statistical tests.  
- Only **one outlier** detected (200 km²).  
