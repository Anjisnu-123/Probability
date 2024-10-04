<!--# Topic
ANOVA: It is a hypothesis testing technique used to compare the means of multiple groups and determine if atleast one group mean is significantly different from others.
Why and when used anova? :- usecase,region
Example: 
Assumptions in Annova: Independence of observations,Normally,Homogeneity of variance,Additivity (defination,importance,assessment)
*To read :* Homogenity test 1>levene's test 2> Bartlett's test

Types of ANOVA: Classification of ANOVA : Based on number factors (one way anova,two way anova,N-way anova),Based on the nature of the groups (Repeated measures anova,mix design anova),Based
on the number of dependent variavle (Multivariate anova)

One way anova : Defination,Mathematical rep:Hypothesis,f stat calculation,example
Two way anova : Defination,math rep: fstat
N-Way anova : Fo analysis of 3 or more factors,Math representation,
Repeated measures ANOVA: Defination,mathematical representation
Mixed design anova : Defination,mathematical rep,example

MANOVA : defination,Mathematical rep,example
POST-HOC tests in ANOVA : to dtetrmine which specific group mean is different from each oter when null hypothesis is different,Two commonly use post hoc: Tukey's HSD,Bonferroni correction(Defination,key feature,,how it works,
example).

CHI-square test: used to determine if there is a significant association b/w catag variables,Introduction,more...
chi-square goodness of fit test: Defination, when to use,mathematical formulation,Assumptions: Data should be in form of counts/freq,Each observation should be independent,The expected frew
for each catag should be atleast 5.

chi - square goodness of fit test example mathematical

Chi sq test of independence: Defination,Contingency table,when to use,Mathematical formulation,Assumptions: Data should be in form of counts/freq,Each observation should be independent,The expected frew
for each catag should be atleast 5.

Application of chi sq test in AI-ML : 1.Feature selection , 2.Model evaluation,3.market basket analysis

Bootstraping : stat method that involves repeatedly sampling data with replacement from an observed dataset to create multiple new dataset.Key idea,Process,Example of bootstraping
Why use bootstraping : Key benifits: Dealing with small sample size,estimating std error,robustness
Application in AI ML:  model evaluation,confidence intervals for performance metrics
Bootstrap confidence intervals : Defination,steps to calc bootstrap confidence intervals: Resampling with replacement,compute stat,distribution of stat,Percentaile method.
Types of  bootstrap : percentile bootstrap,basic bootstrap,bias correlated accelerated
Examples of bootstrap
Mathematical defination of bootstrap confidence intervals
*to study: GMM,PELT*
confidence intervals:
Bayesian Inference: (bayesian vs frequentist approach Basic comparison),frequentist approach ,bayesian approach
Bayes theorem and role in bayesian inference,interpretation
How bayesian inference updates the belief?: prior,likelihood,posterior,summary of bayesian inference
Example of bayesian inference: Application in machine learning

Application of bayesian inference in AI ML: Naive bayes classifier,bayesian neural networks,Bayesian optimization:(use,how it works,example)
Practical example of hypothesis testing: testing in medical studies,Marketing A/B testing , onfidence intervals in survey rate,
Aplication: model evalutaion and statistical tetsing : cross validation,significance testing in model comparison(ANOVA)

Applications:A/B testing in model performance: purpose,steps in testing:Define hypothesis,splitting the data,measure performance,Test for
significanc ,interpreting results.

Application : USe of confidence intervals in prediction : purpose,theoritical bg,formula,application in ML,Example
Why inferential stat matter in AI ML : Validate resullts,imporve models,manage uncertainity,Feature selection

Key techniques in inferential stat: Hypothesis testing,confidence interval,regressionanalysis,anova:(purpose,key components,applications)
Bridging the gap between stat and ML: stat foundation for ML,Model evaluation and uncertainity,data drive decisions -->




# Statistical Techniques and Their Applications in AI/ML

This repository contains comprehensive information and examples of various statistical techniques and their applications in Artificial Intelligence and Machine Learning. The content covers fundamental concepts, mathematical representations, and practical applications of these techniques in AI/ML workflows.

## Table of Contents

