## **Global Well-Being Prediction from World Happiness Report**

## Objective
The objective of this project is to analyze and predict global happiness scores and direction (increase or decrease) over year by examining various socioeconomic and psychological factors that influence people's well-being across countries. By exploring the relationships between indicators such as GDP per capita, social support, health, freedom of life choices, generosity, and perceptions of corruption, the project aims to identify the key drivers of happiness and uncover patterns in global well-being. This analysis can provide valuable insights for policymakers, organizations, and researchers working to enhance societal well-being and improve quality of life globally.

## Specific Goals

### 1. Understand the Drivers of Happiness
- Explore how factors like GDP, social support, health, and freedom contribute to happiness levels across different countries and regions.
- Identify the key socioeconomic and psychological factors that most influence happiness scores globally.

### 2. Identify Global Trends
- Analyze trends in happiness scores globally and regionally.
- Identify regions or countries with consistently high or low happiness levels.

### 3. Predict Happiness Scores
- Build predictive models using machine learning techniques to forecast happiness scores based on available features like GDP, social support, and other socio-economic variables.
- Compute the change in "Life Ladder Score" over years for each country and predict the direction (increase or decrease).

### 4. Assess the Role of Governance and Perception
- Investigate the influence of governance factors such as freedom and perceptions of corruption on happiness.
- Analyze how governance correlates with other metrics influencing happiness scores.

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

## Data Description

This dataset encompasses various indicators that influence happiness across countries from 2005 to 2023. Below is a brief explanation of the key columns:

- **Country**: Name of the country.
- **Region**: Region to which the country belongs.
- **Year**: The year of the happiness report data (e.g., 2019, 2020, etc.).
- **Log GDP per capita**: The natural logarithm of the country's GDP per capita, adjusted for purchasing power parity (PPP) to account for differences in the cost of living between countries.
- **Log GNI per capita**: Represents the logarithmic transformation of Gross National Income (GNI) per capita, used to analyze income distribution and economic trends.
- **GNI Classification**: Categorizes countries based on their Gross National Income (GNI) per capita into low, lower-middle, upper-middle, or high-income groups.
- **Total Population**: The total number of people living in a specific country or region at a given time.
- **Population Growth Rate**: Indicates the annual percentage increase in a country's population, reflecting birth and death rates as well as migration.
- **Population Growth**: Categorizes a country's population Growth over a period of  time as low, high, moderate or negative.
- **Voice and Accountability** - Measures the extent to which a country's citizens are able to participate in selecting their government and the extent to which freedom of expression, freedom of association, and a free media exist.
- **Political Stability** - Reflects the likelihood of political instability and the occurrence of violent conflicts, including terrorism, political violence, and civil wars.
- **Government Effectiveness** - Assesses the quality of public services, the civil service's competence, and the government's ability to formulate and implement policies effectively.
- **Regulatory Quality** - Measures the ability of the government to formulate and implement sound policies and regulations that promote private sector development.
- **Rule of Law** - Evaluates the extent to which individuals and businesses have confidence in and abide by the rules of society, including the protection of property rights and the enforcement of contracts.
- **Internet Penetration** - Classifies the Country with access to the internet in a given country or region.
- **Social support**: The national average of binary responses (either 0 or 1 representing No/Yes) to the question about having relatives or friends to count on in times of trouble.
- **Healthy life expectancy**: The average number of years a newborn infant would live in good health, based on mortality rates and life expectancy at different ages.
- **Child Mortality**: The number of deaths of children under five years of age per 1,000 live births, reflecting child health and healthcare quality.
- **Freedom to make life choices**: The national average of responses to the question about satisfaction with freedom to choose what to do with one's life.
- **Generosity**: The residual of regressing the national average of responses to the question about donating money to charity on GDP per capita.
- **Perceptions of corruption**: The national average of survey responses to questions about the perceived extent of corruption in the government and businesses.
- **Positive affect**: The national average of responses to questions about positive emotions experienced yesterday.
- **Negative affect**: The national average of responses to questions about negative emotions experienced yesterday.
- **Life Ladder score**: The happiness score for each country, based on responses to the Cantril Ladder question that asks respondents to think of a ladder, with the best possible life for them being a 10, and the worst possible life being a 0.

