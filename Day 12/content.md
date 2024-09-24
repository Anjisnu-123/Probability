## Topic

Introduction to freq distribution:Defination,frequency,distribution,freq dist of a variable: steps-> identify the var,determine the range,set intervals or catag,count freq,Graphical rep
of freq dist: (Bar chart,histogram,pie chart,freq polygon,cumulative freq curve:ogive): how to plot,charataeristic,Examples
  -- Freq curve and types of freq curve:normal dist,skewed dist,bimodal dist,uniform dost,exponential dist
  -- pros and cons of freq dist


### Descriptive vs inferential vs predictive analytics:  compare b/w descriptive,inferential and predictive analytics

| Aspect          | Descriptive Analytics                          | Inferential Analysis                  | Predictive Analytics                            |
|-----------------|------------------------------------------------|---------------------------------------|------------------------------------------------|
| Purpose         | Summarize and describe past data               | Make inferences about a population    | Predict future trends and behaviors            |
| Techniques      | Mean, median, mode, frequency distribution      | Hypothesis testing, regression, confidence intervals | Machine learning, regression, decision trees   |
| Data Used       | Entire dataset                                 | Sample of the population               | Historical data with a focus on trends and patterns |
| Application      | Initial data analysis and reporting             | Generalizing findings to a larger population | Strategic decision-making and forecasting      |
| Example         | Sales report summarizing                       | A/B testing for marketing campaigns    | Predicting customer churn using past behavior   |



When to use each type in data science: des, inf , pred

Descriptive analytics: intro,example,Application in data science , key technique
Inferential analytics: intro,defination, use,example,application in data science,Key technique: Hypothesis testing,reg testing,confidence intervals,sampling method
*To read: sampling methdods , shephard correction and derivation of kurtosis from there*

Predictive analytics: Introduction, defination,use,example,key techniques


#### Univariae analysis and measures

Introduction to measure central tendency,Defination of measrue of central tendency,necessity of measures of central tendency

Arithmatic mean,Geometric mean,Harmonic mean,Median,Mode: defination,formula,assumptions,inference,use in ds,example

How we choose a right measure of central tendency

| Measure of Central Tendency | Properties                                                                 | Strengths                                                  | Weaknesses                                                        | Usage Context                       | Outlier Sensitivity |
|-----------------------------|---------------------------------------------------------------------------|------------------------------------------------------------|------------------------------------------------------------------|-------------------------------------|---------------------|
| **Mean**                    | Based on all values; unique for a given dataset; reflects total sum of data points | Uses all data points; easy to compute                      | Highly sensitive to outliers; not suitable for skewed data      | Symmetric distributions; numerical data | High                |
| **Median**                  | Middle value; not affected by extreme values; divides data into two equal parts | Robust to outliers; represents center well for skewed data | Does not consider all data points; may not reflect small changes in data | Skewed distributions; ordinal data   | Low                 |
| **Mode**                    | Most frequent value; can be used with categorical data; may have multiple modes | Useful for categorical data; simple and intuitive          | May not exist in some datasets; does not use all data points     | Categorical data; nominal data      | None                |
| **Geometric Mean**         | Always less than or equal to the mean; suitable for multiplicative relationships; based on all data points | Better for proportional growth rates; less sensitive to large values compared to the mean | Cannot be used for negative or zero values; complex to compute manually | Proportional growth ratios           | Moderate            |
| **Harmonic Mean**          | Gives greater weight to smaller values; based on all data points; always the lowest mean | Best for rates and ratios; effective when dealing with inversely proportional data | Sensitive to small values; cannot be used if any value is zero or negative | Rates and ratios; speed or efficiency metrics | Moderate            |


### Dispersion: introduction,defination,necessity,use of dispersion in ds and AI
Types of measure in dispersion: Range,IQR,variance,std deviation,mean absolute deviation:def,formula,inference,use in data science,use in data science ,example

| Measure             | When to Use                                         | Considerations                                                  |
|---------------------|-----------------------------------------------------|----------------------------------------------------------------|
| **Range**           | When you need a quick assessment of variability     | Sensitive to outliers                                          |
| **Interquartile Range (IQR)** | When dealing with skewed data or outliers     | Provides a robust measure of the spread of the middle 50% of the data, minimizing outlier effects |
| **Variance**        | For normally distributed data to understand overall variability | Sensitive to outliers; better for datasets without extreme values |
| **Standard Deviation (SD)** | When you need a measure of spread in the same units as the data | Sensitive to outliers; ideal for normally distributed data     |
| **Mean Absolute Deviation (MAD)** | When you want a robust measure of dispersion that reduces the effect of outliers | Less influenced by extreme values, providing a clear deviation from the mean |
| **Coefficient of Variation (CV)** | When comparing the relative variability of datasets with different units or means | A unitless measure; useful for assessing risk in finance or comparing variability across different datasets |


| Measure                   | Properties                                       | Strengths                                              | Weaknesses                                              | Usage Context                               | Outlier Sensitivity     |
|---------------------------|-------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|--------------------------------------------|-------------------------|
| **Range**                 | Simple to calculate; uses only extreme values   | Quick overview of data spread                          | Highly sensitive to outliers; can be misleading        | Initial data exploration; quick summary   | Very sensitive          |
| **Interquartile Range (IQR)** | Focuses on central 50% of data; robust measure | Less affected by outliers; represents central spread  | Does not account for extreme values; can overlook variability | Box plots; detecting outliers              | Low sensitivity         |
| **Variance**              | Measures spread using squared differences        | Useful for statistical analysis; foundational for inferential statistics | Sensitive to outliers; units are squared                | In-depth data analysis; inferential statistics | High sensitivity        |
| **Standard Deviation (SD)** | Derived from variance; same units as data      | Provides context to variance; intuitive interpretation  | Sensitive to outliers; can misrepresent spread in skewed data | Data analysis; quality control              | High sensitivity        |
| **Mean Absolute Deviation (MAD)** | Uses absolute differences; intuitive         | Less sensitive to outliers; easier to interpret       | May not capture variability as well as variance         | Robust analysis; general data description   | Moderate sensitivity     |
| **Coefficient of Variation (CV)** | Standardized measure; expresses dispersion relative to the mean | Useful for comparing datasets with different units or means | Can be misleading if the mean is near zero             | Comparing variability across different datasets | Moderate sensitivity     |


### Moments: defination,types:raw,central,Moments aboit an arbitary point

Skewness: Intro,formula for moment based skewness,other measures of skewness: Pearsons 1st coefficient of skewness(mode based),pearsons second cofficient of skewness (Median based),interpretation of skewness

Kurtosis: Introduction,formula for moment based kurtosis,other measure of kurtosis:Excess kurtosis,sample based formula,interpretation of kurtosis: meso kurtic,lepto kurtick,platykurtic

## bivariate analysis: most common pairs: Numerical vs numericsl,catag vs catag,catag vs numerical ,numerical vs time,catag vs time

Numerical vs numerical: Defination,why use scatter plot,how to interpret,where to apply:financial,health data,inference, Corelation anaysis: defination of corelation,Mathematical formula:pearson correlation coefficient(very detiled explaination with example),Spearmans rank correlation coefficient
