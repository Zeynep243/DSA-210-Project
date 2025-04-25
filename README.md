# Country's Success to Education Quality Analysis (DSA 210 Project)

## Project Overview and Motivation
My goal is to analyze how a country's education is effected from its GDP per capita, income classification, GINI scores, effective governence, and educational spending. I will use PISA test scores as an indicator to check how these features affect education. 

I will be using PISA score for each country from the years 2000, 2003, 2006, ..., 2018,2022. PISA science, reading, math and combined total scores for both boys and girls will be looked at. I will also look at how invesment in education changes gender gap between the countries, if higher GDP and investment results in less gender gap. I am interested in this topic because education covers a huge portion in our lives so I wanted to look at factors that affect the education quality.

---
## Data Source and Features 

* I took all of my data from World Bank, links lead to csv files to download the datasets.
* Since PISA scores are calculated in every three years, I will look at the years between 2000-22 that has PISA scores

- [World Bank Income Classification Dataset](https://ourworldindata.org/grapher/world-bank-income-groups.csv?v=1&csvType=full&useColumnShortNames=true)
  * High, low, upper-middle, lower-middle income groups for each country
    
 - [World Bank World Regions Dataset](https://ourworldindata.org/grapher/world-regions-according-to-the-world-bank.csv?v=1&csvType=full&useColumnShortNames=false)

   * World regions for counries like Europe, Asia...
 - [World Bank PISA Math Score Boy/Girl Dataset](https://ourworldindata.org/grapher/pisa-mean-performance-on-the-mathematics-scale-by-sex.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank PISA Reading Score Boy/Girl Dataset](https://ourworldindata.org/grapher/pisa-mean-performance-on-the-reading-scale-by-sex.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank PISA Science Score Boy/Girl Dataset](https://ourworldindata.org/grapher/average-performance-of-15-year-old-girls-and-boys-on-the-science-scale.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank PISA Math Average Dataset](https://ourworldindata.org/grapher/pisa-test-score-mean-performance-on-the-mathematics-scale.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Reading Average Dataset](https://ourworldindata.org/grapher/pisa-test-score-mean-performance-on-the-reading-scale.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Science Average Dataset](https://ourworldindata.org/grapher/average-performance-of-15-year-olds-on-the-science-scale.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Total Expenditure on Education Dataset](https://ourworldindata.org/grapher/total-government-expenditure-on-education-gdp.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank GDP per capita Dataset](https://ourworldindata.org/grapher/gdp-per-capita-worldbank.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World GINI Index Bank Dataset](https://ourworldindata.org/grapher/economic-inequality-gini-index.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Gender Inequality Index Dataset](https://ourworldindata.org/grapher/gender-inequality-index-from-the-human-development-report.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Share of Expenditure on Education Dataset](https://ourworldindata.org/grapher/share-of-education-in-government-expenditure.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Average Years of Schooling Dataset](https://ourworldindata.org/grapher/average-years-of-schooling.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Average Years of Schooling Male Dataset](https://ourworldindata.org/grapher/mean-years-of-schooling-male.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Average Years of Schooling Female Dataset](https://ourworldindata.org/grapher/mean-years-of-schooling-female.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Expected Years of Schooling Dataset](https://ourworldindata.org/grapher/expected-years-of-schooling.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Human Development Index Dataset](https://ourworldindata.org/grapher/human-development-index.csv?v=1&csvType=full&useColumnShortNames=false)
 - [World Bank Political Corruption Dataset](https://ourworldindata.org/grapher/political-corruption-index.csv?v=1&csvType=full&useColumnShortNames=false)

---
## Data Anaysis
### Research Questions
- Do countries with higher GDP have higher PISA scores, do they have more or less gender gap in comparison to lower GDP countries?
- Does teacher to pupil ratio affect PISA scores?
- Do countries with higher education spending have higher PISA scores?
- Does political stability and government effectiveness result in more education expenditure in ratio to GDP? Or does it increase PISA test scores?
- Does higher teacher to pupil ratio increasse PISA scores?
  
---
### Hypotheses 
**H₀:** Gender gap between high GDP countries are no different than gender gap in low GDP countries.  
**H₁:** Gender gap between high GDP countries are less than the gender gap in low GDP countries. 

**H₀:** Countries with higher GDP per capita have same overall PISA scores with lower GDP per capita countries.  
**H₁:** Countries with higher GDP per capita have higher overall PISA scores than lower GDP per capita countries.

**H₀:** The teacher-to-pupil ratio has no effect on PISA scores.  
**H₁:** Higher teacher-to-pupil ratio results in higher PISA scores.

**H₀:** The percentage of GDP spent on education do not change PISA scores.  
**H₁:** Higher percentage of GDP spent on education results in higher PISA scores.

**H₀:** Political stability and government effectiveness do not have an effect on PISA scores.  
**H₁:** Higher political stability and government effectiveness result in higher PISA scores.

---
### Methods 
- I will use hypothesis testing to answer the research questions.
- For machine learning, multiple regression could be used to predict PISA score outcomes of the countries using their GDP, education spending and teacher to pupil ratio. 

### Python Methods
- Numpy and Pandas will be used to clean the data and to transform it to useful format.
- Matplotlib will be used to visualise the data. Mean, variance and changes in the data will be shown using graphs.
- SciPy will be used to perform hypothesis testing. For chi square, t-test and ANOVA. 

---
## Limitations and Future Work

- I am only looking at a limited number of features. Many different factors like cultural tendencies, family relationships, historical importance given to education can affect students performance. These features would be hard to quantify and they are not included in this analysis.
- On top of these, immediate investments a country makes to education may produce long term results. Since I am working with currently available data and limited time frame of 6 years, such improvements may not be directly seen.
- For future work, long term effects can be analyzed to have a broader view, and more features can be added. Countries can be individually analyzed according to their historical educational backgrounds.
---



