# Country's Success to Education Quality Analysis (DSA 210 Project)

## Project Overview and Motivation
My goal is to analyze how a country's education is effected from its GDP per capita, income classification, GINI scores, effective governence, and educational spending. I will use PISA test scores as an indicator to check how these features affect education. 

I will be using PISA score for each country from the years 2000, 2003, 2006, ..., 2018,2022. PISA science, reading, math and combined total scores for both boys and girls will be looked at. These scores will be compared with rest of the features to see if there is any significant relationship. I am interested in this topic because education covers a huge portion in our lives so I wanted to look at factors that affect the education quality.

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
- Do countries with higher GDP have higher PISA scores?
- Does a country's region have any correlation with its PISA scores?
- Do girls and boys do better at different subjects, do they have similar overall results?
- Do countries with higher education spending have higher PISA scores?
- Does GINI score have correlation with mean total PISA scores?
---
### Hypotheses 

**H₀:** Girls mean and boys mean for PISA reading scores are the same.  
**H₁:** Girls mean PISA reading scores are higher than boys.  

**H₀:** Girls mean and boys mean for PISA math scores are the same.  
**H₁:** Girls mean PISA math scores are different than boys mean.  

**H₀:** Girls mean and boys mean for PISA science scores are the same.  
**H₁:** Girls mean PISA science scores are different than boys mean.  

**H₀:** The total PISA score mean is identical across all four income groups.  
**H₁:** At least one income group has a different total PISA score mean.  

**H₀:** The mean total PISA scores for high and lower-middle income countries are the same.  
**H₁:** There is significant difference between the mean total PISA scores for high and lower-middle income countries.

**H₀:** The mean total PISA scores for high income and other income groups are the same. 
**H₁:** There is significant difference between the mean total PISA scores for high income and other income groups.  

**H₀:** The mean total PISA score is identical across all five world regions.  
**H₁:** At least one world region has a significantly different mean total PISA score.

**H₀:** The mean total PISA score for Europe and Africa are the same.  
**H₁:** Europe's mean total PISA score is significantly higher than Africa's.

**H₀:** The mean total PISA score for South America and North America are the same.  
**H₁:** The mean total PISA score for South America and North America are significantly different.




---
### Methods 
- I will use hypothesis testing and EDA to answer the research questions.
- For machine learning, multiple regression could be used to predict PISA score outcomes of the countries using their GDP, education spending and income group. 

### Python Methods
- Numpy and Pandas will be used to clean the data and to transform it to useful format.
- Matplotlib will be used to visualise the data. Interesting findings, average scores, changes in the data will be shown using graphs.
- SciPy will be used to perform hypothesis testing. For chi square, t-test and ANOVA. 

---
## EDA and Hypothesis Testing


