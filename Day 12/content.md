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

#### bivariate analysis: most common pairs: Numerical vs numericsl,catag vs catag,catag vs numerical ,numerical vs time,catag vs time

Numerical vs numerical: Defination,why use scatter plot,how to interpret,where to apply:financial,health data,inference, Corelation anaysis: defination of corelation,Mathematical formula:pearson correlation coefficient(very detiled explaination with example),Spearmans rank correlation coefficient,Kendall's tau correlation coefficient: Mathemtaical formula-> count concordant and discordant pair(calculation),kendals tau formula,Interpretation,example calculation

Types of corelation: positive corelation,negative corr,no corr,linear corr,non linear corr,perfect corr,partial corr: charateristics,examples

Usage of correlations: Predective analysis,quality control,finance and economics,social science,health science,markting research ,enviromental studies,education: usage interpretation,examples.






# Data Analysis and Visualization Concepts

This repository covers various concepts related to data analysis and visualization, including:

## 1. Introduction to Frequency Distribution

- **Definition of Frequency Distribution**: Frequency distribution refers to the tabular or graphical representation of the distribution of a variable, showing the number of observations (frequency) within each of several non-overlapping intervals or classes.
- **Steps to Calculate Frequency Distribution**:
  1. Identify the variable of interest.
  2. Determine the range (difference between the highest and lowest values) of the variable.
  3. Set the intervals or categories for the variable.
  4. Count the frequency (number of observations) for each interval or category.
  5. Represent the frequency distribution graphically.
- **Graphical Representation of Frequency Distribution**:
  - Bar Chart: Displays the frequencies as vertical bars, useful for both numerical and categorical variables.
  - Histogram: Similar to a bar chart, but the bars are contiguous, representing a continuous variable.
  - Pie Chart: Displays the relative frequencies as slices of a circle, useful for categorical variables.
  - Frequency Polygon: Connects the midpoints of the top of the bars in a histogram, forming a polygonal line.
  - Cumulative Frequency Curve (Ogive): Plots the cumulative frequencies, showing the proportion of the data below a certain value.
- **Types of Frequency Curves**:
  - Normal Distribution: A symmetric, bell-shaped curve, with equal means, medians, and modes.
  - Skewed Distribution: A distribution with one tail longer than the other, indicating an asymmetric spread of the data.
  - Bimodal Distribution: A distribution with two distinct peaks, indicating the presence of two dominant subgroups within the data.
  - Uniform Distribution: A distribution where all values within a range have an equal probability of occurrence.
  - Exponential Distribution: A distribution with a decreasing probability density function, often seen in waiting times or failure rates.
- **Pros and Cons of Frequency Distribution**:
  - Pros: Provides a clear visualization of the distribution of a variable, helps in identifying patterns, and supports decision-making.
  - Cons: Can be affected by the choice of intervals or categories, may not accurately represent the underlying distribution, and can be sensitive to outliers.

## 2. Descriptive, Inferential, and Predictive Analytics

| Aspect          | Descriptive Analytics                          | Inferential Analysis                  | Predictive Analytics                            |
|-----------------|------------------------------------------------|---------------------------------------|------------------------------------------------|
| Purpose         | Summarize and describe past data               | Make inferences about a population    | Predict future trends and behaviors            |
| Techniques      | Mean, median, mode, frequency distribution      | Hypothesis testing, regression, confidence intervals | Machine learning, regression, decision trees   |
| Data Used       | Entire dataset                                 | Sample of the population               | Historical data with a focus on trends and patterns |
| Application      | Initial data analysis and reporting             | Generalizing findings to a larger population | Strategic decision-making and forecasting      |
| Example         | Sales report summarizing                       | A/B testing for marketing campaigns    | Predicting customer churn using past behavior   |

- **When to Use Each Type in Data Science**:
  - **Descriptive Analytics**: Provide an initial overview and understanding of the data, often used for reporting and visualization. Examples include summarizing sales data, generating reports, and identifying patterns in customer behavior.
  - **Inferential Analytics**: Make inferences about a population based on sample data, used for hypothesis testing and drawing conclusions. Examples include A/B testing for marketing campaigns, estimating population parameters from sample data, and understanding the relationships between variables.
  - **Predictive Analytics**: Forecast future trends and behaviors based on historical data, used for strategic decision-making and forecasting. Examples include predicting customer churn, forecasting sales, and identifying risk factors in financial or healthcare data.

## 3. Measures of Central Tendency

