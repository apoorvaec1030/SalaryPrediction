Salary Prediction

Examine a set of job postings with salaries and then predict salaries for a new set of job postings

Load the data into a Pandas dataframe

Look for duplicate data, invalid data (e.g. salaries <=0), or corrupt data and remove it

Observation- 'NONE' degree has a big share in the data. It can be handled separately

Corr Notes
Correlation methods- 'pearson', 'kendall', 'spearman', Point-Biserial Pearson r correlation is the most widely used correlation statistic to measure the degree of the relationship between linearly related variables. Point-biserial correlation is conducted with the Pearson correlation formula except that one of the variables is dichotomous. Dichotomous variable- is one that takes on one of only two possible values when observed or measured. ASSUMPTIONS- For the Pearson r correlation, both variables should be normally distributed (normally distributed variables have a bell-shaped curve). Other assumptions include linearity and homoscedasticity. Linearity assumes a straight line relationship between each of the two variables and homoscedasticity assumes that data is equally distributed about the regression line. Kendall rank correlation: is a 'non-parametric' test that measures the strength of dependence between two variables.Kendall rank correlation: Kendall rank correlation is a non-parametric test that measures the strength of dependence between two variables. https://www.statisticssolutions.com/kendalls-tau-and-spearmans-rank-correlation-coefficient/ Kendall & Spearman is non-parametric test. Kendall is based on order & Ranking and discordant and concordant pairs. Hence not sensitive to error. Spearman is based on deviations hence sensitive to error.

PLOT Observation-In multivarPlot salary zero is noticed.

5 row with zero salary. Out of which 3 are CTO, Manager and VP level job types whose salaries cannot be zero. Another guy is a doctorate with 11 years of exp. Salary incorrect. Removing 4 rows.

---- 5 Establish a baseline ----
Selecting three models for salary prediction project:
1.	Continous data
2.	Dataset set is 1M rows
3.	Mix of continuous and categorical vars
Basic model & why- Linear regression- Random Forest- This will capture non-linearities as well. Light GBM & XGBoostRegressor- This has gradient boosting capability which means it can select which node to split the data at. This can help get more meaningful results
New features- Other possible features could be included:
1.	Previous salary
2.	Percent jump in salary each job switch
3.	skill set
4.	grades in major
5.	performance rating
6.	performance rating over the years
7.	Total job switch in the career





