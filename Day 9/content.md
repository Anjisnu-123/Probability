noulTopic: 

Convergence Concepts: Law of large number:weak law of large number,strong law of large number,central limit theorem: statement of clt.
Application of distributions: stat inference:Hypothesis testing,confidence values,fitting data to distribution:Parameter estimation,goodness of fit test.Practical example
To read: Anova

Discrete distribution:

Bernouli,binomial,geometric,negative binomial,poisson,hypergeometric, multinomial ,discrete uniform,zipf's dist: for all defination and aplications. for every dist write PMF,CDF,mean
var,skewness,kurtosis,special characteristics(if any),example
To watch:-- Raymen zeta function to watch for zipf's denominatore harmonic mean

Application in datascience
Name:     |           Best Fit                     | Where use
|----------|----------------------------------------|-----------
|Bernoulli | Binary classification, medical testing | modeling wheather spam or not |
|Binomial:  A/B testing,quality contol: success rate of a marketing campaign with 100 lead and 30% conversion rate
|Geometric: modeling time untill success,customer retention: No of website visit untill user make a purchase
|Negative binomial: overdispersion in count , sales and demand forecasting: Number of customer visits need to achieve 5 succesful purchase
|poisson: Event rate modeling,traffic flow analysis: number of calls recieved per hour at a call center
|Hypergeometric dist: quality control,survey analysis: number of defective itemes found in a sample of 20 from a batch
|multinomial: document classification,multi class classifictaion: distributon of words accross topics in a text classification
|Discrete uniform: Random sampling,algo design: Randomly selectig card from a weel shuffled deck
|zipf's: Text analysis,city population modeling: frequency of words in a large corpus



# Convergence Concepts and Discrete Distributions

This project explores various concepts in probability and statistics, including the Law of Large Numbers, Central Limit Theorem, and various discrete distributions. It provides implementations for statistical inference methods such as hypothesis testing, confidence intervals, and parameter estimation.

