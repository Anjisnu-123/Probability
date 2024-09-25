<!--noulTopic: 

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
|Binomial | A/B testing,quality contol | success rate of a marketing campaign with 100 lead and 30% conversion rate|
|Geometric | modeling time untill success,customer retention | No of website visit untill user make a purchase|
|Negative binomial | overdispersion in count , sales and demand forecasting | Number of customer visits need to achieve 5 succesful purchase|
|poisson | Event rate modeling,traffic flow analysis | number of calls recieved per hour at a call center|
|Hypergeometric dist | quality control,survey analysis | number of defective itemes found in a sample of 20 from a batch|
|multinomial | document classification,multi class classifictaion | distributon of words accross topics in a text classification|
|Discrete uniform | Random sampling,algo design | Randomly selectig card from a weel shuffled deck|
|zipf's | Text analysis,city population modeling | frequency of words in a large corpus| -->



# Probability Distributions and Applications in Data Science

This repository contains information about various probability distributions, convergence concepts, and their applications in data science. It serves as a comprehensive guide for students, data scientists, and researchers working with statistical concepts and their practical implementations.

## Table of Contents

1. [Convergence Concepts](#convergence-concepts)
   - [Law of Large Numbers](#law-of-large-numbers)
   - [Central Limit Theorem](#central-limit-theorem)
2. [Discrete Distributions](#discrete-distributions)
   - [Bernoulli Distribution](#bernoulli-distribution)
   - [Binomial Distribution](#binomial-distribution)
   - [Geometric Distribution](#geometric-distribution)
   - [Negative Binomial Distribution](#negative-binomial-distribution)
   - [Poisson Distribution](#poisson-distribution)
   - [Hypergeometric Distribution](#hypergeometric-distribution)
   - [Multinomial Distribution](#multinomial-distribution)
   - [Discrete Uniform Distribution](#discrete-uniform-distribution)
   - [Zipf's Distribution](#zipfs-distribution)
3. [Applications in Data Science](#applications-in-data-science)
4. [Statistical Inference](#statistical-inference)
   - [Hypothesis Testing](#hypothesis-testing)
   - [Confidence Intervals](#confidence-intervals)
5. [Fitting Data to Distributions](#fitting-data-to-distributions)
   - [Parameter Estimation](#parameter-estimation)
   - [Goodness of Fit Tests](#goodness-of-fit-tests)
6. [Additional Resources](#additional-resources)

## Convergence Concepts

### Law of Large Numbers

The Law of Large Numbers (LLN) is a fundamental concept in probability theory that describes the behavior of sample means as the sample size increases.

#### Weak Law of Large Numbers (WLLN)

The WLLN states that the sample mean converges in probability to the population mean as the sample size increases.

#### Strong Law of Large Numbers (SLLN)

The SLLN states that the sample mean converges almost surely to the population mean.

### Central Limit Theorem

The Central Limit Theorem (CLT) states that the distribution of the sample mean approaches a normal distribution as the sample size increases, regardless of the underlying distribution of the population.

## Discrete Distributions

### Bernoulli Distribution

- **Definition**: Models a single binary outcome (success/failure)
- **PMF**: P(X = 1) = p, P(X = 0) = 1 - p
- **CDF**: F(x) = 0 if x < 0, 1 - p if 0 ≤ x < 1, 1 if x ≥ 1
- **Mean**: p
- **Variance**: p(1-p)
- **Application**: Binary classification, medical testing

### Binomial Distribution

- **Definition**: Models the number of successes in n independent Bernoulli trials
- **PMF**: P(X = k) = C(n,k) * p^k * (1-p)^(n-k)
- **Mean**: np
- **Variance**: np(1-p)
- **Application**: A/B testing, quality control


## Discrete Distributions

### Bernoulli Distribution

- **Definition**: Models a single binary outcome (success/failure)
- **PMF**: P(X = 1) = p, P(X = 0) = 1 - p
- **CDF**: F(x) = 0 if x < 0, 1 - p if 0 ≤ x < 1, 1 if x ≥ 1
- **Mean**: p
- **Variance**: p(1-p)
- **Skewness**: (1 - 2p) / √(p(1-p))
- **Kurtosis**: (1 - 6p(1-p)) / (p(1-p))
- **Special Characteristics**: Simplest discrete distribution; only two possible outcomes
- **Example**: Modeling whether a coin flip results in heads (success) or tails (failure)
- **Application**: Binary classification, medical testing (e.g., positive/negative test results)

### Binomial Distribution

- **Definition**: Models the number of successes in n independent Bernoulli trials
- **PMF**: P(X = k) = C(n,k) * p^k * (1-p)^(n-k), where C(n,k) is the binomial coefficient
- **CDF**: F(x) = Σ(k=0 to ⌊x⌋) C(n,k) * p^k * (1-p)^(n-k)
- **Mean**: np
- **Variance**: np(1-p)
- **Skewness**: (1 - 2p) / √(np(1-p))
- **Kurtosis**: 3 + (1 - 6p(1-p)) / (np(1-p))
- **Special Characteristics**: Sum of n independent Bernoulli trials
- **Example**: Number of heads in 10 coin flips
- **Application**: A/B testing, quality control (e.g., number of defective items in a batch)

### Geometric Distribution

- **Definition**: Models the number of failures before the first success in a sequence of independent Bernoulli trials
- **PMF**: P(X = k) = (1-p)^k * p, for k = 0, 1, 2, ...
- **CDF**: F(x) = 1 - (1-p)^(⌊x⌋+1)
- **Mean**: (1-p) / p
- **Variance**: (1-p) / p^2
- **Skewness**: (2-p) / √(1-p)
- **Kurtosis**: 6 + (p^2 / (1-p))
- **Special Characteristics**: Memoryless property
- **Example**: Number of coin flips until the first heads
- **Application**: Modeling time until success, customer retention (e.g., number of website visits until a purchase)

### Negative Binomial Distribution

- **Definition**: Models the number of failures before the r-th success in a sequence of independent Bernoulli trials
- **PMF**: P(X = k) = C(k+r-1, k) * p^r * (1-p)^k, for k = 0, 1, 2, ...
- **CDF**: No simple closed form; can be expressed using incomplete beta function
- **Mean**: r(1-p) / p
- **Variance**: r(1-p) / p^2
- **Skewness**: (2-p) / √(r(1-p))
- **Kurtosis**: 6/r + (p^2 / (r(1-p)))
- **Special Characteristics**: Generalizes the geometric distribution (r=1 case)
- **Example**: Number of failures before achieving 5 successes in a series of trials
- **Application**: Overdispersion in count data, sales and demand forecasting

### Poisson Distribution

- **Definition**: Models the number of events occurring in a fixed interval of time or space
- **PMF**: P(X = k) = (λ^k * e^(-λ)) / k!, for k = 0, 1, 2, ...
- **CDF**: F(x) = e^(-λ) * Σ(k=0 to ⌊x⌋) (λ^k / k!)
- **Mean**: λ
- **Variance**: λ
- **Skewness**: 1 / √λ
- **Kurtosis**: 1 / λ
- **Special Characteristics**: Mean equals variance; limit of binomial distribution as n→∞ and p→0
- **Example**: Number of emails received in an hour
- **Application**: Event rate modeling, traffic flow analysis, queueing theory

### Hypergeometric Distribution

- **Definition**: Models the number of successes in a sample drawn without replacement from a finite population
- **PMF**: P(X = k) = (C(K,k) * C(N-K,n-k)) / C(N,n), where N is population size, K is number of successes in population, n is sample size
- **CDF**: F(x) = Σ(k=0 to ⌊x⌋) (C(K,k) * C(N-K,n-k)) / C(N,n)
- **Mean**: n * (K/N)
- **Variance**: n * (K/N) * ((N-K)/N) * ((N-n)/(N-1))
- **Skewness**: Complex expression; depends on N, K, and n
- **Kurtosis**: Complex expression; depends on N, K, and n
- **Special Characteristics**: Models sampling without replacement; approaches binomial as N→∞
- **Example**: Number of red balls drawn from an urn containing red and blue balls
- **Application**: Quality control, survey analysis (e.g., number of defective items in a sample from a batch)

### Multinomial Distribution

- **Definition**: Generalization of the binomial distribution to k possible outcomes
- **PMF**: P(X₁=x₁, ..., Xk=xk) = (n! / (x₁!...xk!)) * p₁^x₁ * ... * pk^xk
- **Mean**: E[Xi] = n * pi
- **Variance**: Var(Xi) = n * pi * (1-pi)
- **Covariance**: Cov(Xi, Xj) = -n * pi * pj (for i ≠ j)
- **Special Characteristics**: Generalizes binomial to multiple categories
- **Example**: Distribution of colored marbles drawn from a bag
- **Application**: Document classification, multi-class classification (e.g., distribution of words across topics in text classification)

### Discrete Uniform Distribution

- **Definition**: Models a finite set of equally likely outcomes
- **PMF**: P(X = k) = 1 / (b - a + 1), for k = a, a+1, ..., b
- **CDF**: F(x) = (⌊x⌋ - a + 1) / (b - a + 1)
- **Mean**: (a + b) / 2
- **Variance**: ((b - a + 1)^2 - 1) / 12
- **Skewness**: 0
- **Kurtosis**: -6/5 * ((b-a+1)^2 + 1) / ((b-a+1)^2 - 1)
- **Special Characteristics**: All outcomes equally likely; maximum entropy discrete distribution
- **Example**: Rolling a fair die (a=1, b=6)
- **Application**: Random sampling, algorithm design (e.g., randomly selecting a card from a well-shuffled deck)

### Zipf's Distribution

- **Definition**: Models frequency of occurrence as a function of rank in a set
- **PMF**: P(X = k) = (1/k^s) / (ζ(s)), where ζ is the Riemann zeta function
- **CDF**: F(x) = (H_{⌊x⌋,s}) / (ζ(s)), where H_{n,s} is the n-th generalized harmonic number
- **Mean**: ζ(s-1) / ζ(s) for s > 2
- **Variance**: ζ(s-2)/ζ(s) - (ζ(s-1)/ζ(s))^2 for s > 3
- **Special Characteristics**: Power law distribution; often observed in natural and social phenomena
- **Example**: Frequency of words in a large corpus
- **Application**: Text analysis, city population modeling, internet traffic analysis

## Applications in Data Science

| Distribution | Best Fit For | Example Use Case |
|--------------|--------------|------------------|
| Bernoulli | Binary classification | Modeling whether an email is spam or not |
| Binomial | A/B testing | Success rate of a marketing campaign with 100 leads and 30% conversion rate |
| Geometric | Modeling time until success | Number of website visits until a user makes a purchase |
| Negative Binomial | Overdispersion in count data | Number of customer visits needed to achieve 5 successful purchases |
| Poisson | Event rate modeling | Number of calls received per hour at a call center |
| Hypergeometric | Quality control | Number of defective items found in a sample of 20 from a batch |
| Multinomial | Multi-class classification | Distribution of words across topics in text classification |
| Discrete Uniform | Random sampling | Randomly selecting a card from a well-shuffled deck |
| Zipf's | Text analysis | Frequency of words in a large corpus |




## Statistical Inference

### Hypothesis Testing

Hypothesis testing is a statistical method used to make decisions about population parameters based on sample data. It involves formulating null and alternative hypotheses, calculating test statistics, and making decisions based on p-values or critical values.

### Confidence Intervals

Confidence intervals provide a range of values that likely contain the true population parameter with a certain level of confidence. They are useful for estimating population parameters and quantifying the uncertainty in point estimates.

## Fitting Data to Distributions

### Parameter Estimation

Parameter estimation involves determining the best-fit parameters for a given probability distribution based on observed data. Common methods include:

- Maximum Likelihood Estimation (MLE)
- Method of Moments
- Bayesian estimation

### Goodness of Fit Tests

Goodness of fit tests assess how well a theoretical distribution fits the observed data. Common tests include:

- Chi-square test
- Kolmogorov-Smirnov test
- Anderson-Darling test

## Additional Resources

- [ANOVA (Analysis of Variance)](https://en.wikipedia.org/wiki/Analysis_of_variance)
- [Riemann zeta function](https://en.wikipedia.org/wiki/Riemann_zeta_function) (related to Zipf's distribution)

For more information on these topics, please refer to standard probability and statistics textbooks or online resources from reputable universities and organizations.
 plt.ylabel('Sample Mean')
 plt.show()
