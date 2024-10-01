# Topic: Inferential statistics 

**Introduction to inferntial stat :** Defination: how its different from descriptive stat,Key concept: population vs sample,parameters vs stat,Goal of inferential stat: GEneralization,
hypothesis testing,estimation and predictive modeling

**Population vs sample :** Population,sample,why use a sample?
**Parameters vs stat :** Parameter,example,keypoint,Stat: example,keypoints,why is the distiction important.
**Bias vs Variability :** Bias:Types of bias,impact of bias,variability:source of variability:sampling error,natural variability,impact of variability,impact of variability,Relationship b/w bias and variability,bias vs variability,
Goal in stat: minimize the bias and control variability....

**Sampling :** Dfination,Types of sampling: Random sampling:Simple random sampling with replacement,without replacement,startified sampling,cluster sampling,systematic sampling.

**Sampling distribution :** What is sampling dist,CLT,why CLT is important,

<!--**Importance of sample size :** Why is sample size important,small samples: Higher variability ,potential bias,limited statistical power,Large samples: Reduced variability,better representation,
increased statistical error.

**Sampling distributions :** concept of sampling distribution,example,characteristic of sampling distribution

**Standard error :** defination,formula,roles of standard error: estimation of population parameters,construction of confidence intervals,Hypothesis testing
**Poiny estimation :** Defination,example of point estimates: sample mean,sample proportion

**Good point estimate properties :** Unbiasness: Defination,explanation,example,importance, Consistency: Defination,explanation,example,importance,EFFICIENCY: Def,exp,var comparison,example,
Sufficiency(additional proo): def ,math exp,example,importance


**Corelation :coefficient** def,range formula,assumptions,example,spearman's rank: def,range formula,usecaase,corelation matrix, interpreting corelation values: strong corelation > 0.7, moderate corelation 0.3<|r|<=0.7,weak corelation |r|<=0,3

**Confidence Intervals :** what is a confidence interval,component of confidence level: point estimate,margin of error,confidence level,common confidence level,trade-off,formula for population
mean: for large sample sizes,for small sample sizes,math example,confidence interval formula for population proportion

**What is the margin of error :** It is the amount added to and subtracted from the point estimate in a confidence interval,components of margin of error: critical value(z or t)standard error,
formula

**Z-Scores :** Used when population std deviation is known or sample size id large crtitical values for confidence level 90,95,99,**Tscore :** when use?,vary depends on deg of freedom,


**Hypothesis testing :**
Deifnation,Null hypothesis, alternative hypothesis

**Level of significance :** Defination,mathematical rep,interpretation,Type 1 error,example.

**Power or test :** defination,mathematical rep,type 2 error,example

**Types of error :** Type 1 error,type 2 error: defination,consequence,significance level,power of test,example

**Critical value and rejection region :**Critical value,mathematical calculation,rejection region.

# **TEST STAT**
what are test stat: defination,z-test,t-test:single sample ttest,two sample t-test,paired t-test|,chi squared test,ANOVA,

Test stat general formula for ztest and ttest.
**P-value and its interpretation :** defination,mathematical expression,decision rule,example

**Steps in hypothesis testing :** 
- define hypothesis
- select significance levels
- choose appropiate test and calculate test statistics
- Make a decision

**Parametric test :** Defination,Asssumptions of parametric tests:Normality,homogeneity of varriance,interval or ratio scale,example of parametric tests:Ztest,ttest:types(one sample ttest,independent two sample ttest,paired t test),example

**Non-parametric test :** Defination,when to use non parametric test,examples of non parametric tests: mann whitney u test,wilcoxon signed-rank test.

| Feature               | Parametric Tests                         | Non-Parametric Tests                   |
|-----------------------|------------------------------------------|----------------------------------------|
| **Assumptions**       | Assume normality and equal variances     | No specific distribution assumptions    |
| **Data Type**         | Interval or ratio                        | Ordinal, nominal, or continuous        |
| **Sample Size**       | Typically requires larger samples        | Can work with smaller samples          |
| **Power**             | Generally more powerful when assumptions are met | Less powerful but more flexible |
| **Examples**          | Z-test, T-test, ANOVA                   | Mann-Whitney U, Wilcoxon, Kruskal-Wallis |



**simple Linear regression :** Defination,equn,purpose,assumptions,example
**Multiple Linear regression :** Defination,equn,purpose,assumptions,example

**Oridanry least square(OLS) :** OBjecticve, what are residuals,why minimize squared residuals,Purpose of OLS