## Table of Contents
- [Convergence Concepts](#convergence-concepts)
  - [Law of Large Numbers](#law-of-large-numbers)
  - [Central Limit Theorem](#central-limit-theorem)
- [Statistical Inference](#statistical-inference)
  - [Hypothesis Testing](#hypothesis-testing)
  - [Confidence Intervals](#confidence-intervals)
  - [Parameter Estimation](#parameter-estimation)
  - [Goodness of Fit Tests](#goodness-of-fit-tests)
- [Discrete Distributions](#discrete-distributions)
  - [Bernoulli Distribution](#bernoulli-distribution)
  - [Binomial Distribution](#binomial-distribution)
  - [Geometric Distribution](#geometric-distribution)
  - [Negative Binomial Distribution](#negative-binomial-distribution)
  - [Poisson Distribution](#poisson-distribution)
  - [Hypergeometric Distribution](#hypergeometric-distribution)
  - [Multinomial Distribution](#multinomial-distribution)
  - [Discrete Uniform Distribution](#discrete-uniform-distribution)
  - [Zipf's Distribution](#zipfs-distribution)
- [Practical Examples](#practical-examples)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Convergence Concepts

### Law of Large Numbers
The Law of Large Numbers states that as the number of trials increases, the sample average will converge to the expected value.

- **Weak Law**: For any \(\epsilon > 0\),
  \[
  P(|\bar{X}_n - \mu| < \epsilon) \to 1 \text{ as } n \to \infty
  \]

- **Strong Law**: Almost surely, the sample average converges to the expected value.

### Central Limit Theorem (CLT)
The Central Limit Theorem states that the distribution of the sample mean approaches a normal distribution as the sample size becomes large, regardless of the shape of the population distribution.

- **Statement**: If \(X_1, X_2, \ldots, X_n\) are i.i.d. random variables with mean \(\mu\) and variance \(\sigma^2\), then:
  \[
  Z = \frac{\bar{X}_n - \mu}{\sigma/\sqrt{n}} \xrightarrow{d} N(0, 1)
  \]

## Statistical Inference

### Hypothesis Testing
Hypothesis testing involves making decisions based on the value of a parameter and testing if the observed data supports a specific hypothesis.

### Confidence Intervals
Confidence intervals provide a range of values that likely contain the population parameter.

### Parameter Estimation
Parameter estimation aims to determine the values of parameters based on sample data.

### Goodness of Fit Tests
Goodness of fit tests assess how well a statistical model fits observed data.

## Discrete Distributions

### 1. Bernoulli Distribution
- **Definition**: A Bernoulli distribution models a single trial with two outcomes: success (1) and failure (0).
- **PMF**: 
  \[
  P(X = k) = p^k(1-p)^{1-k}, \quad k \in \{0, 1\}
  \]
- **CDF**: 
  \[
  F(x) = \begin{cases} 
  0 & \text{if } x < 0 \\
  1 - p & \text{if } 0 \leq x < 1 \\
  1 & \text{if } x \geq 1 
  \end{cases}
  \]
- **Mean**: \( \mu = p \)
- **Variance**: \( \sigma^2 = p(1-p) \)
- **Skewness**: \( \frac{1 - 2p}{\sqrt{p(1 - p)}} \)
- **Kurtosis**: \( 3 - \frac{6p(1-p)}{p(1-p)} \)
- **Special Characteristics**: Only two outcomes; the simplest discrete distribution.
- **Best Fit Model**: Logistic regression for binary outcomes.

### 2. Binomial Distribution
- **Definition**: Models the number of successes in \(n\) independent Bernoulli trials.
- **PMF**: 
  \[
  P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}, \quad k = 0, 1, \ldots, n
  \]
- **CDF**: 
  \[
  F(k) = \sum_{j=0}^{k} P(X = j)
  \]
- **Mean**: \( \mu = np \)
- **Variance**: \( \sigma^2 = np(1-p) \)
- **Skewness**: \( \frac{1 - 2p}{\sqrt{np(1-p)}} \)
- **Kurtosis**: \( \frac{(1 - 6p(1-p))}{np(1-p)} + 3 \)
- **Special Characteristics**: Approaches normal distribution as \(n\) increases.
- **Best Fit Model**: Binomial regression for count data.

### 3. Geometric Distribution
- **Definition**: Models the number of trials until the first success.
- **PMF**: 
  \[
  P(X = k) = (1-p)^{k-1} p, \quad k = 1, 2, \ldots
  \]
- **CDF**: 
  \[
  F(k) = 1 - (1-p)^k
  \]
- **Mean**: \( \mu = \frac{1}{p} \)
- **Variance**: \( \sigma^2 = \frac{1-p}{p^2} \)
- **Skewness**: \( \frac{2 - p}{\sqrt{1-p}} \)
- **Kurtosis**: \( 6 + \frac{p^2}{1-p} \)
- **Special Characteristics**: Memoryless property (the future does not depend on the past).
- **Best Fit Model**: Poisson regression for count data.

### 4. Negative Binomial Distribution
- **Definition**: Models the number of failures before a specified number of successes.
- **PMF**: 
  \[
  P(X = k) = \binom{k+r-1}{r-1} p^r (1-p)^k
  \]
- **CDF**: 
  \[
  F(k) = \sum_{j=0}^{k} P(X = j)
  \]
- **Mean**: \( \mu = \frac{r}{p} \)
- **Variance**: \( \sigma^2 = \frac{r(1-p)}{p^2} \)
- **Skewness**: \( \frac{2 - p}{\sqrt{r(1-p)}} \)
- **Kurtosis**: \( 6 + \frac{p^2}{r(1-p)} \)
- **Special Characteristics**: Can model overdispersed count data.
- **Best Fit Model**: Generalized linear models with a negative binomial link.

### 5. Poisson Distribution
- **Definition**: Models the number of events in a fixed interval of time or space.
- **PMF**: 
  \[
  P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!}
  \]
- **CDF**: 
  \[
  F(k) = \sum_{j=0}^{k} P(X = j)
  \]
- **Mean**: \( \mu = \lambda \)
- **Variance**: \( \sigma^2 = \lambda \)
- **Skewness**: \( \frac{1}{\sqrt{\lambda}} \)
- **Kurtosis**: \( 3 + \frac{1}{\lambda} \)
- **Special Characteristics**: Suitable for rare events.
- **Best Fit Model**: Poisson regression for event count data.

### 6. Hypergeometric Distribution
- **Definition**: Models the number of successes in a sample drawn without replacement from a finite population.
- **PMF**: 
  \[
  P(X = k) = \frac{\binom{K}{k} \binom{N-K}{n-k}}{\binom{N}{n}}
  \]
- **CDF**: 
  \[
  F(k) = \sum_{j=0}^{k} P(X = j)
  \]
- **Mean**: \( \mu = \frac{nK}{N} \)
- **Variance**: \( \sigma^2 = \frac{nK(N-K)(N-n)}{N^2(N-1)} \)
- **Skewness**: \( \frac{(N-n)(K-n)(N-K)}{(K+n)(N-K+n)(N-n)} \)
- **Kurtosis**: Complex formula; typically less relevant.
- **Special Characteristics**: Applicable in quality control and sampling.
- **Best Fit Model**: Hypergeometric tests for proportions.

### 7. Multinomial Distribution
- **Definition**: Generalizes the binomial distribution for scenarios with more than two outcomes.
- **PMF**: 
  \[
  P(X_1 = k_1, X_2 = k_2, \ldots, X_k = k_k) = \frac{n!}{k_1! k_2! \ldots k_k!} p_1^{k_1} p_2^{k_2} \ldots p_k^{k_k}
  \]
- **CDF**: 
  \[
  F(k_1, k_2, \ldots, k_k) = \sum P(X_1 \leq k_1, X_2 \leq k_2, \ldots, X_k \leq k_k)
  \]
- **Mean**: \( \mu_i = np_i \)
- **Variance**: \( \sigma^2_i = np_i(1 - p_i) \)
- **Skewness**: Depends on the probabilities; no simple formula.
- **Kurtosis**: Complex; generally less relevant.
- **Special Characteristics**: Suitable for categorical data.
- **Best Fit Model**: Multinomial logistic regression for categorical outcomes.

### 8. Discrete Uniform Distribution
- **Definition**: All outcomes are equally likely in a finite sample space.
- **PMF**: 
  \[
  P(X = k) = \frac{1}{n}, \quad k = 1, 2, \ldots, n
  \]
- **CDF**: 
  \[
  F(x) = \frac{x-a+1}{b-a+1}, \quad a \leq x < b
  \]
- **Mean**: \( \mu = \frac{a+b}{2} \)
- **Variance**: \( \sigma^2 = \frac{(b-a+1)^2 - 1}{12} \)
- **Skewness**: 0 (symmetric)
- **Kurtosis**: \( \frac{9}{5} \) (light tails)
- **Special Characteristics**: All outcomes equally likely.
- **Best Fit Model**: Use when data is uniformly distributed.

### 9. Zipf's Distribution
- **Definition**: Describes the frequency of words or items in a large dataset.
- **PMF**: 
  \[
  P(X = k) = \frac{1/k^s}{\sum_{n=1}^{N} 1/n^s}
  \]
- **Mean**: Depends on the parameter \(s\).
- **Variance**: Depends on the parameter \(s\).
- **Skewness**: Depends on \(s\); generally high for small \(s\).
- **Kurtosis**: Depends on \(s\).
- **Special Characteristics**: Heavy-tailed distribution; often found in natural languages.
- **Best Fit Model**: Power-law models for heavy-tailed data.

## Practical Examples
Here you can include practical implementations, such as:

### Simulating the Law of Large Numbers
```python
import numpy as np
import matplotlib.pyplot as plt

p = 0.5
n_trials = 1000
sample_means = [np.mean(np.random.binomial(1, p, n)) for n in range(1, n_trials + 1)]

plt.plot(sample_means)
plt.axhline(y=p, color='r', linestyle='--')
plt.title('Law of Large Numbers')
plt.xlabel('Number of Trials')
plt.ylabel('Sample Mean')
plt.show()
