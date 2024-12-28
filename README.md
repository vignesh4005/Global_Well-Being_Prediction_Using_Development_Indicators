## **Global Well-Being Prediction Using Development Indicators (Socioeconomic, Governance, and Happiness Metrics)**

## Objective
The main goal of this project is to predict the global well-being of countries based on a combination of socioeconomic, governance, and subjective well-being indicators. The project leverages data from the World Happiness Report from 2005 to 2023, integrating various factors such as economic conditions, social support, governance, health, and individual perceptions to predict overall happiness and life satisfaction across nations.

## Specific Goals

### 1. Data Exploration and Preprocessing
- Analyze and preprocess the dataset to handle missing values, normalize data, and ensure the integrity of categorical and numerical variables.
- Identify the key socioeconomic and psychological factors that most influence happiness scores globally.

### 2. Identify Global Trends
- Analyze trends in happiness scores globally and regionally.
- Identify regions or countries with consistently high or low happiness levels.

### 3. Predict Happiness Scores
- Build predictive models using machine learning techniques to forecast happiness scores based on available features like GDP, social support, and other socio-economic variables.
- Compute the change in "Life Ladder Score" over years for each country and predict the direction (increase or decrease).

### 4. Socioeconomic, Governance, and Well-Being Insights
- Investigate how socioeconomic factors (e.g., GNI per capita, total population, internet penetration) and governance indicators (e.g., Voice and Accountability, Government Effectiveness) influence happiness.
- Identify the most significant drivers of well-being across countries and explore any regional patterns that could inform policymaking.

### 5. Visualize Relationships
- Create meaningful visualizations to represent the relationships between key variables.
- Highlight patterns, outliers, and correlations to provide a deeper understanding of global well-being.

## Dataset Overview
This dataset was prepared using data from the following trusted sources:

