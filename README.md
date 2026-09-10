# 📊 Seasonal Agriculture Performance Analysis

## 📌 Project Overview

**Seasonal Agriculture Performance Analysis** is a data analytics project that investigates how agricultural performance varies across different seasons — **Kharif, Rabi, and Zaid**.

The project analyzes agricultural data to understand patterns and differences in **crop yield, production, revenue, cost, profit, water usage, water efficiency, environmental conditions, irrigation methods, disease and pest risk, crop-season combinations, and state-season performance**.

The objective is to transform raw agricultural data into meaningful insights that can support better **seasonal agricultural planning, resource utilization, crop selection, irrigation decisions, and regional planning**.

---

## 🎯 Problem Statement

Agricultural activities are influenced by seasonal variations in environmental conditions, farming practices, resource availability, and market conditions. As a result, agricultural performance may differ from one season to another.

However, raw agricultural data does not clearly explain how agricultural performance changes across seasons or what patterns can be observed under different seasonal conditions.

Therefore, this project analyzes the agricultural dataset to identify:

- Seasonal differences in agricultural yield
- Seasonal profitability patterns
- Water usage and water efficiency
- Performance of different irrigation methods
- Crop-season performance
- State-season profitability
- Relationships between agricultural variables
- Environmental conditions and their relationship with yield
- Disease and pest risk across seasons

The findings are used to provide data-driven recommendations for agricultural planning.

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Analyze agricultural performance across **Kharif, Rabi, and Zaid** seasons.
2. Compare average crop yield across different seasons.
3. Analyze seasonal revenue, cost, and profitability.
4. Study water usage and water efficiency across seasons.
5. Compare different irrigation methods based on yield, profit, and water usage.
6. Identify high-performing crop-season combinations.
7. Analyze profitability across states and seasons.
8. Study the relationship between environmental variables and yield.
9. Analyze disease and pest risk across seasons.
10. Identify important patterns and relationships in the agricultural dataset.
11. Provide data-driven recommendations for better agricultural planning.

---

## 📂 Dataset Information

The dataset contains:

- **4,000 records**
- **28 variables**

The dataset includes information related to:

| Category | Information |
|---|---|
| Season | Kharif, Rabi, Zaid |
| Crop | Chilli, Cotton, Groundnut, Maize, Pulses, Rice, Sugarcane, Wheat |
| Location | State |
| Yield | Crop yield in tonnes/ha |
| Production | Production in tonnes |
| Financial | Revenue, Total Cost, Profit |
| Market | Market Price |
| Water | Water Used and Water Efficiency |
| Irrigation | Drip, Flood, Rainfed, Sprinkler |
| Environment | Rainfall, Temperature, Soil Moisture |
| Soil | Soil pH and other soil-related variables |
| Inputs | Nitrogen, Phosphorus, Potassium, Fertilizer |
| Crop Quality | Seed Quality Score |
| Risk | Disease and Pest Risk |

---

## 🛠️ Technologies Used

### Programming Language

- Python

### Data Analysis

- Pandas
- NumPy

### Data Visualization

- Matplotlib
- Seaborn

### Development Environment

- Google Colab

---

## 🔄 Project Workflow

The project follows the following data analytics workflow:

```text
Data Collection
      ↓
Data Loading
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Missing Value Handling
      ↓
Duplicate Checking
      ↓
Descriptive Statistics
      ↓
Outlier Analysis
      ↓
Univariate Analysis
      ↓
Bivariate Analysis
      ↓
Multivariate Analysis
      ↓
Correlation Analysis
      ↓
Seasonal Analysis
      ↓
Visualization
      ↓
Insights
      ↓
Recommendations
````

---

## Data Cleaning

Data cleaning was performed before conducting the analysis.

### Missing Values

Missing values were identified in important variables such as:

* Rainfall
* Soil Moisture
* Yield

Missing values were handled using **season-wise median imputation** so that missing values were replaced using the median value of the corresponding season.

After imputation:

> **Total missing values = 0**

### Duplicate Records

Duplicate records were checked to ensure that the analysis was not affected by repeated observations.

> **Duplicate records = 0**

---

# 📊 Exploratory Data Analysis

The project uses several types of exploratory analysis.

## 1. Univariate Analysis

Individual variables were analyzed using:

* Histograms
* Count plots
* Box plots
* Descriptive statistics

Examples include:

* Yield distribution
* Profit distribution
* Season distribution
* Outlier analysis

---

## 2. Bivariate Analysis

Relationships between two variables were investigated using:

* Scatter plots
* Box plots
* Grouped comparisons

Examples include:

* Season vs Yield
* Season vs Profit
* Yield vs Profit

---

## 3. Multivariate Analysis

Multiple variables were analyzed together to understand more complex agricultural patterns.

Examples include:

* Crop × Season × Yield
* Irrigation × Season × Yield
* State × Season × Profit
* Environmental variables × Yield

---

# 📈 Key Results and Findings

## 1. Seasonal Yield Performance

The analysis shows that **Kharif recorded the highest average yield**, while **Zaid recorded the lowest average yield**.

| Season |      Average Yield |
| ------ | -----------------: |
| Kharif | **5.63 tonnes/ha** |
| Rabi   |     5.04 tonnes/ha |
| Zaid   | **4.64 tonnes/ha** |

### Insight

Kharif showed the strongest average yield performance among the three seasons.

---

## 2. Seasonal Profitability

Kharif also recorded the highest average profit.

| Season |  Average Profit |
| ------ | --------------: |
| Kharif | **₹178,914.65** |
| Rabi   |      ₹87,689.47 |
| Zaid   | **-₹24,804.82** |

### Insight

Zaid recorded **negative average profitability**, indicating that costs exceeded revenue on average in this season.

This suggests that Zaid season requires further investigation into:

* Crop selection
* Production costs
* Resource usage
* Revenue
* Market conditions

---

## 3. Seasonal Water Usage

Average water usage varies across seasons.

| Season | Average Water Used |
| ------ | -----------------: |
| Kharif |         6102.20 m³ |
| Rabi   |         5846.99 m³ |
| Zaid   |     **6419.89 m³** |

### Insight

Zaid used the highest average amount of water while also recording the lowest average yield.

This indicates a potential water-use challenge during Zaid.

---

## 4. Water Efficiency

Water efficiency was compared across seasons.

| Season |  Water Efficiency |
| ------ | ----------------: |
| Kharif | **5.89 t/1000m³** |
| Rabi   |     5.19 t/1000m³ |
| Zaid   |     4.41 t/1000m³ |

### Insight

Kharif achieved the highest average water efficiency among the three seasons.

---

## 5. Disease and Pest Risk

Kharif recorded the highest average disease/pest risk while also recording the highest average yield.

### Insight

Higher agricultural performance during Kharif is accompanied by higher disease/pest risk in the dataset.

Therefore, pest and disease monitoring should be strengthened during Kharif.

---

## 6. Irrigation Method Analysis

Different irrigation methods were compared using:

* Average Yield
* Average Profit
* Average Water Used
* Water Efficiency

| Irrigation Method | Avg Yield |   Avg Profit | Avg Water Used | Water Efficiency |
| ----------------- | --------: | -----------: | -------------: | ---------------: |
| **Drip**          |  **6.58** | **₹219,626** |     5918.75 m³ |             6.27 |
| Flood             |      4.86 |      ₹73,354 | **8026.47 m³** |             3.44 |
| Rainfed           |      4.60 |      ₹79,050 | **3549.55 m³** |         **7.56** |
| Sprinkler         |      5.16 |      ₹91,121 |     6208.26 m³ |             4.67 |

### Key Findings

* **Drip irrigation** recorded the highest average yield.
* Drip irrigation also recorded the highest average profit.
* **Flood irrigation** used the highest amount of water.
* **Rainfed agriculture** achieved the highest water efficiency.

### Important Observation

Irrigation methods involve trade-offs between yield, profitability, water usage, and water efficiency.

Therefore, irrigation decisions should not be based on a single performance measure.

---

## 7. Crop-Season Performance

The analysis compared crop performance across Kharif, Rabi, and Zaid seasons.

The dataset contains crops such as:

* Chilli
* Cotton
* Groundnut
* Maize
* Pulses
* Rice
* Sugarcane
* Wheat

### Highest-performing combination

**Sugarcane in Kharif** recorded the strongest crop-season performance.

* Average Yield: **53.46 tonnes/ha**
* Average Profit: approximately **₹10.01 lakh**
* Water Efficiency: approximately **36.00 t/1000m³**

### Insight

Crop performance varies significantly across seasons, making crop-season combinations important for agricultural planning.

---

## 8. State-Season Profitability

Agricultural profitability differs across states and seasons.

Some examples:

| State          | Best-performing Season |  Average Profit |
| -------------- | ---------------------- | --------------: |
| Gujarat        | Kharif                 |     ₹217,051.33 |
| Tamil Nadu     | Kharif                 |     ₹211,303.96 |
| Karnataka      | Kharif                 |     ₹201,226.21 |
| Telangana      | Kharif                 |     ₹199,668.38 |
| Andhra Pradesh | Kharif                 |     ₹169,315.52 |
| Punjab         | **Rabi**               | **₹169,294.52** |
| Maharashtra    | Kharif                 |     ₹168,801.05 |

### Insight

The best-performing season is not the same across all states.

For example:

* Gujarat performs best during **Kharif**.
* Punjab performs best during **Rabi**.

Therefore, seasonal planning should be **region-specific** rather than assuming that one season will perform best everywhere.

---

## 9. Environmental Conditions and Yield

The relationship between environmental variables and yield was investigated using correlation analysis.

| Variable      | Correlation with Yield |
| ------------- | ---------------------: |
| Rainfall      |                   0.03 |
| Temperature   |                   0.01 |
| Soil Moisture |                   0.01 |

### Insight

Rainfall, temperature, and soil moisture show **very weak linear relationships with yield** in this dataset.

These correlations indicate association only and **do not establish causation**.

Other factors such as crop selection, irrigation, management practices, costs, and market conditions may also influence agricultural performance.

---

## 10. Yield and Profit Relationship

The correlation between yield and profit is approximately:

> **0.49**

This indicates a **moderate positive linear relationship** between yield and profit in the dataset.

### Insight

Higher yield is generally associated with higher profit, but the relationship is not perfect.

This means that profitability can also depend on factors such as:

* Revenue
* Production cost
* Market price
* Water usage
* Crop selection
* Irrigation method

---

# 🔍 Important Insights

The major insights from the project are:

1. **Kharif recorded the highest average yield at 5.63 tonnes/ha.**
2. **Zaid recorded the lowest average yield at 4.64 tonnes/ha.**
3. **Kharif had the highest average profit of ₹178,914.65.**
4. **Zaid had negative average profitability of ₹24,804.82.**
5. Zaid used the highest average amount of water while recording the lowest yield.
6. Kharif achieved the highest seasonal water efficiency.
7. Kharif showed the highest disease/pest risk along with the highest average yield.
8. Drip irrigation recorded the highest average yield and profit.
9. Rainfed agriculture recorded the highest water efficiency.
10. Sugarcane in Kharif was the strongest crop-season combination.
11. Agricultural profitability varies considerably across states and seasons.
12. Rainfall, temperature, and soil moisture showed very weak linear relationships with yield.

---

# 💡 Recommendations

Based on the analysis, the following recommendations are proposed:

### 1. Focus on profitable seasonal opportunities

Kharif showed strong average yield and profitability and can be considered an important season for agricultural planning.

### 2. Investigate low Zaid profitability

The negative average profitability during Zaid should be investigated by examining:

* Crop selection
* Production costs
* Water usage
* Revenue
* Market conditions

### 3. Evaluate water usage against output

High water usage does not necessarily result in higher yield. Resource usage should be evaluated together with yield and profitability.

### 4. Evaluate irrigation methods using multiple metrics

Irrigation decisions should consider:

* Yield
* Profit
* Water consumption
* Water efficiency

rather than focusing on only one metric.

### 5. Strengthen pest and disease monitoring

Kharif showed the highest average disease/pest risk, so preventive monitoring and management should receive additional attention during this season.

### 6. Consider crop-season combinations

Crop selection should consider seasonal performance because the same crop may perform differently across Kharif, Rabi, and Zaid.

### 7. Use region-specific seasonal planning

Since the best-performing season differs across states, agricultural planning should consider regional conditions rather than applying one seasonal strategy to all states.

### 8. Consider multiple factors for yield planning

Yield should not be predicted or planned using environmental variables alone. Crop, irrigation, resource usage, production, and management-related factors should also be considered.

---

# ⚠️ Limitations

The analysis has several limitations:

1. Missing values were handled using **season-wise median imputation**, which may not perfectly represent the original values.
2. The number of observations is not equal across seasons.
3. Extreme observations may influence averages and correlation values.
4. Correlation indicates association and does not establish causation.
5. Seasonal differences may be influenced by crop selection, environmental conditions, irrigation, costs, and market conditions.
6. The dataset cannot establish that a particular agricultural practice directly caused a change in yield or profitability.
7. Additional historical weather data, market price fluctuations, and detailed farm-management information could improve the analysis.
8. Different crops have substantially different yield ranges, which can affect overall comparisons and outlier detection.

---

# 🚀 Future Scope

The project can be extended in several ways.

### Historical Weather Analysis

Incorporate historical weather data to study:

* Year-to-year seasonal changes
* Weather variability
* Long-term agricultural trends

### Market Analysis

Include historical market price fluctuations to better understand changes in profitability.

### Farm Management Analysis

Add detailed information about:

* Farming practices
* Fertilizer usage
* Irrigation schedules
* Seed selection
* Other management practices

### Crop-Specific Analysis

Perform detailed analysis for individual crops to reduce the influence of differences in crop composition.

### Region-Specific Analysis

Develop state- or region-specific models and recommendations.

### Predictive Analytics

Machine learning models could be developed to predict:

* Future crop yield
* Agricultural profitability
* Water requirements
* Seasonal performance

### Interactive Dashboard

An interactive dashboard could be developed to allow users to explore:

* Seasonal performance
* Crop performance
* Irrigation performance
* State-wise performance
* Profitability
* Water efficiency

### Water Resource Planning

Further analysis can identify more water-efficient agricultural practices and support sustainable resource planning.

---

# 📁 Project Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── README.md
│
├── seasonal_agriculture_performance_dataset.csv
│
├── Seasonal_Agriculture_Performance_Data_Analytics(1).ipynb
│
├── VOIS_Major_Project_PPT.pptx
```

