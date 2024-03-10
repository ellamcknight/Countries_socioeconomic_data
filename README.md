# Countries_socioeconomic_data
## Countries socioeconomic analysis

Data analysis on world health & socioeconomic data. 

Analytical techniques incorporated where:
- Regression with polynomial features
- Clustering 

For this project the dataset was sourced from:
[World Bank](https://data.worldbank.org/region/world?view=chart)

### First - exploratory data analysis
1. Descriptive statistics
2. Histograms
3. Boxplots
4. Correlation matrix
5. Pairplots

*Descriptive statistics*

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/Datatable.png?raw=true)

The descriptive analysis of the dataset provides a comprehensive overview of various socio-economic and health indicators for 167 countries. 

*Here's a summary of the key statistics:*

- Child Mortality: The average child mortality rate is 38.27 deaths per 1000 live births, with a wide range from 2.6 to 208, indicating significant differences in child health and survival rates across countries.
- Exports: On average, countries export goods and services worth 41.11% of their GDP. The exports as a percentage of GDP vary greatly among countries, from as low as 0.109% to as high as 200%.
- Health Spending: Countries spend an average of 6.82% of their GDP on health. This percentage ranges from 1.81% to 17.9%, showing diverse priorities or capabilities in health expenditure.
- Imports: On average, imports account for 46.89% of the GDP, with a range from 0.0659% to 174%, indicating varying degrees of dependency on imported goods and services.
- Income: The range of income per person is 609 to 125,000 dollars.
- Inflation: The mean inflation rate is 7.78, but it varies widely from -4.21 to 104, reflecting very different economic conditions and monetary policies.
- Life Expectancy: The average life expectancy is approximately 70.56 years, with a minimum of 32.1 years and a maximum of 82.8 years, highlighting disparities in healthcare, living conditions, and access to essential services.
- Total Fertility Rate: On average, women have about 2.95 children in their lifetime, with the total fertility rate ranging from 1.15 to 7.49 children per woman.
- GDP per Capita: The range of GDP per capita is 231 to 105,000 dollars.

These statistics highlight the vast differences in economic performance, health outcomes, and demographic characteristics across countries. The data can be further analysed to explore correlations between different indicators, identify trends, and understand the factors driving differences in health, economic well-being, and development levels among countries.

*Histograms*

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/histograms.png?raw=true)

The plots above displays the distribution of various socio-economic and health indicators for countries in the dataset. Each histogram is accompanied by a Kernel Density Estimate (KDE) curve, providing a smooth estimate of the distribution. 

*Here's a brief overview of what each plot reveals:*

- Child Mortality: Most countries have a low child mortality rate, but there's a long tail indicating some countries with very high rates.
- Exports & Imports: Both show a wide range of values, with many countries clustered at the lower end, indicating a concentration of countries with lower trade as a percentage of GDP.
- Health Spending: The distribution is skewed towards lower health spending as a percentage of GDP, with fewer countries spending a higher proportion.
- Income: This plot shows a wide disparity in income per person, with a concentration of countries at the lower end of the income spectrum.
- Inflation: Most countries have relatively low inflation rates, but there are outliers with very high inflation.
- Life Expectancy: The distribution shows a skew towards higher life expectancy, with fewer countries having very low life expectancy.
- Total Fertility Rate: There's a broad spread of fertility rates, with a tendency towards lower fertility rates in many countries.
- GDP per Capita: Similar to income, there's a significant disparity in GDP per capita, with many countries concentrated at the lower end.

*Boxplots*

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/boxplots.png?raw=true)

Boxplots are particularly useful for identifying the median, quartiles, and outliers within each distribution.

*Here's a brief overview of what each plot reveals:*

- Child Mortality: There's a wide interquartile range, indicating significant variation in child mortality rates among countries. Numerous outliers suggest that some countries have exceptionally high child mortality rates.
- Exports & Imports: Both indicators have a relatively wide range but with many outliers, indicating that some countries have exceptionally high or low trade percentages relative to their GDP.
- Health Spending: The distribution shows a moderate range of health spending as a percentage of GDP, with a few countries spending significantly more, as indicated by outliers.
- Income: There's a large spread in income per person, with many outliers on the higher end, highlighting income disparity among countries.
- Inflation: Most countries have moderate inflation rates, but there are several outliers with extremely high inflation.
- Life Expectancy: The life expectancy across countries shows a skew towards higher values, but with outliers on both ends, indicating variations in health outcomes.
- Total Fertility Rate: The fertility rate shows variability among countries, with some outliers indicating very high fertility rates.
- GDP per Capita: Similar to income, there's a significant spread in GDP per capita with numerous outliers, highlighting economic disparities.