Formula for estimating beta1 in simple linear regression: Formula for slope,steps to calculate beta1, interpretation of beta1

**R.squared and its interpretation :** what is r squared defination,formula,interpretation,limitations of r squared

**Adjusted R^2 :** what is adjusted r^2,why use adjusted R^2,interpretation,example

**Hypothesis testing for regression coefficients :** objective,null hypothesis,alternate hypothesis,steps for testing,compatre with critical value,
decision,example


**Confidence intervals for regression parameters :** what is confidence intervals,interpreting confidence intervals,example



*To read*: BLUE(best linear unbiased estimator)
-->

# Inferential Statistics: A Comprehensive Overview

## Introduction to Inferential Statistics

### Definition
Inferential statistics involves using data from a sample to make inferences or generalizations about a population. It differs from descriptive statistics, which merely describes the features of a dataset.

### Key Concepts
- **Population vs Sample**: 
  - **Population**: The complete set of items or individuals that we are interested in studying.
  - **Sample**: A subset of the population used to gather insights.
  
- **Parameters vs Statistics**:
  - **Parameter**: A characteristic or measure of a population (e.g., population mean).
  - **Statistic**: A characteristic or measure obtained by using the data from a sample (e.g., sample mean).

### Goals of Inferential Statistics
1. **Generalization**: Making predictions or generalizations about a population based on sample data.
2. **Hypothesis Testing**: Determining the validity of assumptions about a population.
3. **Estimation**: Estimating population parameters (e.g., using confidence intervals).
4. **Predictive Modeling**: Creating models to predict future outcomes based on past data.

---

## Population vs Sample

### Population
- **Definition**: The entire group of individuals or items that share a characteristic of interest.
- **Example**: All adults in a country.

### Sample
- **Definition**: A subset of the population selected for analysis.
- **Why Use a Sample?**: 
  - Cost-effective and time-efficient.
  - Often, studying the entire population is impractical or impossible.

---

## Parameters vs Statistics

### Parameters
- **Definition**: A characteristic or measure of a population.
- **Example**: Population mean (µ).
- **Key Point**: Parameters are typically unknown and need to be estimated.

### Statistics
- **Definition**: A characteristic or measure obtained from a sample.
- **Example**: Sample mean (x̄).
- **Key Points**:
  - Statistics are known values calculated from sample data.
  - The distinction is important for making accurate inferences about the population.

---

## Bias vs Variability

### Bias
- **Definition**: A systematic error that leads to an incorrect estimate of a population parameter.
- **Types of Bias**: Selection bias, measurement bias, response bias.
- **Impact of Bias**: Can lead to invalid conclusions.

### Variability
- **Definition**: The degree to which data points in a dataset differ from each other.
- **Sources of Variability**: 
  - Sampling error
  - Natural variability among subjects
- **Impact of Variability**: Higher variability can obscure patterns and lead to less reliable estimates.
- **Relationship Between Bias and Variability**: 
  - Bias is about accuracy, while variability is about precision.
  
### Goal in Statistics
- Minimize bias and control variability to achieve reliable estimates.

---

## Sampling

### Definition
Sampling is the process of selecting a subset of individuals from a population to estimate characteristics of the whole population.

### Types of Sampling
1. **Random Sampling**:
   - **Simple Random Sampling**: Each member has an equal chance of selection.
     - **With Replacement**: Selected individuals can be chosen more than once.
     - **Without Replacement**: Selected individuals cannot be chosen again.
2. **Stratified Sampling**: Population is divided into strata, and samples are drawn from each stratum.
3. **Cluster Sampling**: The population is divided into clusters, and entire clusters are randomly selected.
4. **Systematic Sampling**: Selecting every nth member from a list of the population.

---

## Sampling Distribution

### What is Sampling Distribution?
The distribution of a statistic (e.g., sample mean) obtained from repeated sampling from the same population.

### Central Limit Theorem (CLT)
- States that the sampling distribution of the sample mean approaches a normal distribution as the sample size increases, regardless of the population's distribution.
  
### Importance of CLT
- It allows for the use of normal probability methods in inferential statistics, even with non-normal data distributions when sample sizes are sufficiently large.

---

## Importance of Sample Size

### Why is Sample Size Important?
- **Small Samples**: Higher variability, potential bias, and limited statistical power.
- **Large Samples**: Reduced variability, better representation of the population, increased statistical power.

---

## Standard Error