### Arithmetic Mean
- **Definition**: The arithmetic mean is the sum of all the values in the dataset divided by the total number of values.
- **Formula**: `Arithmetic Mean = (Sum of all values) / (Total number of values)`
- **Assumptions**: The dataset should be numerical and continuous.
- **Inference**: The arithmetic mean represents the central value of the dataset and is influenced by all the data points.
- **Use in Data Science**: The arithmetic mean is a widely used measure of central tendency in data analysis, regression modeling, and statistical inference.
- **Example**: Consider the dataset `[5, 10, 15, 20, 25]`. The arithmetic mean would be calculated as `(5 + 10 + 15 + 20 + 25) / 5 = 15`.

### Geometric Mean
- **Definition**: The geometric mean is the nth root of the product of n values in the dataset.
- **Formula**: `Geometric Mean = (Product of all values)^(1/n)`, where n is the total number of values.
- **Assumptions**: The dataset should contain only positive values, and the values should have a multiplicative relationship.
- **Inference**: The geometric mean is always less than or equal to the arithmetic mean and is suitable for data with proportional growth rates.
- **Use in Data Science**: The geometric mean is useful for analyzing percentage changes, growth rates, and other multiplicative relationships in data.
- **Example**: Consider the dataset `[2, 4, 8, 16]`. The geometric mean would be calculated as `(2 * 4 * 8 * 16)^(1/4) = 8`.

### Harmonic Mean
- **Definition**: The harmonic mean is the reciprocal of the arithmetic mean of the reciprocals of the values in the dataset.
- **Formula**: `Harmonic Mean = n / (1/x1 + 1/x2 + ... + 1/xn)`, where n is the total number of values.
- **Assumptions**: The dataset should contain only positive values, and the values should have an inverse or reciprocal relationship.
- **Inference**: The harmonic mean gives greater weight to smaller values and is always the lowest among the three means (arithmetic, geometric, and harmonic).
- **Use in Data Science**: The harmonic mean is useful for rates and ratios, such as speed or efficiency metrics.
- **Example**: Consider the dataset `[2, 4, 8, 16]`. The harmonic mean would be calculated as `4 / (1/2 + 1/4 + 1/8 + 1/16) = 4.8`.

### Median
- **Definition**: The median is the middle value when the dataset is arranged in order (either ascending or descending).
- **Formula**: To find the median, first arrange the dataset in order, then:
  - If the dataset has an odd number of values, the median is the middle value.
  - If the dataset has an even number of values, the median is the average of the two middle values.
- **Assumptions**: The dataset can be numerical or ordinal.
- **Inference**: The median is not affected by extreme values (outliers) and represents the central value of the dataset.
- **Use in Data Science**: The median is useful for analyzing skewed data and provides a robust measure of central tendency.
- **Example**: Consider the dataset `[5, 10, 15, 20, 25]`. The median is 15, as it is the middle value in the ordered dataset.

### Mode
- **Definition**: The mode is the value that appears most frequently in the dataset.
- **Formula**: To find the mode, count the frequency of each value and identify the value with the highest frequency.
- **Assumptions**: The dataset can be numerical, ordinal, or nominal.
- **Inference**: The mode is useful for identifying the most common or typical value in the dataset and can be used with categorical data.
- **Use in Data Science**: The mode is helpful for understanding the distribution of categorical variables and can be used in clustering algorithms.
- **Example**: Consider the dataset `[5, 10, 15, 15, 20, 25]`. The mode is 15, as it appears twice, which is more than any other value in the dataset.

### Choosing the Right Measure of Central Tendency

| Measure of Central Tendency | Properties                                                                 | Strengths                                                  | Weaknesses                                                        | Usage Context                       | Outlier Sensitivity |
|-----------------------------|---------------------------------------------------------------------------|------------------------------------------------------------|------------------------------------------------------------------|-------------------------------------|---------------------|
| **Mean**                    | Based on all values; unique for a given dataset; reflects total sum of data points | Uses all data points; easy to compute                      | Highly sensitive to outliers; not suitable for skewed data      | Symmetric distributions; numerical data | High                |
| **Median**                  | Middle value; not affected by extreme values; divides data into two equal parts | Robust to outliers; represents center well for skewed data | Does not consider all data points; may not reflect small changes in data | Skewed distributions; ordinal data   | Low                 |
| **Mode**                    | Most frequent value; can be used with categorical data; may have multiple modes | Useful for categorical data; simple and intuitive          | May not exist in some datasets; does not use all data points     | Categorical data; nominal data      | None                |
| **Geometric Mean**         | Always less than or equal to the mean; suitable for multiplicative relationships; based on all data points | Better for proportional growth rates; less sensitive to large values compared to the mean | Cannot be used for negative or zero values; complex to compute manually | Proportional growth ratios           | Moderate            |
| **Harmonic Mean**          | Gives greater weight to smaller values; based on all data points; always the lowest mean | Best for rates and ratios; effective when dealing with inversely proportional data | Sensitive to small values; cannot be used if any value is zero or negative | Rates and ratios; speed or efficiency metrics | Moderate            |

