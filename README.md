# World Happiness Prediction Project

### Author: Aditya Shah ([as5069@scarletmail.rutgers.edu](mailto:as5069@scarletmail.rutgers.edu))  

This project develops a regression model to predict happiness levels using socioeconomic and psychological indicators. It highlights the potential of statistical modeling in understanding the dynamics of human well-being.

---

## 📌 Introduction  
The goal of this project is to build a statistical model to predict happiness levels across countries using variables like:  
- GDP per capita  
- Social support  
- Life expectancy  
- Generosity  
- Corruption perceptions  

Key methods include regression analysis with advanced techniques like Random Forest and Gradient Boosting. The model performance is evaluated using metrics such as:  
- Mean Squared Error (MSE)  
- R-squared  
- Cross-validation  

---

## 📊 Dataset Description  
The dataset, sourced from the World Happiness Report, includes the following attributes:  
- Country, Year, Happiness Score  
- Log GDP per capita  
- Social Support  
- Life Expectancy  
- Freedom of Choices  
- Generosity, Corruption  
- Positive and Negative Affect  

A thematic map visualizes the global distribution of happiness scores.

---

## 🔍 Model Overview  
### Random Forest Regressor:  
- Handles large datasets with complex, non-linear relationships.  
- Robust to multicollinearity and overfitting.  

**Key Formulas**:  
1. **Mean Squared Error (MSE)**:  
   \[
   MSE = \frac{1}{n} \sum_{i=1}^n (y_i - \hat{y_i})^2
   \]  
2. **Random Forest Prediction**:  
   \[
   \hat{y}_{\text{forest}} = \frac{1}{T} \sum_{t=1}^T \hat{y}_t
   \]  

**Model Preprocessing**:  
- **Categorical Features**: Imputed and one-hot encoded.  
- **Numerical Features**: Missing values imputed using the mean.  

**Data Split**:  
- Training set: 80%  
- Validation set: 20%  

Hyperparameter tuning was performed using Randomized Search with cross-validation.

---

## 📈 Results  
- **Median Happiness Scores by Region**:  
  - Oceania, North America, and Europe show improvements.  
  - Africa and South Asia face challenges.  
- **Feature Importance Analysis**:  
  - Most impactful: GDP per capita, Social Support, Life Expectancy.  
  - Less impactful: Features like Generosity and Corruption.  

**Model Performance**:  
- Optimized Random Forest Regressor achieved **MSE = 0.21664**.  
- Residual analysis confirms close alignment of predictions with actual values.  

---

## 🎯 Conclusion  
- Key predictors of happiness include GDP per capita, social support, and life expectancy.  
- The project identified regional trends in happiness scores, revealing economic, cultural, and social dynamics globally.  

---