### Definition
Standard error measures the accuracy with which a sample represents a population.

### Formula
\[ SE = \frac{s}{\sqrt{n}} \]
Where:
- \( s \) = sample standard deviation
- \( n \) = sample size

### Roles of Standard Error
1. **Estimation of Population Parameters**: Helps in estimating population means.
2. **Construction of Confidence Intervals**: Defines the range around a sample estimate.
3. **Hypothesis Testing**: Determines the distribution of the test statistic.

---

## Point Estimation

### Definition
Point estimation refers to the use of sample data to calculate a single value (point estimate) that serves as the best guess for an unknown population parameter.

### Examples of Point Estimates
- **Sample Mean**: \( \bar{x} \)
- **Sample Proportion**: \( \hat{p} \)

---

## Good Point Estimate Properties

1. **Unbiasedness**
   - **Definition**: An estimator is unbiased if its expected value equals the true parameter.
   - **Example**: Sample mean is an unbiased estimator of the population mean.
   - **Importance**: Ensures accuracy in estimation.

2. **Consistency**
   - **Definition**: An estimator is consistent if it converges in probability to the true parameter as the sample size increases.
   - **Example**: Sample mean becomes closer to population mean with larger samples.
   - **Importance**: Ensures reliability with larger samples.

3. **Efficiency**
   - **Definition**: An estimator is efficient if it has the smallest variance among all unbiased estimators.
   - **Example**: The sample mean is more efficient than the median for normally distributed data.
   - **Importance**: Provides more precise estimates.

4. **Sufficiency**
   - **Definition**: A statistic is sufficient if it captures all necessary information from the sample.
   - **Mathematical Expression**: The likelihood function for the sample given the parameter.
   - **Importance**: Reduces data without losing information.

---

## Correlation Coefficient

### Definition
A measure of the strength and direction of the linear relationship between two variables.

### Range
The correlation coefficient (r) ranges from -1 to 1:
- **1**: Perfect positive correlation
- **0**: No correlation
- **-1**: Perfect negative correlation

### Assumptions
- Linear relationship
- Homoscedasticity (constant variance)
- Normality of variables (for significance tests)

### Example
If r = 0.85, it indicates a strong positive correlation between the variables.

### Spearman's Rank Correlation
- **Definition**: A non-parametric measure of correlation based on ranked values.
- **Range**: Same as Pearson's, from -1 to 1.
- **Use Case**: Ideal for ordinal data or non-linear relationships.

### Correlation Matrix
A table showing correlation coefficients between multiple variables.

### Interpreting Correlation Values
- **Strong correlation**: \( |r| > 0.7 \)
- **Moderate correlation**: \( 0.3 < |r| \leq 0.7 \)
- **Weak correlation**: \( |r| \leq 0.3 \)

---

## Confidence Intervals

### What is a Confidence Interval?
A range of values used to estimate a population parameter, providing an interval estimate that reflects uncertainty.

### Components of Confidence Interval
1. **Point Estimate**: The statistic from the sample (e.g., sample mean).
2. **Margin of Error**: The range within which the true population parameter is expected to lie.
3. **Confidence Level**: The probability that the interval contains the population parameter (e.g., 95%).

### Common Confidence Levels
- 90%, 95%, and 99%.

### Trade-off
Higher confidence levels result in wider intervals, which may reduce precision.

### Formula for Population Mean
- **For Large Sample Sizes**: 
  \[
  CI = \bar{x} \pm z \times \frac{s}{\sqrt{n}}
  \]
- **For Small Sample Sizes**: 
  \[
  CI = \bar{x} \pm t \times \frac{s}{\sqrt{n}}
  \]

### Example
Calculating a 95% confidence interval for the population mean based on sample data.

### Confidence Interval Formula for Population Proportion
\[
CI = \hat{p} \pm z \times \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}
\]

---

## Margin of Error

### Definition
The margin of error is the amount added to and subtracted from the point estimate in a confidence interval.

### Components of Margin of Error
1. **Critical Value**: The z-score or t-score corresponding to the desired confidence level.
2. **Standard Error**: Measure of the variability of the estimate.

### Formula
\[
ME = z \times SE \quad \text{(for large samples)}
\]
or
\[
ME = t \times SE \quad \text{(for small samples)}
\]

---

## Z-Scores

### Definition
A Z-score indicates how many standard deviations an element is from the mean.

### Usage
Used when the population standard deviation is known or the sample size is large.

