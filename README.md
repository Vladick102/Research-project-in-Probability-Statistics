# Socioeconomic Factors and Voting Patterns: Statistical Analysis

## Project Overview
This project analyzes the relationship between various socioeconomic factors and voting patterns across U.S. counties. The authors use statistical methods to determine how factors such as unemployment rates, median income, urban influence, and education levels correlate with political preferences in elections.

## Dataset
The dataset contains county-level information with the following variables:
- State and County names
- FIPS (Federal Information Processing Standard) codes
- Unemployment rate
- Median household income
- Urban Influence Code
- Income percentile
- Percentage of population with Bachelor's degrees
- Winning political party (Democrat or Republican)
- Percentage of votes for the dominant party

## Methodologies

### Exploratory Data Analysis
- Histograms for all numerical variables
- Density plots comparing distributions by winning party
- Key findings:
  - Republicans tend to have slightly lower unemployment rates
  - Democrats show higher median incomes with wider distribution
  - Democrats dominate in urban areas (low Urban Influence Code)
  - Republicans show stronger presence in middle-income percentiles
  - Democrats show higher education levels (Bachelor's degree percentage)

### Statistical Testing
- Chi-squared tests to determine which factors significantly influence election outcomes
- Results showed that Bachelor's degree percentage, unemployment rate, and Urban Influence Code had the strongest impact on election results

### Predictive Modeling
Two classification models were implemented and compared:

1. **Naive Bayes Classifier**
   - Based on Bayes' theorem with strong independence assumptions
   - Predicts party affiliation based on county characteristics
   - Achieved 82.57% accuracy on the test set

2. **Logistic Regression**
   - Models the log-odds of a county voting Democratic vs. Republican
   - Accounts for relationships between predictors
   - Achieved 89.95% accuracy on the test set

## Conclusions
- The logistic regression model outperformed the Naive Bayes classifier
- The superiority of the logistic regression model is attributed to its ability to capture dependencies between predictors
- Naive Bayes performed worse due to its assumption of independence between predictors, which doesn't hold in real-world voting data
- The project demonstrates that socioeconomic factors can effectively predict voting patterns with high accuracy

## Contributors
- Vladyslav Sydorak https://github.com/Vladick102
- Mykhailo Ponomarenko https://github.com/mykhailoponomarenko
- Mykhailo Ivasiuk https://github.com/Fenix125