## 4. Measures of Dispersion

- **Introduction to Dispersion**: Dispersion refers to the spread or variability of a dataset around the measures of central tendency.
- **Types of Dispersion Measures**:
  - **Range**: The difference between the highest and lowest values in the dataset.
    - **Formula**: Range = Highest value - Lowest value
    - **When to Use**: When you need a quick assessment of variability, but it's sensitive to outliers.
  - **Interquartile Range (IQR)**: The difference between the 75th and 25th percentiles, provides a robust measure of spread.
    - **Formula**: IQR = Q3 - Q1, where Q3 is the 75th percentile and Q1 is the 25th percentile.
    - **When to Use**: When dealing with skewed data or outliers, as it provides a robust measure of the spread of the middle 50% of the data, minimizing outlier effects.
  - **Variance**: A measure of the average squared deviation from the mean, used for normally distributed data.
    - **Formula**: Variance = Σ(x - mean)^2 / (n-1), where x is each data point, mean is the arithmetic mean, and n is the total number of data points.
    - **When to Use**: For normally distributed data to understand overall variability, but it's sensitive to outliers and better for datasets without extreme values.
  - **Standard Deviation (SD)**: The square root of the variance, represents the average deviation from the mean.
    - **Formula**: Standard Deviation = √Variance
    - **When to Use**: When you need a measure of spread in the same units as the data, but it's sensitive to outliers and ideal for normally distributed data.
  - **Mean Absolute Deviation (MAD)**: The average of the absolute differences from the mean, a robust measure of dispersion.
    - **Formula**: MAD = Σ|x - median| / n, where x is each data point, median is the median of the dataset, and n is the total number of data points.
    - **When to Use**: When you want a robust measure of dispersion that reduces the effect of outliers, as it is less influenced by extreme values and provides a clear deviation from the mean.
  - **Coefficient of Variation (CV)**: A standardized measure that expresses dispersion relative to the mean, useful for comparing the relative variability of datasets with different units or means.
    - **Formula**: CV = (Standard Deviation / Mean) * 100
    - **When to Use**: When comparing the relative variability of datasets with different units or means, as it is a unitless measure that can be useful for assessing risk in finance or comparing variability across different datasets.

| Measure                   | Properties                                       | Strengths                                              | Weaknesses                                              | Usage Context                               | Outlier Sensitivity     |
|---------------------------|-------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|--------------------------------------------|-------------------------|
| **Range**                 | Simple to calculate; uses only extreme values   | Quick overview of data spread                          | Highly sensitive to outliers; can be misleading        | Initial data exploration; quick summary   | Very sensitive          |
| **Interquartile Range (IQR)** | Focuses on central 50% of data; robust measure | Less affected by outliers; represents central spread  | Does not account for extreme values; can overlook variability | Box plots; detecting outliers              | Low sensitivity         |
| **Variance**              | Measures spread using squared differences        | Useful for statistical analysis; foundational for inferential statistics | Sensitive to outliers; units are squared                | In-depth data analysis; inferential statistics | High sensitivity        |
| **Standard Deviation (SD)** | Derived from variance; same units as data      | Provides context to variance; intuitive interpretation  | Sensitive to outliers; can misrepresent spread in skewed data | Data analysis; quality control              | High sensitivity        |
| **Mean Absolute Deviation (MAD)** | Uses absolute differences; intuitive         | Less sensitive to outliers; easier to interpret       | May not capture variability as well as variance         | Robust analysis; general data description   | Moderate sensitivity     |
| **Coefficient of Variation (CV)** | Standardized measure; expresses dispersion relative to the mean | Useful for comparing datasets with different units or means | Can be misleading if the mean is near zero             | Comparing variability across different datasets | Moderate sensitivity     |

## 5. Moments

- **Definition of Moments**: Moments are statistical measures that describe the shape and characteristics of a probability distribution.
- **Types of Moments**:
  - **Raw Moments**: Describe the distribution based on the average of the raw data values.
  - **Central Moments**: Describe the distribution based on the average of the deviations from the mean.
  - **Moments about an Arbitrary Point**: Describe the distribution based on the average of the deviations from an arbitrary point.
- **Skewness**:
  - **Introduction to Skewness**: Skewness is a measure of the asymmetry of the probability distribution of a random variable about its mean.
  - **Formula for Moment-Based Skewness**: `Skewness = (Σ(x - mean)^3) / (n * standard deviation^3)`, where x is each data point, mean is the arithmetic mean, n is the total number of data points, and standard deviation is the standard deviation of the dataset.
  - **Other Measures of Skewness**: Pearson's First Coefficient of Skewness (mode-based) and Pearson's Second Coefficient of Skewness (median-based)
  - **Interpretation of Skewness**: Positive skewness indicates a longer right tail, negative skewness indicates a longer left tail, and zero skewness indicates a symmetric distribution.