### Critical Values for Confidence Levels
- 90%: \( z = 1.645 \)
- 95%: \( z = 1.96 \)
- 99%: \( z = 2.576 \)

## T-Scores

### When to Use
Used when the population standard deviation is unknown, and the sample size is small. The critical value varies based on degrees of freedom.

---

## Hypothesis Testing

### Definition
A statistical method used to decide whether there is enough evidence to reject a null hypothesis.

### Null Hypothesis (H0)
The statement being tested, usually positing no effect or no difference.

### Alternative Hypothesis (H1 or Ha)
The statement that contradicts the null hypothesis, indicating an effect or difference.

---

## Level of Significance

### Definition
The probability of rejecting the null hypothesis when it is true.

### Mathematical Representation
Commonly denoted as \( \alpha \) (e.g., 0.05).

### Interpretation
A lower significance level means stronger evidence is required to reject the null hypothesis.

### Type I Error
The error of rejecting a true null hypothesis.
- **Example**: Concluding that a drug is effective when it is not.

---

## Power of the Test

### Definition
The probability of correctly rejecting the null hypothesis when it is false.

### Mathematical Representation
\[ \text{Power} = 1 - \beta \]
Where \( \beta \) is the probability of making a Type II error.

### Type II Error
Failing to reject a false null hypothesis.
- **Example**: Concluding that a drug is not effective when it is.

---

## Types of Errors

### Type I Error
- **Definition**: Rejecting a true null hypothesis.
- **Consequence**: False positive.

### Type II Error
- **Definition**: Failing to reject a false null hypothesis.
- **Consequence**: False negative.

---

## Critical Value and Rejection Region

### Critical Value
The threshold that determines the rejection region for the null hypothesis.

### Mathematical Calculation
Depends on the significance level and the distribution used (z or t).

### Rejection Region
The area in the tails of the distribution where we would reject the null hypothesis.

---

## Test Statistics

### Definition
A standardized value used to determine whether to reject the null hypothesis.

### Types of Tests
1. **Z-Test**: Used when population variance is known.
2. **T-Test**:
   - **Single Sample T-Test**: Compares the sample mean to a known population mean.
   - **Two-Sample T-Test**: Compares the means of two independent samples.
   - **Paired T-Test**: Compares means from the same group at different times.
3. **Chi-Squared Test**: Tests relationships between categorical variables.
4. **ANOVA**: Compares means across three or more groups.

### General Formula for Z-Test and T-Test
- **Z-Test**: 
\[
Z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}
\]
- **T-Test**: 
\[
T = \frac{\bar{x} - \mu}{\frac{s}{\sqrt{n}}}
\]

---

## P-Value and Its Interpretation

### Definition
The p-value is the probability of observing the test results under the null hypothesis.

### Mathematical Expression
\[ P \leq \alpha \]

### Decision Rule
- If \( p \leq \alpha \): Reject the null hypothesis.
- If \( p > \alpha \): Do not reject the null hypothesis.

### Example
Calculating the p-value from test statistics to determine significance.

---

## Steps in Hypothesis Testing
1. Define the hypotheses (null and alternative).
2. Select significance level (e.g., 0.05).
3. Choose appropriate test and calculate test statistics.
4. Make a decision based on p-value and critical value.

---

## Parametric Tests

### Definition
Statistical tests that assume the underlying population distribution follows a certain parameter (usually normal).

### Assumptions of Parametric Tests
1. Normality of data
2. Homogeneity of variance
3. Data must be interval or ratio scale

### Examples of Parametric Tests
- **Z-Test**
- **T-Test**:
  - One sample t-test
  - Independent two-sample t-test
  - Paired t-test

---

## Non-Parametric Tests

### Definition
Statistical tests that do not assume a specific population distribution.

### When to Use Non-Parametric Tests
- When data does not meet parametric assumptions (e.g., non-normal distributions).

### Examples of Non-Parametric Tests
- **Mann-Whitney U Test**: Compares differences between two independent groups.
- **Wilcoxon Signed-Rank Test**: Compares two related groups.

---

## Comparison of Parametric and Non-Parametric Tests

| Feature               | Parametric Tests                         | Non-Parametric Tests                   |
|-----------------------|------------------------------------------|----------------------------------------|
| **Assumptions**       | Assume normality and equal variances     | No specific distribution assumptions    |
| **Data Type**         | Interval or ratio                        | Ordinal, nominal, or continuous        |
| **Sample Size**       | Typically requires larger samples        | Can work with smaller samples          |
| **Power**             | Generally more powerful when assumptions are met | Less powerful but more flexible |
| **Examples**          | Z-Test, T-Test, ANOVA                   | Mann-Whitney U, Wilcoxon, Kruskal-Wallis |

