### Analysis
Understand the past

### Analytics 
Predict the future

## Data Analysis:
- Business case studies
- Qualitative analytics
- Preliminary data report
- Reporting with visuals
## Data Analytics:
- Creating Dashboards
- A/B testing

Explanation:
Data analysis focuses on understanding and interpreting existing data (case studies, qualitative review, reports, visuals).
Data analytics often involves using data and tools to predict, optimize, or test (dashboards for monitoring, A/B testing for experimentation).

## Traditional AI
Mainly applied to structured datasets to improve efficiency and accuracy in repetitive tasks

## Generative AI
Generating new raw data or content, such as text, code, audio, or images by relying on patterns from a given training dataset

## Business intelligence
Includes all technology driven tools involved in the process of analyzing, understanding and reporting available past data

## Machine Learning
Assess potential future scenarios by using advanced statistical methods

Utilize artificial intelligence to predict behavior in unprecendented ways

_____________________________________________
Raw Data
    Cookies
    Surveys

### Data pre processing
- Data
    - Class labeling
      - numerical
      - categorical
    - Data cleansing
    - Missing values
  - Balancing
  - Shuffling
  - ER diagram (Entity Relation)
  - Relational schema (DB tables)
- Big Data
  - Data Masking
  - Complex way in which data is retrived from different sources

### BI techniques
- Turning data in to graphs
- Data is filtered to KPI's.

### Machine Learning
- Creating an algorith, which a computer then uses to find a model that fits the data as beset as possible, and makes very accurate predictions based on that.
- We provide the Machine with algorithms which give the machine directions on how to learn on its own 
- Types of Machine learning
  - Supervised Learning
    - SVMs
    - NNs
    - Deep learning
    - Random Forest
    - Bayesian networkds
  - Unsupervised learning
    - K-means
    - deep learning 
  - Reinforcement learning
  - 

NLP 
Transformers - self attention

#### Data Architect
Designs the way data will be retrieved, processed and consumed
#### Data engineer
Processes the obtained daa so that it is ready for analysis
#### database administrator
Handles control of data,
Mainly workds with traditional data
#### BI analyst
#### BI consultant
#### BI developer

#### Data scientist
#### Data analyst
#### ML Engineer


# Probability
P(A) = preferred outcomes(favorable) / all outcomes (sample space)

  - experimental probabilites
  - Theoretical probabilities

Complements
    all events has complements
    (A')' = A
    P(A) + p(B) + p(C) = 1 (for a event with 3 possibilities)



## Combinatorics
- permutation
  - Pn = n*(n-1)*(n-2).... = n!
  - (n+k)! = n!*(n+1)*(n+2)...*(n+k)
  - (n-k)! = n!/ (n-k+1)*(n-k+2)*.....*(n-k+k)
  -  
- variation
  - Repetition
    - the total number of ways you can pick and arrange some elements in a given set
    - V bar of n and p  = n power p
    - V bar of n and p  = n ^ p
      -  n the total number of elements we have avilable
      -  p the number of positions we need to fill
   - Without Repetition
     - when we can't use the same element twice
     - v of n and p = n! / (n-p)!
     - arranging p elements out of a total number n
- Combinations
  - P of n = n!

### **Summary Table**

---
| Concept      | Formula &nbsp &nbsp &nbsp &nbsp         | Order Matters? |
|--------------|-------------------------------|---------------|
| Permutation  | n!                            | Yes           |
| Variation    | n! / (n-p)! (no rep) <br> n^p (rep) | Yes           |
| Combination  | n! / [p! * (n-p)!]            | No            |
---


We can say that all the different permutations of a single combination are different variations

Choosing those 3 to represent the company is a single combination, since the order in which we pick them is not relevant
Any of the 6 permutaion is a different variation but not a different combination (order)

variation 720 (6*120)
combination 120
permutation 6

What's the number of combination for choosing p-many elements out of a sample space of n elements?
```
C(n, p) = n! / [p! * (n-p)!]
```

## Statatics
```
p(A|B) != p(B|A)
```

Law of total probability
```
p(A) = p(A|B1) * P(B1) + p(A|B2) * P(B2)....
```
If events B₁, B₂, ..., Bₙ form a partition of the sample space (i.e., they are mutually exclusive and exhaustive), then for any event A:
```
p(A) = p(A|B₁)·p(B₁) + p(A|B₂)·p(B₂) + ... + p(A|Bₙ)·p(Bₙ)
```
This law allows you to compute the probability of A by considering all the different ways A can occur via the events 
```
B₁, B₂, ..., Bₙ.p(A) = p(A|B₁)·p(B₁) + p(A|B₂)·p(B₂) + ... + p(A|Bₙ)·p(Bₙ)
```

### Bayes Law
**Bayes Law** (or Bayes’ Theorem) describes how to update the probability of a hypothesis (event A) given new evidence (event B). The formula is:
```
p(A|B) = [p(B|A) · p(A)] / p(B)
```
- **p(A|B):** Probability of A given B (posterior)
- **p(B|A):** Probability of B given A (likelihood)
- **p(A):** Probability of A (prior)
- **p(B):** Probability of B (evidence)