---

# Project Notebook

The Google Colab notebook contains the complete analysis, including:

* Data loading
* Data cleaning
* Missing-value handling
* Duplicate checking
* Descriptive statistics
* Outlier analysis
* Univariate analysis
* Bivariate analysis
* Multivariate analysis
* Correlation analysis
* Seasonal analysis
* Crop-season analysis
* Irrigation analysis
* State-season analysis
* Environmental analysis
* Insights
* Recommendations
* Limitations
* Conclusion

---

# 📊 Visualizations

The project uses several visualization techniques, including:

* Count plots
* Histograms
* Box plots
* Bar charts
* Scatter plots
* Heatmaps
* Correlation heatmaps

These visualizations are used to make seasonal differences and relationships easier to understand.

---

# 🏁 Conclusion

The **Seasonal Agriculture Performance Analysis** project demonstrates how exploratory data analysis can be used to understand agricultural performance across different seasons, crops, irrigation methods, and regions.

The analysis indicates that **Kharif generally shows stronger overall performance**, with the highest average yield, profitability, and seasonal water efficiency. In contrast, **Zaid records lower average yield and negative average profitability**, while also showing the highest average water usage.

The irrigation analysis indicates that **Drip irrigation has the highest average yield and profit**, whereas **Rainfed agriculture has the highest water efficiency**.

The crop-season analysis highlights **Sugarcane in Kharif** as a particularly strong crop-season combination. State-level analysis also demonstrates that seasonal performance varies by region, highlighting the importance of region-specific agricultural planning.

Overall, the project shows that agricultural decisions should consider **season, crop, irrigation, water usage, profitability, and regional differences together**, rather than relying on a single performance measure.