- **Kurtosis**:
  - **Introduction to Kurtosis**: Kurtosis is a measure of the "peakedness" or "flatness" of the probability distribution of a random variable.
  - **Formula for Moment-Based Kurtosis**: `Kurtosis = (Σ(x - mean)^4) / (n * standard deviation^4) - 3`, where x is each data point, mean is the arithmetic mean, n is the total number of data points, and standard deviation is the standard deviation of the dataset.
  - **Other Measures of Kurtosis**: Excess Kurtosis (subtracts 3 from the formula) and Sample-Based Kurtosis Formula
  - **Interpretation of Kurtosis**: Mesokurtic distribution (normal distribution) has a kurtosis of 3, leptokurtic distribution has a kurtosis greater than 3 (more peaked), and platykurtic distribution has a kurtosis less than 3 (flatter).

## 6. Bivariate Analysis

- **Most Common Pairs**:
  - Numerical vs. Numerical
  - Categorical vs. Categorical
  - Categorical vs. Numerical
  - Numerical vs. Time
  - Categorical vs. Time
- **Numerical vs. Numerical**:
  - **Scatter Plot**: Visualizes the relationship between two numerical variables by plotting the data points on a coordinate plane.
  - **Correlation Analysis**:
    - **Pearson Correlation Coefficient**: Measures the linear relationship between two variables, ranging from -1 (perfect negative correlation) to +1 (perfect positive correlation).
## 6. Bivariate Analysis

- **Most Common Pairs**:
  - Numerical vs. Numerical
  - Categorical vs. Categorical
  - Categorical vs. Numerical
  - Numerical vs. Time
  - Categorical vs. Time
- **Numerical vs. Numerical**:
  - **Scatter Plot**: Visualizes the relationship between two numerical variables by plotting the data points on a coordinate plane. The position of the points can reveal the presence and direction of a relationship between the variables.
  - **Correlation Analysis**:
    - **Pearson Correlation Coefficient**: Measures the linear relationship between two variables, ranging from -1 (perfect negative correlation) to +1 (perfect positive correlation). The closer the value is to 1 or -1, the stronger the linear relationship.
    - **Spearman's Rank Correlation Coefficient**: Measures the monotonic relationship between two variables, which means the variables tend to change together but not necessarily in a linear fashion. It is a non-parametric measure that does not require the variables to be normally distributed.
    - **Kendall's Tau Correlation Coefficient**: Measures the ordinal association between two variables. It is based on the number of concordant and discordant pairs in the data, providing a measure of the degree of correspondence between the rankings of the two variables.
  - **Types of Correlation**:
    - **Positive Correlation**: As one variable increases, the other variable also increases.
    - **Negative Correlation**: As one variable increases, the other variable decreases.
    - **No Correlation**: There is no discernible relationship between the two variables.
    - **Linear Correlation**: The relationship between the variables can be described by a straight line.
    - **Non-Linear Correlation**: The relationship between the variables cannot be described by a straight line.
    - **Perfect Correlation**: The variables are perfectly related, either positively or negatively.
  - **Usage and Interpretation of Correlations**:
    - **Predictive Analysis**: Correlations can be used to predict the value of one variable based on the value of another variable.
    - **Quality Control**: Correlations can help identify relationships between variables that may indicate quality issues or process problems.
    - **Finance and Economics**: Correlations are used to analyze the relationships between financial and economic variables, such as stock prices, interest rates, and inflation.
    - **Social Science**: Correlations are used to study the relationships between social and behavioral variables, such as education, income, and crime rates.
    - **Health Science**: Correlations are used to investigate the relationships between health-related variables, such as diet, exercise, and disease risk.
    - **Marketing Research**: Correlations are used to analyze the relationships between marketing variables, such as advertising, sales, and customer satisfaction.
    - **Environmental Studies**: Correlations are used to study the relationships between environmental variables, such as pollution, climate, and biodiversity.
    - **Education**: Correlations are used to analyze the relationships between educational variables, such as test scores, attendance, and teaching methods.

When interpreting correlation coefficients, consider the following:
- A correlation coefficient of +1 indicates a perfect positive linear relationship.
- A correlation coefficient of -1 indicates a perfect negative linear relationship.
- A correlation coefficient of 0 indicates no linear relationship.
- The strength of the correlation is determined by the magnitude of the coefficient, not just the sign.
- Correlation does not imply causation. A high correlation between two variables does not necessarily mean that one variable causes the other.
- The context and domain knowledge are important when interpreting the meaning and significance of a correlation.
- Statistical significance tests can be used to determine the likelihood that the observed correlation is due to chance.
