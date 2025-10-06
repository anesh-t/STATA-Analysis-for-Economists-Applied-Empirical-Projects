# STATA Analysis for Economists — Applied Empirical Projects

This repository contains a collection of applied econometric exercises completed using **Stata**.  
Each project demonstrates how to manage, visualize, and analyze real-world data through modern econometric techniques used in applied economics and public policy research.

---

## 🎯 Project Purpose

The objective of this repository is to provide practical examples of how to use **Stata** for data-driven economic analysis.  
Through these exercises, key econometric methods are implemented step-by-step — from data cleaning and descriptive statistics to regression modeling and advanced estimation techniques.

This repository serves as a learning and reference tool for anyone interested in:
- Strengthening applied econometric skills  
- Reproducing empirical models  
- Learning the structure of Stata `.do` files  
- Building reproducible workflows in economic research  

---

## 📂 Repository Structure

stata-analysis-projects/
│
├── ch3_data.do # Data import, cleaning, and management
├── ch4_basiccommand.do # Basic descriptive statistics and commands
├── ch5_OLSmodel.do # OLS regression models and interpretations
├── ch6_timeseries.do # Time-series econometric applications
├── ch7_IV.do # Instrumental variable estimation
├── ch8_discretemodel.do # Logit/Probit and discrete choice models
│
├── Publicecon_empirical_elasticity.do # Public economics elasticity estimation
├── Publicecon_inequality_lorenz.do # Income inequality and Lorenz curve analysis
│
└── README.md # Repository overview and documentation

markdown
Copy code

---

## 🧠 Topics Covered

1. **Data Handling and Cleaning**
   - Importing and merging datasets (`use`, `merge`, `append`)
   - Generating and labeling variables
   - Managing missing values

2. **Descriptive Statistics**
   - `summarize`, `tabulate`, `correlate`
   - Histograms, scatter plots, and basic data visualization

3. **Regression Analysis**
   - Bivariate and multivariate OLS models
   - Hypothesis testing and interpretation of coefficients

4. **Instrumental Variables (IV)**
   - Using `ivregress` for endogeneity correction
   - Understanding two-stage least squares (2SLS)

5. **Time-Series Models**
   - Setting time-series data with `tsset`
   - Exploring trends, AR(1) models, and forecasting

6. **Discrete Choice Models**
   - Binary outcome models (`logit`, `probit`)
   - Calculating and interpreting marginal effects

7. **Public Economics Applications**
   - Elasticity estimation
   - Lorenz curves and inequality measures (Gini coefficient)

---

## 📊 Example Command Snippets

```stata
* Basic summary statistics
summarize wage age education

* OLS regression
reg wage education experience age

* Instrumental variable model
ivregress 2sls wage (education = distance_to_college)

* Time-series setup and regression
tsset year
reg gdp growth_rate, lags(1)

* Logit model
logit employed education gender age
