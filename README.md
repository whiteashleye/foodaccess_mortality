# Food Deserts and the Understated Impact on Public Health

---
## Author:

Ashley White
- [LinkedIn](https://www.linkedin.com/in/aewhite5/)
- [Personal Site](https://www.radicaldata.co)

---
## Introduction
Many academic studies have examined the effects of food access on proximal outcomes, such as food shopping behavior and food consumption. Others have asserted the relative lack of access to full-service grocery stores and the easier access to fast and convenience foods may be linked to obesity and other diet-related diseases.

I have initiated this data science study to quantify the social externalities of food access in an effort to raise awareness and encourage communities to more effectively advocate for effective solutions.

[Presentation](https://docs.google.com/presentation/d/1jXU9hSN0IifVkv4yjy-Uy0IvyltaqJX00cUokGf5ggM/edit?usp=sharing)

---
## Data Collection

| Name | Description | Link |
| --- | --- | --- |
| Food Access Research Atlas | Spatial overview of food access indicators for low-income and other census tracts using measures of supermarket accessibility | [Link](https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data/)|
|Compressed Mortality, 1999-2016| Rates of death by underlying cause of death, state, county, age, race, sex, and year | [Link](https://wonder.cdc.gov/cmf-icd10.html)|

---
## TOC
### Inputs
- [Mortality and Food Access Cleaned Data File](https://github.com/whiteashleye/foodaccess_mortality/blob/master/df_foodaccess_allmortality_SVI.csv)

### Modeling
- [Elastic Net Regression](https://github.com/whiteashleye/foodaccess_mortality/blob/master/FoodAccess_Mortality_Regression_NoPoverty_Log10_AWS.ipynb)

- [Random Forest Regression](https://github.com/whiteashleye/foodaccess_mortality/blob/master/FoodAccess_Mortality_RandomForest_AWS.ipynb)

- [Poisson GLM](https://github.com/whiteashleye/foodaccess_mortality/blob/master/FoodAccess_Mortality_Statsmodels.ipynb)

### Scores & Evaluation
- [Elastic Net Scores](https://github.com/whiteashleye/foodaccess_mortality/blob/master/enet_Log10_scores.csv)

- [Poisson GLM Coefficients](https://github.com/whiteashleye/foodaccess_mortality/blob/master/LAShare_coefs.csv)

- [Random Forest Scores](https://github.com/whiteashleye/foodaccess_mortality/blob/master/rf_scores.csv)

- [Random Forest Feature Importance](https://github.com/whiteashleye/foodaccess_mortality/blob/master/rf_feature_importance.csv)


---

## Data Collection and Analysis

### The Question:
What is the impact of food access on public healthy?

### The Data Science Problem:
What is the covariance / correlation and predictive accuracy of food access  features  as it relates to per capita mortality rates?

### The Approach:
Leverage generalized linear models and decision tree regression to evaluate mean absolute error, r^2, and feature importance

---

### Conclusion

* Food access can explain 20-80% of the variance in per capita mortality rates  at  the county level
* Increased correlation in deaths from drug overdoses, transportation, and diabetes
* Lessons to be learned from self-sustaining rural areas
* SNAP appears to help reduce impact of food access

---

### Next Steps

* Incorporate Data from Food Environment Atlas & Census Tract Mortality
* Improve viz / interactivity
* Identify counties with biggest potential for improvement / intervention
* Identify counties to gather lessons learned
