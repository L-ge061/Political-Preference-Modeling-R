# Political Preference Modeling 

## Overview
This project analyzes the relationship between **race, gender, and political party preference** using statistical modeling in R. The study applies contingency tables, logistic regression, log-linear models, and model selection methods (AIC, BIC, Lasso regression) to uncover political patterns and associations.

---

## Tools Used
- **R programming language**
- **tidyverse** (data manipulation & visualization)
- **glm** (logistic & log-linear regression)
- **glmnet** (Lasso regression)

---

## Analysis Workflow
1. **Data Import & Exploration** – Contingency tables across Race, Gender, and Party.  
2. **Logistic Regression** – Party preference modeled as a function of Race.  
3. **Log-linear Models** – Tested associations among Race, Gender, and Party.  
4. **Model Selection** – Forward, backward, and stepwise selection using AIC/BIC.  
5. **Regularization** – Lasso regression for variable selection.  
6. **Statistical Testing** – Wald, Likelihood Ratio, and Score tests.  
7. **MLE Validation** – Verified first-order conditions and variance-covariance matrices.  

---

## Findings & Insights
- **Race and Party**: Race showed a weak but consistent association with political party preference, especially among female voters.  
- **Black vs. White**: Black individuals had higher odds of supporting Party A compared to White individuals, though results were not strongly significant.  
- **Gender Effects**: Gender did not strongly alter the Race-Party relationship, suggesting relative homogeneity across gender groups.  
- **Model Selection**: Multiple methods pointed to the same model:  
  `Frequency ~ Race + Gender + Party + Race:Party`  
- **Lasso Regression**: Most predictors were shrunk to zero, highlighting only Race and selected interactions as meaningful.  

---

## Conclusion / Business & Political Insights
- **Policy & Campaign Strategy**: Weak but present racial differences suggest that tailored campaign messaging may be more effective than broad outreach.  
- **Resource Allocation**: Since gender is not a strong modifier, resources can be focused on race-based differences rather than gender segmentation.  
- **Predictive Modeling**: Regularization methods show that a small number of predictors drive most variation, allowing analysts and campaign teams to reduce complexity.  
- **Broader Implications**: Findings demonstrate how data science can uncover subtle demographic influences on political preferences, aiding decision-making in politics and public policy.  

---

## What’s Next? (Future Exploration)
If given more time, this project could be expanded by:  
- Adding more demographic features (e.g., age, education, region, income).  
- Comparing regression models with **machine learning classifiers** (Random Forests, Gradient Boosting).  
- Conducting **longitudinal or time-series analysis** if repeated survey data is available.  
- Building an **interactive dashboard (Shiny app or Power BI)** to allow users to explore patterns dynamically.  
- Extending analysis beyond politics to **marketing, healthcare, or social behavior** datasets with similar structures.  

