## README.md

**Description**


This project focuses on analyzing and predicting happiness levels across various countries using the World Happiness Report (WHR) 2018 dataset. The dataset contains socio-economic indicators that influence the "Life Ladder" score, a measure of the overall happiness level in each country.

**Dataset:**
The dataset, WHR2018Chapter2OnlineData.csv, includes the following features:

- Country: The name of the country.
- Year: The year of the observation.
- Life Ladder: The happiness score of the country, which serves as the target variable for prediction.
- Log GDP per capita: The logarithm of the country's GDP per capita.
- Social support: The perceived social support in the country.
- Healthy life expectancy at birth: The life expectancy at birth adjusted for health.
- Freedom to make life choices: The perceived freedom to make life choices in the country.
- Generosity: The generosity score based on survey responses.
- Perceptions of corruption: The perception of corruption in the government and business.
- Positive affect: The average positive emotional state of the population.
- Negative affect: The average negative emotional state of the population.
- Confidence in national government: The confidence level in the national government.
- Democratic Quality: The quality of democracy in the country.
- Delivery Quality: The effectiveness of the government in delivering public services.
- GINI index: The measure of income inequality within the country.
The dataset was preprocessed by handling missing values, scaling numerical features, and removing features with excessive missing data.

**Machine Learning Problem**


The goal of this project was to develop a predictive model for the "Life Ladder" score using various socio-economic indicators. This is a supervised learning problem that involves regression since the target variable, "Life Ladder," is a continuous numerical value.

**Approach**


**Exploratory Data Analysis (EDA):**
Extensive EDA was conducted to understand the relationships between the features and the target variable. Key steps included:

- Handling missing values by filling them with the mean.
- Identifying outliers through visualizations like boxplots.
- Understanding feature correlations with a heatmap.


**Model Development:**
Three models were trained and evaluated:

1. Linear Regression: A simple model to establish a baseline.
2. Random Forest Regressor: An ensemble method to capture non-linear relationships.
3. Gradient Boosting Regressor: Another ensemble method that sequentially improves predictions by correcting errors.
**Final Model Selection:**
After hyperparameter tuning, the **Random Forest Regressor with optimized parameters** was selected as the final model due to its strong performance in predicting happiness scores.

**Libraries Used**


- Pandas: For data manipulation and analysis, used to load and process the dataset.
- NumPy: For numerical computing, used for handling arrays and mathematical operations.
- Matplotlib: For data visualization, used to create plots and visualize data distributions.
- Seaborn: For advanced data visualization, used to generate plots such as heatmaps and pairplots.
- Scikit-learn: For machine learning, used for model training, evaluation, and feature scaling, including Linear Regression, Random Forest, and Gradient Boosting models.
- StandardScaler: From scikit-learn, used for feature scaling to standardize numerical values.
- GridSearchCV: From scikit-learn, used for hyperparameter tuning to optimize model performance.

**Key Findings**


Through the modeling process, it was identified that certain factors had a more significant impact on the happiness score:

- Log GDP per capita: Higher economic prosperity was strongly associated with higher happiness scores.
- Social support: Countries where people felt they had more social support tended to have higher happiness scores.
- Healthy life expectancy: Better health outcomes positively influenced happiness.
- Freedom to make life choices: Greater personal freedom was closely linked to higher happiness levels.
- Perceptions of corruption: Higher perceived corruption was associated with lower happiness scores.
These insights underscore the importance of economic stability, social cohesion, health, and governance in fostering national happiness.

**Conclusion**


The project successfully demonstrated how machine learning techniques can be applied to predict and analyze factors contributing to national happiness. The final model provided valuable insights into which socio-economic indicators are most influential in determining the happiness levels of different countries. This model, in addition to providing information for anybody looking to understand 'happiness', can also be valuable for policymakers, NGOs, and companies aiming to improve well-being and target interventions effectively in different regions.
