# Predictive-modelling-of-Tailpipe-CO2-emission-for-Early-vehicle-Analysis
# Predictive Modeling of Tailpipe CO₂ Emissions for Early Vehicle Design  

##  Objectives  
The goal of this project is to develop a predictive model to estimate vehicle tailpipe CO₂ emissions during the early engineering design phase. By analyzing relationships between fuel consumption, vehicle specifications, and engine characteristics, this model provides a data-driven way to:  
- Assess environmental impact of design decisions.  
- Improve fuel efficiency in vehicle development.  
- Support manufacturers, policymakers, and consumers in reducing emissions.  

---

##  Workflow Overview  

### 1. Data Import & Exploration  
- Dataset: **43,177 vehicles** (1984–2020) from [FuelEconomy.gov](https://www.fueleconomy.gov/).  
- Tools used: **Python (Pandas, Matplotlib, Seaborn), SAS, MATLAB, Tableau**.  
- Initial steps:  
  - Load CSV dataset.  
  - Check for missing values, duplicates, and inconsistencies.  
  - Review variable types (categorical vs. continuous).  

### 2. Data Preprocessing  
- Handled missing/null values (e.g., engine displacement, volume).  
- Converted categorical variables (fuel type, transmission, vehicle type) into appropriate formats.  
- Addressed multicollinearity using **Variance Inflation Factor (VIF)** analysis.  
- Removed poorly coded categorical predictors to reduce overfitting.  

### 3. Statistics Used  
- **Descriptive Statistics** (mean, median, variance, skewness, kurtosis).  
- **Pearson Correlation Coefficient** to measure linear relationships.  
- **Chi-Square Test of Independence & Homogeneity** to analyze categorical associations (e.g., emission category vs. fuel type, vehicle type, transmission type).  
- **Regression Modeling**:  
  - Initial regression with multiple predictors.  
  - Final regression model with optimized predictors (annual fuel consumption, combined MPG, engine displacement, cylinders, volume).  

### 4. Exploratory Data Analysis (EDA)  
- **Boxplots**: CO₂ emissions by number of cylinders.  
- **Distribution Analysis**: Probability density function of emissions.  
- **Correlation Plots**:  
  - Positive: CO₂ emissions vs. fuel consumption (barrels).  
  - Negative: CO₂ emissions vs. fuel efficiency (MPG).  
- **Contingency Tables**: Associations between emission categories and categorical features.  

---

##  Key Findings  
- Strong positive correlation between fuel consumption and CO₂ emissions (r ≈ 0.99).  
- Strong negative correlation between fuel efficiency (MPG) and emissions (r ≈ -0.91).  
- Significant associations between emission categories and **vehicle type, fuel type, and transmission** (Chi-square, p < 0.001).  
- Final regression model achieved **R² ≈ 0.98**, confirming high predictive accuracy.  

---

