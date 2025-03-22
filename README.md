# Assessing the Impact of the 2008 Financial Crisis on Heart Disease Mortality  

##  Project Overview  
This project investigates whether the 2008 financial crisis caused an increase in heart disease mortality rates in the United States. Using a **Difference-in-Differences (DiD)** analysis, the study compares mortality trends between a treatment group (heart disease deaths) and a control group (cancer deaths) before and after the financial crisis. The goal is to isolate the impact of the financial crisis on heart disease mortality while accounting for general mortality trends.  

---

##  Objective  
- To assess the causal relationship between the 2008 financial crisis and heart disease mortality rates.  
- To determine if changes in heart disease deaths post-crisis are statistically significant compared to a control group.  
- To analyze patterns in financial and health data to identify trends and potential public health implications.  

---

## 🗂 Datasets Used  
| Dataset | Source | Usage |  
|---------|--------|-------|  
| **Heart Disease Mortality Data** | CDC (2007–2022) | Analyzed heart disease mortality trends |  
| **Cancer Mortality Data** (Control Group) | CDC (2007–2022) | Served as a control to isolate the crisis impact |  
| **S&P 500 Stock Prices** | Yahoo Finance (2007–2022) | Tracked financial crisis progression and severity |  
| **Unemployment Rates** | Bureau of Labor Statistics (2007–2022) | Incorporated to assess economic conditions influencing public health |  
| **Inflation Rates** | World Bank (2005–2022) | Captured broader economic stress during the financial crisis |  

---

##  Methodology  
### 1. **Data Preparation**  
- Collected and cleaned data from the CDC, Yahoo Finance, Bureau of Labor Statistics, and World Bank.  
- Aggregated and standardized heart disease and cancer mortality data by age and region.  
- Created binary variables for treatment (heart disease = 1, cancer = 0) and post-crisis period (post-September 2008 = 1).  

### 2. **Difference-in-Differences (DiD) Model**  
The DiD analysis follows this regression model:  

Deaths = β0 + β1 * Treatment + β2 * PostCrisis + β3 * (Treatment * PostCrisis) + ε

- **β₀** – Baseline deaths for cancer pre-crisis.  
- **β₁** – Difference in deaths between heart disease and cancer pre-crisis.  
- **β₂** – Change in cancer deaths post-crisis.  
- **β₃** – Effect of the crisis on heart disease deaths (DiD estimator).  

### 3. **Testing and Results**  
- Tested the model for three post-crisis periods (3 months, 6 months, 9 months).  
- Analyzed statistical significance using p-values and coefficient interpretations.  
- **No statistically significant evidence** was found linking the 2008 crisis to an increase in heart disease mortality rates.  

---

##  Key Findings  
1. The DiD estimator was not statistically significant across all time periods.  
2. Visual inspection showed consistent trends in heart disease and cancer deaths pre- and post-crisis.  
3. The p-values were consistently above the 0.05 significance threshold, indicating no causal relationship between the crisis and heart disease deaths.  

---

## 🛠️ Tools and Technologies  
- **Python** – Data cleaning, modeling, and analysis  
- **Pandas, NumPy** – Data manipulation and aggregation  
- **Statsmodels** – Regression analysis  
- **Matplotlib, Seaborn** – Data visualization  

---

##  Challenges  
- Controlled for confounding mortality trends using a control group.  
- Ensured data consistency across different time frames and geographic locations.  
- Interpreted complex interactions between health and economic variables.  

---

##  Conclusion  
The analysis found no statistically significant increase in heart disease deaths post-2008 financial crisis. The study effectively demonstrates the application of DiD analysis in a real-world public health and economic scenario.  


---

##  Next Steps  
- Include additional control variables (e.g., healthcare access, lifestyle factors).  
- Extend the study to other causes of death for broader analysis.  
- Explore machine learning models for better mortality rate prediction.  

---

##  Contributors  
- **Sankalp Biswal**  

---

##  References  
- Centers for Disease Control and Prevention (CDC)  
- Yahoo Finance  
- Bureau of Labor Statistics  
- World Bank  

---

## License  
This project is licensed under the MIT License.  


