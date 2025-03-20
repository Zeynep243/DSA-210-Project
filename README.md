# Country's Success to Education Quality Analysis (DSA 210 Project)

## Project Overview and Motivation
My goal is to analyze how a country's education is effected from its GDP, effective governence, teacher to pupil ratios and educational spending. I will use PISA test scores as an indicator to check how these features affect education. I will also look at how invesment in education changes gender gap between the countries, if higher GDP and investment results in less gender gap. I am interested in this topic because education takes a lot of our time so wanted to look at factors in a country that affect its education quality.


## Data Source and Features 

I will look at the data between years 2012-18
- PISA Performance Scores by Country
Found on Kaggle datasets: https://www.kaggle.com/datasets/thedevastator/pisa-performance-scores-by-country
* Features: PISA reading, mathematics and sciences scores for countries between 2012-2018
I will use PISA scores as an indicator of the quality of education

- World Education Dataset
Found on Kaggle datasets: https://www.kaggle.com/datasets/bushraqurban/world-education-dataset
* Features: Primary school enrolment, Government expenditure on education as a percentage of GDP, Primary completion rate, Pupil teacher ratio, Secondary school enrolment

- World Bank Governance Indicator Dataset
https://www.worldbank.org/en/publication/worldwide-governance-indicators/interactive-data-access
* Features: Political stability, government effectiveness
I will use these features to analyze how government stability affects educational outcomes of the country

- World Bank GDP Dataset
https://data.worldbank.org/indicator/NY.GDP.PCAP.CD
* Features: GDP, GDP per capita
I will use country's GDP to analyze its effects on education and education spending

## Data Anaysis
### Research Questions
- Do countries with higher GDP have higher PISA scores, do they have more or less gender gap in comparison to lower GDP countries?
- Does teacher to pupil ratio affect primary school completion rate?
- Do countries with higher education spending have higher teacher to pupil ratio?
- Does political stability and government effectiveness result in more education expenditure in ratio to GDP? Or does it increase PISA test scores?
- Does higher teacher to pupil ratio correlate with secondary and primary school enrolments?

### Methods 
- I will use hypothesis testing to answer the research questions.
- I plan to use machine learning to predict PISA score outcomes of the countries using their GDP, education spending and teacher to pupil ratio. 

#### Python Methods
- Numpy and Pandas will be used to clean the data and to transform it to useful format.
- Matplotlib will be used to visualise the data. Mean, variance and changes in the data will be shown using graphs.
- SciPy will be used to perform hypothesis testing. For chi square, t-test and ANOVA. 

## Findings


## Limitations and Future Work

- I am only looking at a limited number of features. Many different factors like cultural tendencies, family relationships, historical importance given to education can affect students performance. These features would be hard to quantify and they are not included in this analysis.

- On top of these, immediate investments a country makes to education may produce long term results. Since I am working with currently available data and limited time frame of 6 years, such improvements may not be directly seen.

- For future work, long term effects can be analyzed to have a broader view, and more features can be added. Countries can be individually analyzed according to their historical educational backgrounds.




