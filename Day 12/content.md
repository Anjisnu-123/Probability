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
*To read: sampling methdods*

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
> Types of measure in dispersion: Range,IQR,variance,std deviation,mean absolute deviation:def,formula,inference,use in data science,use in data science ,example

