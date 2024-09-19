Topic: 

Convergence Concepts: Law of large number:weak law of large number,strong law of large number,central limit theorem: statement of clt.
Application of distributions: stat inference:Hypothesis testing,confidence values,fitting data to distribution:Parameter estimation,goodness of fit test.Practical example
To read: Anova

Discrete distribution:

Bernouli,binomial,geometric,negative binomial,poisson,hypergeometric, multinomial ,discrete uniform,zipf's dist: for all defination and aplications. for every dist write PMF,CDF,mean
var,skewness,kurtosis,special characteristics(if any),example





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
  Z = \frac{\bar{X}_n - \mu}{\sigma/\sqrt{n}} \xrightarrow{d} N(0, 1
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

### Bernoulli Distribution
- **PMF**: 
  \[
  P(X = k) = p^k(1-p)^{1-k}, \quad k \in \{0, 1\}
  \]
- **Mean**: \( \mu = p \)
- **Variance**: \( \sigma^2 = p(1-p) \)
- **Skewness**: \( \frac{1-2p}{\sqrt{p(1-p)}} \)

### Binomial Distribution
- **PMF**: 
  \[
  P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}, \quad k = 0, 1, \ldots, n
  \]
- **Mean**: \( \mu = np \)
- **Variance**: \( \sigma^2 = np(1-p) \)

### Geometric Distribution
- **PMF**: 
  \[
  P(X = k) = (1-p)^{k-1} p, \quad k = 1, 2, \ldots
  \]
- **Mean**: \( \mu = \frac{1}{p} \)
- **Variance**: \( \sigma^2 = \frac{1-p}{p^2} \)

### Negative Binomial Distribution
- **PMF**: 
  \[
  P(X = k) = \binom{k+r-1}{r-1} p^r (1-p)^k
  \]
- **Mean**: \( \mu = \frac{r}{p} \)
- **Variance**: \( \sigma^2 = \frac{r(1-p)}{p^2} \)

### Poisson Distribution
- **PMF**: 
  \[
  P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!}
  \]
- **Mean**: \( \mu = \lambda \)
- **Variance**: \( \sigma^2 = \lambda \)

### Hypergeometric Distribution
- **PMF**: 
  \[
  P(X = k) = \frac{\binom{K}{k} \binom{N-K}{n-k}}{\binom{N}{n}}
  \]
- **Mean**: \( \mu = \frac{nK}{N} \)
- **Variance**: \( \sigma^2 = \frac{nK(N-K)(N-n)}{N^2(N-1)} \)

### Multinomial Distribution
- **PMF**: 
  \[
  P(X_1 = k_1, X_2 = k_2, \ldots, X_k = k_k) = \frac{n!}{k_1! k_2! \ldots k_k!} p_1^{k_1} p_2^{k_2} \ldots p_k^{k_k}
  \]
- **Mean**: \( \mu_i = np_i \)
- **Variance**: \( \sigma^2_i = np_i(1-p_i) \)

### Discrete Uniform Distribution
- **PMF**: 
  \[
  P(X = k) = \frac{1}{n}, \quad k = 1, 2, \ldots, n
  \]
- **Mean**: \( \mu = \frac{a+b}{2} \)
- **Variance**: \( \sigma^2 = \frac{(b-a+1)^2 - 1}{12} \)

### Zipf's Distribution
- **PMF**: 
  \[
  P(X = k) = \frac{1/k^s}{\sum_{n=1}^{N} 1/n^s}
  \]
- **Mean**: Depends on \(s\)
- **Variance**: Depends on \(s\)

## Practical Examples
Here you can include practical implementations, such as:

- **Simulating the Law of Large Numbers**:
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