1. **[World Happiness Report 2024](https://worldhappiness.report/data/)**  
   - Contains happiness scores and rankings of countries worldwide.
   
2. **[Worldwide Governance Indicators](https://www.worldbank.org/en/publication/worldwide-governance-indicators)**  
   - Includes governance metrics like voice and accountability, political stability, government effectiveness, rule of law, and regulatory quality.

3. **[Individuals using the Internet Report](https://data.worldbank.org/indicator/IT.NET.USER.ZS?locations=;)**  
   - Represents the percentage of individuals using the internet in each country.

4. **[Gross National Income (GNI) per capita](https://data.worldbank.org/indicator/NY.GNP.PCAP.CD?locations=XL)**  
   - Provides data on GNI per capita adjusted for inflation and purchasing power parity.

5. **[United Nations Population Division](https://data.worldbank.org/indicator/SP.POP.TOTL)**  
   - Offers information on total population for each country.

6. **[Population Growth Rate (annual %)](https://data.worldbank.org/indicator/SP.POP.GROW)**  
   - Tracks the annual percentage growth in population.
  
7. **[World health statistics](https://data.who.int/)**
   - Include Under-5 Child Mortality Rate (U5MR).
     
## Sources
- **World Happiness Report 2024**  
- **World Bank Group (Worldwide Governance Indicators, Internet Usage, GNI per Capita, Population Data, and Population Growth Rate)**
- **World Health Organisation**

## Technologies Used
- **Data Preparation:** Microsoft Excel
- **Programming Language:** Python (Jupyter Notebook)
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-Learn

## Data Description
This dataset provides various indicators for countries based on their happiness report data from 2005 to 2023, including economic, social, and governance factors, along with subjective measures like life satisfaction and emotional well-being.

| **Variable**                     | **Type**     | **Values**                                               | **Description**                                                                                                    |
|-----------------------------------|--------------|----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| **Country**                       | Categorical  | 'Finland', 'USA', 'India', 'Australia', etc.              | The name of the country for which the happiness report data is recorded.                                           |
| **Region**                        | Categorical  | 'Europe', 'Asia', 'Middle-East', etc.                     | The geographical region to which the country belongs.                                                              |
| **Year**                          | Numerical    | 2005 to 2023                                              | The year of the happiness report data.                                                                              |
| **Log GDP per capita**            | Numerical    | Continuous values (e.g., 8.5, 10.2, etc.)                 | The natural logarithm of the country's GDP per capita, adjusted for purchasing power parity (PPP).                 |
| **Log GNI per capita**            | Numerical    | Continuous values (e.g., 8.1, 9.0, etc.)                  | The logarithmic transformation of Gross National Income (GNI) per capita, adjusted for cost of living differences.  |
| **GNI Classification**            | Categorical  | Low, Lower-middle, Upper-middle, High                     | Categorizes countries based on their Gross National Income (GNI) per capita into income groups.                    |
| **Total Population**              | Numerical    | Integer values (e.g., 1.2 billion, 100 million, etc.)     | The total number of people living in a country or region.                                                          |
| **Population Growth Rate (%)**    | Numerical    | Percentage values (e.g., 2.5%, 1.2%, etc.)                | The annual percentage increase in a country's population.                                                          |
| **Population Growth**             | Categorical  | Low, High, Moderate, Negative                             | Categorizes the population growth rate over a period as low, high, moderate, or negative.                          |
| **Voice and Accountability**      | Categorical  | Empowered, Limited Freedom, Oppressed                     | Measures the extent of citizens' ability to participate in selecting their government and the existence of freedoms. |
| **Political Stability**           | Categorical  | Peaceful, Fragile, Conflict-Prone                         | Reflects the likelihood of political instability, violent conflicts, and political violence.                        |
| **Government Effectiveness**      | Categorical  | Efficient, Developing, Inefficient                        | Assesses the quality of public services and the government's ability to formulate and implement policies.            |
| **Regulatory Quality**            | Categorical  | Progressive, Inconsistent, Restrictive                    | Measures the government's ability to create and enforce regulations that foster private sector development.          |
| **Rule of Law**                   | Categorical  | Just, Vulnerable, Lawless                                 | Evaluates the extent to which individuals and businesses have confidence in and follow the rule of law.              |
| **Internet Penetration**          | Categorical  | High, Moderate, Low                                       | Classifies the country based on the percentage of the population with internet access.                              |
| **Social support**                | Numerical    | Average of binary responses (0 to 1)                      | The national average of binary responses about having relatives or friends to count on in times of trouble.         |
| **Healthy life expectancy**       | Numerical    | Continuous values (e.g., 70, 80, etc.)                    | The average number of years a newborn infant would live in good health, based on mortality rates.                   |
| **Child Mortality**               | Categorical  | High, Moderate, Low                                       | The number of deaths of children under five years of age per 1,000 live births, reflecting child health.            |
| **Freedom to make life choices**  | Numerical    | Average of binary responses (0 to 1)                      | The national average of responses regarding satisfaction with freedom to choose life decisions.                     |
| **Generosity**                    | Numerical    | Average of binary responses (0 to 1)                      | A residual value of national charity donations, regressed on GDP per capita.                                        |
| **Perceptions of corruption**     | Numerical    | Average of binary responses (0 to 1)                      | The national average of survey responses regarding perceived corruption in government and businesses.               |
| **Positive affect**               | Numerical    | Average of binary responses (0 to 1)                      | The national average of responses about positive emotions experienced yesterday.                                    |
| **Negative affect**               | Numerical    | Average of binary responses (0 to 1)                      | The national average of responses about negative emotions experienced yesterday.                                    |
| **Life Ladder score**             | Numerical    | Continuous scale (e.g., 0 to 10)                          | The happiness score based on responses to the Cantril Ladder question, where 10 is the best possible life and 0 is the worst. |

## Results Summary

### 1. Life Ladder Score Prediction
**Best Model:** RandomForestRegressor  
- **Test R²:** 0.856 (excellent generalization).  
- **MSE:** 0.178 (minimal error).  
- **MAE:** 0.321 (low average error).  
- **Overfitting:** Minimal (Train R²: 0.851).  

**Alternatives:** GradientBoostingRegressor and XGBRegressor are strong options but slightly less accurate.  

### 2. Healthy Life Expectancy Prediction
**Best Model:** RandomForestRegressor  
- **Test R²:** 0.916 (outstanding generalization).  
- **MSE:** 3.63, **MAE:** 1.27 (low errors).  
- **Overfitting:** Balanced (Train R²: 0.852).  

**Alternatives:** XGBRegressor performs similarly but with slightly higher errors.  

**Final Recommendation:**  
RandomForestRegressor is the best model for both tasks, delivering high accuracy, minimal errors, and excellent generalization.

