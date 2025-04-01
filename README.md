# Country's Success to Education Quality Analysis (DSA 210 Project)

## Project Overview and Motivation
My goal is to analyze how a country's education is effected from its GDP, effective governence, teacher to pupil ratios and educational spending. I will use PISA test scores as an indicator to check how these features affect education. I will also look at how invesment in education changes gender gap between the countries, if higher GDP and investment results in less gender gap. I am interested in this topic because education takes a lot of our time so wanted to look at factors in a country that affect its education quality.


## Data Source and Features 

I will look at the data between years 2012-18
- PISA Performance Scores by Country
Found on Kaggle datasets: https://www.kaggle.com/datasets/thedevastator/pisa-performance-scores-by-country
  * Features: PISA reading, mathematics and sciences scores for countries between 2012-2018: I will use PISA scores as an indicator of the quality of education

- World Education Dataset
Found on Kaggle datasets: https://www.kaggle.com/datasets/bushraqurban/world-education-dataset
  * Features: Primary school enrolment, Government expenditure on education as a percentage of GDP, Primary completion rate, Pupil teacher ratio, Secondary school enrolment

- [World Bank Governance Indicator Dataset](https://www.worldbank.org/en/publication/worldwide-governance-indicators/interactive-data-access)
  * Features: Political stability, government effectiveness: I will use these features to analyze how government stability affects educational outcomes of the country

- [World Bank GDP Dataset](https://data.worldbank.org/indicator/NY.GDP.PCAP.CD)
  * Features: GDP, GDP per capita: I will use country's GDP to analyze its effects on education and education spending

## Data Anaysis
### Research Questions
- Do countries with higher GDP have higher PISA scores, do they have more or less gender gap in comparison to lower GDP countries?
- Does teacher to pupil ratio affect PISA scores?
- Do countries with higher education spending have higher PISA scores?
- Does political stability and government effectiveness result in more education expenditure in ratio to GDP? Or does it increase PISA test scores?
- Does higher teacher to pupil ratio increasse PISA scores?

### Hypotheses 
H₀: Gender gap between high GDP countries are no different than gender gap in low GDP countries. 
H₁: Gender gap between high GDP countries are less than the gender gap in low GDP countries. 

H₀: Countries with higher GDP per capita have same overall PISA scores with lower GDP per capita countries.
H₁: Countries with higher GDP per capita have higher overall PISA scores than lower GDP per capita countries.

H₀: The teacher-to-pupil ratio has no effect on PISA scores.
H₁: Higher teacher-to-pupil ratio results in higher PISA scores.

H₀: The percentage of GDP spent on education do not change PISA scores.
H₁: Higher percentage of GDP spent on education results in higher PISA scores.

H₀: Political stability and government effectiveness do not have an effect on PISA scores.
H₁: Higher political stability and government effectiveness result in higher PISA scores.


### Methods 
- I will use hypothesis testing to answer the research questions.
- For machine learning, multiple regression could be used to predict PISA score outcomes of the countries using their GDP, education spending and teacher to pupil ratio. 

#### Python Methods
- Numpy and Pandas will be used to clean the data and to transform it to useful format.
- Matplotlib will be used to visualise the data. Mean, variance and changes in the data will be shown using graphs.
- SciPy will be used to perform hypothesis testing. For chi square, t-test and ANOVA. 

## Limitations and Future Work

- I am only looking at a limited number of features. Many different factors like cultural tendencies, family relationships, historical importance given to education can affect students performance. These features would be hard to quantify and they are not included in this analysis.
- On top of these, immediate investments a country makes to education may produce long term results. Since I am working with currently available data and limited time frame of 6 years, such improvements may not be directly seen.
- For future work, long term effects can be analyzed to have a broader view, and more features can be added. Countries can be individually analyzed according to their historical educational backgrounds.