![Gender Score Differences by Subject across PISA Years](https://github.com/user-attachments/assets/22251069-2d70-4f31-b8bf-5fabbf342444)




*   With this graph, I wanted to see if there are any score differences for reading, science and mathematics scores for boys and girls.
    * Subject score differences (girls-boys) are plotted for each year PISA score is taken
    * Difference= subject.girls – subject.boys, subject = ‘Science’, ‘Math’, ‘Reading’, ‘Total’

* It seems that girls are on average scoring higher on reading, so I will apply 1-tailed t test to see if this difference is significant.

* Science and Math scores look nearly the same, so I will apply 2-tailed t test to see if there is a difference.

***

### Hypothesis Testing

* **Significance level alpha = 0.05 will be used for all the tests.**

**H₀:** Girls mean and boys mean for PISA reading scores are the same.  
**H₁:** Girls mean PISA reading scores are significantly higher than boys.

**H₀:** μ girls − μ boys = 0  
**H₁:** μ girls > μ boys


**Method:** One-tailed independent t-test is used.
* t = 10.623, one-tailed p = 0.0000
   * P-value is smaller than 0.05, null hypothesis is rejected. 
   * There is significant evidence that girls mean PISA reading scores are higher than boys.
***

**H₀:** Girls mean and boys mean for PISA math scores are the same.  
**H₁:** Girls mean PISA math scores are significantly different than boys mean.

**H₀:** μ girls − μ boys = 0  
**H₁:** μ girls - μ boys ≠ 0


**Method:** Two-tailed independent t-test is used.
* t = -1.412, two-tailed p = 0.1581
   * Two tailed p-value is bigger than 0.05, fail to reject null hypothesis. 
   * Not enough evidence to say girls and boys mean PISA math scores are different.

***
**H₀:** Girls mean and boys mean for PISA science scores are the same.  
**H₁:** Girls mean PISA science scores are significantly different than boys mean.

**H₀:** μ girls − μ boys = 0  
**H₁:** μ girls - μ boys ≠ 0

**Method:** Two-tailed independent t-test is used.

* t = 1.246, two-tailed p = 0.2129
   * Two tailed p-value is bigger than 0.05, fail to reject null hypothesis. 
   * Not enough evidence to say girls and boys mean PISA science scores are different.


* Hypothesis tests showed that while there is a difference between reading scores between boys and girls, math and science score differences are not statistically significant.
****

![Score Distribution by Income Level](https://github.com/user-attachments/assets/9222a0fe-c4ce-4c10-be81-9e5933580b38)


******************************************
**H₀:** The mean total PISA score is identical across all four income groups.  
**H₁:** At least one income group has a significantly different mean total PISA score.  

**Method:** ANOVA is used since more than two means are compared.

* f-statistic = 245.359 p-value = 0.0000
   * P-value is smaller than 0.05, null hypothesis is rejected. 
   * At least one of the income groups mean is different than the others.

* Result from ANOVA support the visual difference income groups have in the graph.

***

![Distribution of PISA Scores by Income Group-1](https://github.com/user-attachments/assets/934819cd-8785-406e-afb4-c31cd9540a9b)

* From these graphs there seems to be a significant PISA score difference between high income and lower-middle income countries. Also other combinations of income groups will be subject to hypothesis testing to see the relation.

******************************************
**H₀:** The mean total PISA scores for high and lower-middle income countries are the same.  
**H₁:** There is significant difference between the mean total PISA scores for high and lower-middle income countries.

**Method:** Two-tailed independent t test is used.
* t-statistic = 24.146 two-tailed p-value = 0.000
   * P-value is smaller than 0.05, null hypothesis is rejected. 
   * There is significant difference between mean total PISA scores of high and lower-middle income countries. Higher income countries have higher PISA scores.


****
* It is clear that there is a difference after hypothesis testing, now I will check other income groups and see if such a difference will persist.
***



![Distribution of PISA Scores by Income Group-2](https://github.com/user-attachments/assets/89fb1fcb-643d-445c-9330-daa9cba0df98)

****

**H₀:** The mean total PISA scores for high income and other income groups are the same.  
**H₁:** There is significant difference between the mean total PISA scores for high income and other income groups.

**Method:** Two-tailed independent t test is used.
* t-statistic = 26.024 two-tailed p-value = 0.0000
   * P-value is smaller than 0.05, null hypothesis is rejected.  
   * There is significant difference between mean total PISA scores of high and lower-middle income countries. Higher income countries have higher PISA scores.
     
***
* There is significant difference  when High income and lower-middle income are compared. And such a difference persist in the second t test, when high income countries are compared with other three income groups combined.   

* Higher income countries have higher PISA scores in both cases.

***


![World Region and PISA Scores](https://github.com/user-attachments/assets/489c1c60-1a99-4163-aac8-b667fd0ce90c)

* This graph shows mean total PISA score for different world regions. Below are the number of results each country has:  
   * Europe:         328  
   * Africa:         24  
   * South America:  56  
   * Oceania:        16  
   * Asia:           200  
   * North America:  80  

* Oceania is not included to ANOVA as its sample size is too small.

******************************************
**H₀:** The mean total PISA score is identical across all five world regions.  
**H₁:** At least one world region has a significantly different mean total PISA score.

**Method:** ANOVA is used since more than two means are compared.
* f-statistic = 60.702 p-value = 0.0000

   * P-value is smaller than 0.05, null hypothesis is rejected. 
   * At least one of the world regions mean is different than the others.
* Oceania is excluded from the test. But ANOVA still shows that at least 2 different world regions have different mean PISA scores.

***

**H₀:** The mean total PISA score for Europe and Africa are the same.  
**H₁:** Europe's mean total PISA score is significantly higher than Africa's.

**Method:** One-tailed independent t test is used. From the graph Europe seems to have higher scores so if there is a significant difference Europe would have higher scores.

* t = 34.472, one-tailed p = 0.0000  
   * P-value is smaller than 0.05, null hypothesis is rejected.  
   * There is significant evidence that Europe mean total PISA scores are higher than Africa's.  

***

H₀: The mean total PISA score for South America and North America are the same.  
H₁: The mean total PISA score for South America and North America are significantly different.

t = -1.713, two-tailed p = 0.0893
   * P-value is bigger than 0.05, fail to reject null hypothesis.

* Hypothesis test show that Europe and Africa has significant difference but for South America and North America there is no significant relationship between the scores.
***
![Six Socio-Economic Indicators vs PISA Total Score](https://github.com/user-attachments/assets/2e34d81f-4029-43be-8770-9f0eb2d66f73)
Note: 6 different graphs from ipynb file is combined here to save space


#### Pearson Correlation Tests with PISA total average

* All p-values are smaller than 0.05 so correlation found in these tests are unlikely to be due to random chance and are statistically significant.

***
Gender Inequality: Pearson r = -0.767, p = 0.000  
 * Gender inequality has strong negative correlation with PISA scores
   *  Gender inequality measures reproductive health, empowerment, and economic status for genders, and higher score means higher inequalities. This shows countries that have better gender equality tend to have better scores. 

GDP PPP per Capita: Pearson r = 0.568, p = 0.000  
   * GDP per capita has moderate positive correlation with PISA scores. This could mean that these countries have more resources to allocate to all matters including education hence tending to have better results.
   * Correlation between PISA scores for countries having higher vs less than 50 000 GDP per capita will be looked at in the coming section.

***
Government Education Spending %: Pearson r = -0.262, p = 0.000  
Education Spending to GDP ratio: Pearson r = 0.327, p = 0.000  
  *  Government Education Spending % show how much of the governments total spending goes to education, and Education Spending to GDP ratio shows the share of GDP that is spent on public education.
  *  There is a weak but statistically significant negative correlation between government education spending % and PISA scores, indicating that countries allocating a larger share of total government expenditure to education tend to have slightly lower average PISA scores.
  *  Whereas Education Spending to GDP ratio has again weak, but this time positive correlation with mean total PISA Scores.
  *  These show that allocating a larger portion of a government’s budget to education doesn’t necessarily correlate with higher scores, and countries investing a larger portion of their economic output in education tend to achieve slightly higher PISA scores. But both correlations are weak to do much inference.
***
Expected School Years: Pearson r = 0.691, p = 0.000    
   * Expected school years and PISA scores have strong positive correlation. 
     
Human Development Index: Pearson r = 0.788, p = 0.000  
  * HDI aims to measure long and healthy life, good education, and decent standard of living. By factoring life expectancy at birth, expected and mean years of schooling and GNI per capita.   
     * Since it also has schooling years HDI is expected to have positive correlation with PISA scores (from the correlation test for expected school years (r = 0.691)). But it also shows higher correlation than 0.69 so it indicates that life expectancy and stardard of living also have some positive correlation with PISA scores.

***
Corruption Index: Pearson r = -0.746, p = 0.000  
* Corruption Index measures the corruption in that country's government, and higher scores mean more corruption. Since corruption index has strong negative corrrelation with PISA scores, countries that have transparent governments tend to have higher PISA scores.  

 

***

![PISA Total Score vs GDP per Capita (Bubble Size = GINI Index) 2022 ](https://github.com/user-attachments/assets/72bfcd1a-b1fb-415a-bb22-8ccf84c55573)


* From the PISA scores and GDP graph, it looks like GDP increase is correlated with higher PISA scores. But this effect seems to stop for GDP's higher than 50 000. That is why I used Pearson correlation test to see GDP's correlation with PISA scores for above and below 50 000 GDP per capita.  
   * Higher-GDP subset: Pearson r = -0.220, p = 0.002  
   * Lower-GDP subset: Pearson r = 0.741, p = 0.000  
   * For both subsets p-value < 0.05 so both correlations are statistically significant.

* Looking at the Higher GDP subset's Pearson correlation test, the correlation with PISA scores is weak and it is negatively corelated.

   * So after 50 0000, GDP increase does not have a positive correlation with PISA scores, it even seems to slightly decrease but correlation is weak.  

* On the otherhand, for Lower-GDP subset, GDP has strong positive correlation with PISA scores. So within this subset, countries having higher GDP tend to have higher PISA scores and the correlation is quite strong, unlike the other subset (GDP over 50 000).

* These findings show even though GDP correlates with higher scores, this is not the case when GDP goes above 50 000 per capita.

***
* From the graph higher PISA scoring countries seem to have lower GINI scores so Pearson correlation test is done to see the significance.

GINI Coefficient: Pearson r = -0.504, p = 0.000  
* GINI coeficient increase has moderate negative correlation with PISA scores.
* Higher GINI coefficient means higher income inequality. So the countries with lower GINI coefficient, therefore having more equal income distributions, tend to have higher PISA scores. This finding supports the graph.

***


![Correlation Matrix](https://github.com/user-attachments/assets/95564663-0018-45ac-b8dd-ee191923b9d4)

* From this matrix it is again visible that education spending ratio to GDP and government education spending percentage has lowest correlation with total PISA score averages.  


* Whereas gender inequality, corruption index have strongest negative correlation and HDI has strongest positive correlation with PISA scores.  
  * There are also highly correlated features like gender inequality and average school years or HDI and corruption index, these will be looked at while applying machine learning.


## Machine Learning 

### K-Nearest Neighbours Regression


* If features are not standardized, then larger scaled values will affect the results more than the smaller scaled values when finding the nearest neighbours. Because of this reason, before features are used, they are standardized for KNN.  

* Target value PISA scores will be kept as is.
  
![image](https://github.com/user-attachments/assets/82375460-225a-4fd4-9d7d-4de185d0eddc)
* When different number of neighboors are compared, k=1 gives the lowest MSE. But there is a risk of overfitting if k is picked as 1.

> MSE at k=1: 468.330  
> RMSE at best k=1: 21.641

* Therefore, I plotted another graph to see how different train and validation MSE's are.  
 * As seen in the graph, MSE is ~0 for k=1 in training set and ~300 for validation set. This means there is overfitting.  
 * Because of this even though k=1 lowers the MSE, it looks better to choose k around 5 to 8.

> MSE for k = 5, ..., 8:  
>  k = 5: MSE = 676.412, RMSE = 26.008   
>  k = 6: MSE = 710.845, RMSE = 26.662  
>  k = 7: MSE = 727.382, RMSE = 26.970  
>  k = 8: MSE = 756.822, RMSE = 27.510  

* From these 6 could be chosen to reduce overfitting while getting a relatively lower MSE/RMSE.

---
### Decision Tree


![image](https://github.com/user-attachments/assets/2dd67c25-2338-484f-8c82-9b5508dec3ff)

* Here is a decision tree with min_samples_leaf = 1, and mean_samples_split = 2, and the graph shows how different max_depth affects the model.

* With these hyperparameters best max_depth is 9. And corresponding MSE and RMSE are as follows:      
  * MSE = 847.882 
  * RMSE = 29.118

* Increasing max depth also increases the complexity of the model. Since largest decrease happens before 6. And max_depth = 6 produces very similar results to depth 9, so I will choose 6 as my max depth.
 
* For max_depth = 6:  
  * MSE: 872.777 
  * RMSE: 29.543 


* I will now try different split and leaf sizes to see if they will improve the predictions.

---

![image](https://github.com/user-attachments/assets/cdb3cac5-86ef-4729-927f-bd4c8d87e7e9)

* Choosing min_samples_split = 2 and min_samples_leaf = 7 improved the results further. 

* For min_samples_split = 2 and min_samples_leaf = 8 and max_depth = 6:   
  * MSE: 653.65
  * RMSE: 25.567

* These results are better than comparing with only tuning max_depth hyperparameter.

---
### XGBoost Regression

Before hyperparameter tuning with default values:
* MSE per Fold
| Fold             | MSE     |
|:----------------:|:-------:|
|  1               | 266.63  |
|  2               | 351.95  |
|  3               | 545.95  |
|  4               | 454.79  |
|  5               | 465.95  |
| **Mean MSE**     | **417.05** |

---

* RMSE per Fold

| Fold           | RMSE    |
|:--------------:|:-------:|
|  1              | 16.33   |
|  2              | 18.76   |
|  3              | 23.37   |
|  4              | 21.33   |
|  5              | 21.59   |
| **Mean RMSE** | **20.42** |

---
Fitting 5 folds for each of 100 candidates, totalling 500 fits

*  Best Parameters

| Parameter      | Value |
| -------------- | ----- |
| **learning_rate** | 0.1   |
| **max_depth**     | 5     |
| **n_estimators**  | 500   |

* Cross-Validation Performance

| Metric        | Value  |
| ------------- | ------ |
| **CV MSE**    | 371.77 |
| **CV RMSE**   | 19.28  |

---
![image](https://github.com/user-attachments/assets/158f1509-1519-4b12-8530-aa6252954a47)
* HDI score is calculated using 3 features: healthy life, knowledge and decent standard of living. So this feature seems to encapsulate important information for PISA score prediction.   

* Europe contains many high scoring countries so having a huge importance in XGB could be expected.


---
## Limitations and Future Work

- I am only looking at a limited number of features. Many different factors like cultural tendencies, family relationships, historical importance given to education can affect students performance. These features would be hard to quantify and they are not included in this analysis.
- On top of these, immediate investments a country makes to education may produce long term results. Since I am working with currently available data and limited time frame of 22 years, such improvements may not be directly seen.
- For future work, long term effects can be analyzed to have a broader view, and more features can be added. Countries can be individually analyzed according to their historical educational backgrounds.
---



