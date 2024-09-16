Day 6 INTRODUCTION TO probability---------------------------------------------** To study** :- Hidden markov mode,markov model
topics:----->>>---------sample space: example of sample space,what is event,what is sample space and why used?-------------------Event: definition and importance,whats likelihood,---------subset representation of event: Notation and representation,why subset rep is important-----------------------------------------
Basic terminology and their definitions:-> outcome,trial,favourable outcome,understanding          ----------------------------------------------------- probability as a measure,relative freq interpretation of probab,mutually exclusive events,union and intersection of events,complement of an event
probability axioms:-> non negativity,normalization/total probability,additivity,axiom 1:non negativity,---------------------------, axiom 2:Total probability of sample space, axiom 3: Additivity,additional consequence derived from axioms,importance of axioms and examples
properties of probability:-> complement rule,union of events , conditional probability,probability--------------------------------- of impossible event,probability of entire sample space=1
Importance and role in AI ML of probability ---------------------------------------------------------

conditional probability:-> Defination,mathematical formula,why important,How to caculate condn prob
independence of events:-> defination,mathematical rep,example,implications of indep,application in prob
understanding dependent and independent events in data scienece:-----------------------------------------------------------------------------------------
Introduction to joint and marginal probabilities: what it is,why do we need it-------------------------------------------------------------
Total probability theorem:->desc,formula,why total probability theorem impo,example qsn---------------------------------
Bayes theorem:-> formula,components of bayes theorem,prior prob(p(a)),likelihood(p(b|a)),marginal likelihood(p(b)),posterior prob(p(a|b)),application of bayes theorem,application in sentiment analysis.docmuet catagorization,bayesian a/b testing

Combinatorics->what it is ,why is it important,impact in data science
what is permutation:
role of permutation in prob
what is combination:-formula,numeric example..





# Introduction to Probability

This README provides a comprehensive overview of probability, including fundamental concepts, theorems, and their applications in AI and ML. It covers sample spaces, events, probability axioms, conditional probability, independence, joint and marginal probabilities, the Total Probability Theorem, Bayes' Theorem, and combinatorics.

## Table of Contents

1. [Sample Space and Events](#sample-space-and-events)
2. [Basic Terminology](#basic-terminology)
3. [Probability Axioms](#probability-axioms)
4. [Properties of Probability](#properties-of-probability)
5. [Conditional Probability](#conditional-probability)
6. [Independence of Events](#independence-of-events)
7. [Joint and Marginal Probabilities](#joint-and-marginal-probabilities)
8. [Total Probability Theorem](#total-probability-theorem)
9. [Bayes' Theorem](#bayes-theorem)
10. [Combinatorics](#combinatorics)
11. [Permutation and Combination](#permutation-and-combination)
12. [Importance in AI and ML](#importance-in-ai-and-ml)

## Sample Space and Events

### Sample Space

The sample space \( S \) of an experiment is the set of all possible outcomes. For example, when flipping a coin, the sample space is:

\[ S = \{ \text{Heads}, \text{Tails} \} \]

### Event

An event is a subset of the sample space. For instance, getting a "Heads" when flipping a coin is an event.

#### Importance

Events are used to determine the probability of certain outcomes occurring.

### Subset Representation of Events

Events are represented as subsets of the sample space. For example, if the sample space \( S \) is \(\{1, 2, 3, 4, 5, 6\}\) (rolling a die), an event \( E \) could be \(\{2, 4, 6\}\) (rolling an even number).

#### Notation and Representation

The event \( E \) can be denoted as \( E \subseteq S \).

#### Importance

Subset representation helps in calculating probabilities and understanding relationships between different events.

## Basic Terminology

### Definitions

- **Outcome**: A single result of an experiment.
- **Trial**: A single execution of an experiment.
- **Favorable Outcome**: An outcome that satisfies the condition of the event.

### Understanding Probability

Probability is a measure of how likely an event is to occur. It is given by:

\[ P(E) = \frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}} \]

## Probability Axioms

### Axiom 1: Non-Negativity

The probability of an event is always non-negative:

\[ P(E) \geq 0 \]

### Axiom 2: Total Probability of Sample Space

The probability of the sample space is 1:

\[ P(S) = 1 \]

### Axiom 3: Additivity

For mutually exclusive events \( E_1 \) and \( E_2 \):

\[ P(E_1 \cup E_2) = P(E_1) + P(E_2) \]

#### Additional Consequence

If events are not mutually exclusive:

\[ P(E_1 \cup E_2) = P(E_1) + P(E_2) - P(E_1 \cap E_2) \]

#### Importance and Examples

Axioms form the foundation of probability theory, ensuring consistency in probability calculations.

## Properties of Probability

### Complement Rule

The probability of the complement of an event \( E \) is:

\[ P(E') = 1 - P(E) \]

### Union of Events

For events \( E_1 \) and \( E_2 \):

\[ P(E_1 \cup E_2) = P(E_1) + P(E_2) - P(E_1 \cap E_2) \]

### Conditional Probability

The probability of \( E_1 \) given \( E_2 \):

\[ P(E_1 \mid E_2) = \frac{P(E_1 \cap E_2)}{P(E_2)} \]

### Probability of Impossible Event

The probability of an impossible event is 0:

\[ P(\text{Impossible Event}) = 0 \]

### Probability of Entire Sample Space

The probability of the entire sample space is 1:

\[ P(S) = 1 \]

## Conditional Probability

### Definition

Conditional probability measures the probability of an event given that another event