---

## Simple Linear Regression

### Definition
A statistical method for modeling the relationship between a dependent variable and one independent variable.

### Equation
\[ Y = \beta_0 + \beta_1 X + \epsilon \]
Where:
- \( Y \) = dependent variable
- \( \beta_0 \) = intercept
- \( \beta_1 \) = slope
- \( X \) = independent variable
- \( \epsilon \) = error term

### Purpose
To predict the value of the dependent variable based on the independent variable.

### Assumptions
1. Linearity
2. Independence
3. Homoscedasticity
4. Normality of residuals

### Example
Using linear regression to predict sales based on advertising spend.

---

## Multiple Linear Regression

### Definition
A statistical technique that models the relationship between a dependent variable and two or more independent variables.

### Equation
\[ Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \ldots + \beta_k X_k + \epsilon \]

### Purpose
To understand the effect of multiple independent variables on a dependent variable.

### Assumptions
Similar to simple linear regression but assumes that the residuals should be normally distributed.

### Example
Modeling house prices based on size, location, and number of bedrooms.

---

## Ordinary Least Squares (OLS)

### Objective
To estimate the parameters of a linear regression model by minimizing the sum of the squared residuals.

### What are Residuals?
The difference between the observed value and the predicted value of the dependent variable.

### Why Minimize Squared Residuals?
Minimizing squared residuals helps in achieving the best fit for the regression line, reducing errors in predictions.

### Purpose of OLS
To find the line that best represents the relationship between independent and dependent variables.

### Formula for Estimating \( \beta_1 \) in Simple Linear Regression
\[ \beta_1 = \frac{Cov(X, Y)}{Var(X)} \]

### Steps to Calculate \( \beta_1 \)
1. Calculate covariance between \( X \) and \( Y \).
2. Calculate variance of \( X \).
3. Apply the formula.

### Interpretation of \( \beta_1 \)
Indicates the change in the dependent variable for a one-unit change in the independent variable.

---

## R-squared and Its Interpretation

### Definition
R-squared is the proportion of the variance in the dependent variable that is predictable from the independent variable(s).

### Formula
\[
R^2 = 1 - \frac{SS_{res}}{SS_{tot}}
\]
Where:
- \( SS_{res} \) = sum of squares of residuals
- \( SS_{tot} \) = total sum of squares

### Interpretation
- \( R^2 = 0.8 \): 80% of the variance in the dependent variable can be explained by the independent variable(s).

### Limitations of R-squared
- Does not indicate whether the regression model is adequate.
- Can be artificially inflated by adding more variables.

---

## Adjusted R-squared

### What is Adjusted R-squared?
A modified version of R-squared that adjusts for the number of predictors in the model.

### Why Use Adjusted R-squared?
It accounts for the possibility of overfitting when adding additional independent variables.

### Interpretation
A higher adjusted R-squared indicates a better fit, considering the number of predictors used.

### Example
Comparing models with different numbers of predictors using adjusted R-squared to determine the best fit.

---

## Hypothesis Testing for Regression Coefficients

### Objective
To test whether a regression coefficient is significantly different from zero.

### Null Hypothesis
\( H_0: \beta_i = 0 \) (the independent variable has no effect).

### Alternative Hypothesis
\( H_1: \beta_i \neq 0 \) (the independent variable has an effect).

### Steps for Testing
1. Calculate the test statistic (t-value).
2. Compare with critical value from t-distribution.
3. Make a decision based on the comparison.

### Decision
- If the calculated t-value exceeds the critical value, reject the null hypothesis.

### Example
Testing the significance of a predictor in a multiple regression model.

---

## Confidence Intervals for Regression Parameters

### What are Confidence Intervals?
A range of values within which the true parameter is expected to lie with a certain level of confidence.

### Interpreting Confidence Intervals
If the confidence interval for a regression coefficient does not include zero, it suggests that the predictor is statistically significant.

### Example
Calculating a confidence interval for a regression coefficient and interpreting its meaning.

---

## Additional Reading: BLUE (Best Linear Unbiased Estimator)

### Overview
BLUE refers to the properties of estimators that are linear, unbiased, and have the minimum variance among all unbiased estimators.

---

This comprehensive guide should help you understand the key concepts in inferential statistics.