Overall, these boxplots underscore the disparities in health, economic, and demographic indicators across the countries, highlighting the range of conditions and challenges faced by different nations.

*Correlation matrix*

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/corr_matrix.png?raw=true)

The heatmap above visualizes the correlation matrix of socio-economic and health indicators in the dataset. Each cell in the heatmap shows the correlation coefficient between two variables, ranging from -1 to 1. A coefficient close to 1 indicates a strong positive correlation, meaning that as one variable increases, the other tends to increase as well. A coefficient close to -1 indicates a strong negative correlation, where an increase in one variable tends to be associated with a decrease in the other. Coefficients near 0 suggest little to no linear relationship between the variables. 

*Key insights from the correlation analysis include:*

- Income and GDP per Capita have a strong positive correlation with Life Expectancy, indicating that higher income levels and economic output per person are associated with longer life spans.
- Child Mortality is negatively correlated with Life Expectancy, Income, and GDP per Capita, suggesting that as economic conditions improve, child mortality rates tend to decrease.
- Fertility Rate shows a strong negative correlation with Life Expectancy, Income, and GDP per Capita, consistent with the trend that higher fertility rates are often observed in countries with lower income and shorterlife expectancy.
- Health Spending as a percentage of GDP shows positive correlations with Income and GDP per Capita, indicating that wealthier countries tend to spend a higher proportion of their GDP on health.
- These correlations can help identify the key drivers of health and economic outcomes across countries, guiding further analysis and policy interventions.

*Pairplots*

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/pairplot.png?raw=true)

The scatter plots above illustrate the relationships between key socio-economic and health indicators for the countries in the dataset. Each plot pairs two variables, showing how they are related to each other across different countries.

*Here are some observations:*

- Income vs. Life Expectancy: There's a positive relationship indicating that higher income per person is associated with longer life expectancy.
- Income vs. Child Mortality: A negative relationship is observed, suggesting that as income per person increases, child mortality rates tend to decrease.
- Income vs. Total Fertility Rate: Higher income levels tend to be associated with lower fertility rates.
- GDP per Capita vs. Life Expectancy and Exports: Similar to income, a higher GDP per capita is associated with longer life expectancy and increased exports.
- GDP per Capita vs. Child Mortality and Total Fertility Rate: GDP per capita shows a negative relationship with both child mortality and total fertility rate, echoing the patterns seen with income.

These patterns highlight the strong link between economic indicators and health outcomes. Wealthier countries, as measured by income and GDP per capita, typically have better health outcomes, evidenced by higher life expectancy, lower child mortality rates, and lower fertility rates. These visualisations underscore the interconnectedness of economic development and health providing valuable insights for policymakers.

##### Furthermore

Income, GDP and exports look to have a Polynomial relationship with life expectancy and will affect a linear regression model.

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/focusedpairplot.png?raw=true)

Here the variables have been plotted against life expectancy and the **non-linearity** is very clear for some of the relationships.

### Second - Explore polynomial features

The features that look like they have a polynomial relationship with the target variable (life expectancy):

- GDP per capita
- Exports
- Income
    
The features identified above were used to apply Polynomial features using sci-kit learn.

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/poly1.png?raw=true)

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/poly2.png?raw=true)

As is observed above, the degree 2 polynomial fits the data much better and was thus incorporated into the model later down in the notebook.

### Third - OLS - Ordinary Least Squares (Regression)

First, the OLS model was built using the original features (no polynomial features). The model was run through multiple iterations, each time setting a lower and lower threshold for the p-value.
This was followed by adding the polynomial features into the model and following the same step-wise deletion methods.

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/OLS_output.png?raw=true)

##### *Interpreting the model*

Regression analysis that uses polynomials to model curvature can make interpreting the results trickier. Unlike a linear relationship, the effect of the independent variable changes based on its value. Looking at the coefficients won’t make the picture any clearer. Instead, graph the data to truly understand the relationship. Expert knowledge of the study area can also help you make sense of the results.
Final model output:

**From what we know of our data's relationships we can now say this:**

The following features have a positive impact on the model outcome, suggesting that as this feature is increased, the model predicts a higher life expectancy:

- **GDP per capita**
- **Exports**

The following features have a negative impact on the model outcome, suggesting that as these features are increased, the model predicts a lower life expectancy:

- **Infant Mortality**
- **Imports**

### Forth - predictions

The last part was to see how the model would perform as a predictor using sci-kit learn. A train/test split was done, and then a regression was applied. The residuals were observed:

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/regressionresiduals.png?raw=true)

The last part was to apply regularisation techniques like ridge regularisation:

![alt text](https://github.com/ellamcknight/Countries_socioeconomic_data/blob/main/Images/ridgeresiduals.png?raw=true)

# Clustering analysis