1. [ANOVA (Analysis of Variance)](#anova-analysis-of-variance)
2. [Chi-Square Test](#chi-square-test)
3. [Bootstrapping](#bootstrapping)
4. [Bayesian Inference](#bayesian-inference)
5. [Hypothesis Testing in AI/ML](#hypothesis-testing-in-aiml)
6. [Confidence Intervals in AI/ML](#confidence-intervals-in-aiml)
7. [Key Techniques in Inferential Statistics](#key-techniques-in-inferential-statistics)

## ANOVA (Analysis of Variance)

ANOVA is a hypothesis testing technique used to compare the means of multiple groups and determine if at least one group mean is significantly different from others.

### Types of ANOVA

1. **One-way ANOVA**: Compares means across one factor.
   - Definition: Analyzes the difference in means between two or more groups of an independent variable.
   - Mathematical representation: 
     - Hypothesis: H₀: μ₁ = μ₂ = ... = μₖ, H₁: At least one μᵢ is different
     - F-statistic calculation: F = (Between-group variability) / (Within-group variability)

2. **Two-way ANOVA**: Examines the influence of two different categorical independent variables on one continuous dependent variable.
   - Definition: Analyzes the impact of two factors on the dependent variable.
   - Mathematical representation: Similar to one-way ANOVA, but includes interaction effects.

3. **N-way ANOVA**: For analysis of 3 or more factors.

4. **Repeated Measures ANOVA**: Used when the same subjects are measured multiple times.
   - Definition: Analyzes data from repeated observations on the same subjects.

5. **Mixed Design ANOVA**: Combines between-subjects and within-subjects factors.

6. **MANOVA (Multivariate Analysis of Variance)**:
   - Definition: Analyzes group differences across multiple dependent variables simultaneously.

### Assumptions in ANOVA

1. Independence of observations
2. Normality of residuals
3. Homogeneity of variance
4. Additivity (no interaction between factors unless specified)

### Post-Hoc Tests in ANOVA

Used to determine which specific group means are different from each other when the null hypothesis is rejected.

1. **Tukey's HSD (Honestly Significant Difference)**:
   - Key feature: Controls for family-wise error rate
   - How it works: Compares all possible pairs of means

2. **Bonferroni Correction**:
   - Key feature: Very conservative approach
   - How it works: Adjusts p-values for multiple comparisons

## Chi-Square Test

The Chi-Square test is used to determine if there is a significant association between categorical variables.

### Types of Chi-Square Tests

1. **Chi-Square Goodness of Fit Test**:
   - Definition: Determines whether observed frequencies differ significantly from expected frequencies.
   - When to use: Testing if a sample comes from a specific distribution.
   - Mathematical formulation: χ² = Σ((O - E)² / E), where O is observed frequency and E is expected frequency.

2. **Chi-Square Test of Independence**:
   - Definition: Tests if there is a significant relationship between two categorical variables.
   - Contingency table: Used to organize data for this test.
   - Mathematical formulation: Similar to goodness of fit test, but applied to a contingency table.

### Assumptions

- Data should be in the form of counts or frequencies
- Each observation should be independent
- The expected frequency for each category should be at least 5

### Applications in AI/ML

1. Feature selection
2. Model evaluation
3. Market basket analysis

## Bootstrapping

Bootstrapping is a statistical method that involves repeatedly sampling data with replacement from an observed dataset to create multiple new datasets.

### Key Benefits

- Dealing with small sample sizes
- Estimating standard errors
- Robustness in parameter estimation

### Process

1. Resample with replacement from original dataset
2. Calculate statistic of interest for each resampled dataset
3. Build distribution of the statistic
4. Use distribution to make inferences

### Applications in AI/ML

- Model evaluation
- Confidence intervals for performance metrics

### Types of Bootstrap

1. Percentile Bootstrap
2. Basic Bootstrap
3. Bias-Corrected Accelerated Bootstrap

### Bootstrap Confidence Intervals

- Definition: Range of values likely to contain the true population parameter.
- Steps to calculate:
  1. Resample with replacement
  2. Compute statistic for each sample
  3. Create distribution of statistic
  4. Use percentile method to determine interval

## Bayesian Inference

Bayesian inference is a statistical approach that updates probabilities as more information becomes available.

### Key Concepts

- Prior: Initial belief about parameter
- Likelihood: Probability of data given parameter
- Posterior: Updated belief after observing data
- Bayes' Theorem: P(A|B) = (P(B|A) * P(A)) / P(B)

### How Bayesian Inference Updates Belief

1. Start with prior distribution
2. Collect data
3. Calculate likelihood
4. Compute posterior using Bayes' theorem
5. Posterior becomes new prior for future updates

### Applications in AI/ML

#### Naive Bayes Classifier

The Naive Bayes Classifier is a probabilistic machine learning model based on Bayes' theorem, with an assumption of independence between features.

##### How it works:
1. Calculate the prior probability for each class.
2. Calculate the likelihood of each feature given each class.
3. Use Bayes' theorem to calculate the posterior probability for each class.
4. Choose the class with the highest posterior probability as the prediction.

##### Advantages:
- Simple and fast
- Works well with high-dimensional data
- Performs well with small training datasets
- Handles both continuous and discrete data

##### Limitations:
- Assumes feature independence (which is often not true in real-world scenarios)
- Sensitive to feature correlation

##### Types of Naive Bayes:
1. Gaussian Naive Bayes: For continuous data, assuming a Gaussian distribution
2. Multinomial Naive Bayes: For discrete data, often used in text classification
3. Bernoulli Naive Bayes: For binary/boolean features

##### Example (Python pseudocode):
```python
class NaiveBayes:
    def fit(self, X, y):
        # Calculate prior probabilities and feature likelihoods
        
    def predict(self, X):
        # Calculate posterior probabilities and return the class with highest probability
```

#### Bayesian Neural Networks

Bayesian Neural Networks (BNNs) are neural networks with a prior distribution on their weights.

##### Key features:
1. Uncertainty Quantification: Provides uncertainty estimates for predictions
2. Regularization: Natural protection against overfitting
3. Robustness: Better performance with limited data

##### How it works:
1. Define a prior distribution over the network weights
2. Use variational inference or MCMC methods to approximate the posterior distribution of weights
3. Make predictions by integrating over the posterior distribution of weights

##### Advantages:
- Provides uncertainty estimates
- Robust to overfitting
- Can work well with small datasets

##### Challenges:
- Computationally expensive
- Requires careful choice of priors
- Interpretation of uncertainty can be complex

##### Example (PyTorch pseudocode):
```python
import torch.nn as nn

class BayesianLayer(nn.Module):
    def __init__(self, in_features, out_features):
        super().__init__()
        self.weight_mu = nn.Parameter(torch.Tensor(out_features, in_features))
        self.weight_sigma = nn.Parameter(torch.Tensor(out_features, in_features))

    def forward(self, input):
        weight = self.weight_mu + torch.randn_like(self.weight_sigma) * self.weight_sigma
        return nn.functional.linear(input, weight)
```

#### Bayesian Optimization

Bayesian Optimization is a sequential design strategy for global optimization of black-box functions.

##### Key components:
1. Surrogate Model: Usually a Gaussian Process
2. Acquisition Function: Guides the search for the optimum

##### How it works:
1. Build a probabilistic model of the objective function
2. Use an acquisition function to determine the next point to evaluate
3. Update the model with the new observation
4. Repeat steps 2-3 until convergence or budget exhaustion

##### Advantages:
- Efficient for expensive-to-evaluate functions
- Works well for non-convex problems
- Handles noisy observations

##### Common acquisition functions:
1. Expected Improvement (EI)
2. Upper Confidence Bound (UCB)
3. Probability of Improvement (PI)

##### Applications in ML:
- Hyperparameter tuning
- Neural Architecture Search
- Automated Machine Learning (AutoML)

##### Example (Python pseudocode using GPyOpt):
```python
import GPyOpt

def objective_function(x):
    # Your black-box function to optimize

bounds = [{'name': 'x', 'type': 'continuous', 'domain': (-5,5)}]

optimizer = GPyOpt.methods.BayesianOptimization(f=objective_function, domain=bounds)
optimizer.run_optimization(max_iter=20)
```

### Comparison of Bayesian Methods in AI/ML

| Method | Key Advantage | Main Challenge | Typical Use Case |
|--------|---------------|-----------------|-------------------|
| Naive Bayes | Simplicity and speed | Assumption of feature independence | Text classification, spam filtering |
| Bayesian Neural Networks | Uncertainty quantification | Computational complexity | Safety-critical applications, small datasets |
| Bayesian Optimization | Efficiency for expensive evaluations | Scalability to high dimensions | Hyperparameter tuning, AutoML |

## Hypothesis Testing in AI/ML

Hypothesis testing is crucial in validating model performance and making data-driven decisions.

### Applications

#### A/B Testing in Model Performance

- Purpose: Compare performance of two models or variations
- Steps:
  1. Define hypothesis (null and alternative)
  2. Split data
  3. Measure performance
  4. Test for significance
  5. Interpret results

#### Significance Testing in Model Comparison

- Purpose: Determine if one model significantly outperforms another
- Common methods: t-test, ANOVA for multiple model comparison

## Confidence Intervals in AI/ML

Confidence intervals provide a range of plausible values for a population parameter.

### Applications

- Model Prediction Uncertainty: Quantify uncertainty in model predictions
- Performance Metric Estimation: Provide range for metrics like accuracy, F1-score

### Use in ML Model Evaluation

- Purpose: Assess reliability and stability of model performance
- Steps:
  1. Calculate point estimate of metric
  2. Estimate standard error (often using bootstrapping)
  3. Construct confidence interval
  4. Interpret results in context of problem

## Key Techniques in Inferential Statistics

1. Hypothesis Testing: Assessing evidence against a null hypothesis
2. Confidence Intervals: Estimating range of plausible values for parameters
3. Regression Analysis: Modeling relationships between variables
4. ANOVA: Comparing means across groups

## Why Inferential Statistics Matter in AI/ML

- Validate results: Ensure findings are not due to chance
- Improve models: Guide model selection and refinement
- Manage uncertainty: Quantify confidence in predictions and estimates
- Feature selection: Identify significant predictors

## Bridging the Gap Between Statistics and ML

- Statistical foundations for ML: Understanding underlying principles
- Model evaluation and uncertainty quantification: Rigorous assessment of model performance
- Data-driven decision making: Applying statistical inference to guide decisions in ML pipelines

## Contributing

Feel free to contribute to this repository by submitting pull requests or opening issues for discussion. We welcome contributions that enhance the content, provide examples, or improve explanations.



---

By providing this comprehensive guide, we aim to bridge the gap between traditional statistical techniques and their modern applications in AI and Machine Learning. Whether you're a student, researcher, or practitioner, we hope this resource helps you navigate the complex landscape of statistical methods in data science.






