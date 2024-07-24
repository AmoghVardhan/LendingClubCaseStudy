# Lending Club Case Study

## Problem Statement
The data given in the loan dataset contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

## Process

### Data Cleaning
The data needs to be cleaned before deriving analysis. There can be various issues in the dataset. The data cleaning steps we followed were:
1. Clean all null columns.
2. Clean columns with high NaN values.
3. Remove columns having only 1 unique values.
4. Remove rows having null values
5. Handling of data types - fixing data types, string manipulation for getting the data into right format.


### Data Understanding
Go through data dictionary to remove columns that do not contribute to loan default analysis.

### Outlier Treatment
Remove outliers which can distort the data during visualtisation. IQR method is used to remove outliers.

### Univariate Analysis
Univariate analysis refers to the statistical examination of a single variable to summarize its main characteristics and understand its distribution. The goal is to describe and analyze the variable independently, without considering its relationship with other variables.

1. Created a bar graph to understand the distribution by loan status across the following variables:

    a. Home ownership\
b. Loan amount\
c. Interest rate\
d. Purpose of loan\
e. Annual income\
f. Address

2. Created histogram charts to see the distribution of the loan status across different metrics.

### Bivariate Analysis
Bivariate analysis refers to the statistical analysis of two variables to understand the relationship between them. The goal is to explore how one variable affects or is related to another. This type of analysis can reveal patterns, correlations, or associations and is often used to understand dependencies and causal relationships.

1. Created different box plots of various metrics to compare data of fully paid and charged-off loans.
2. Created different scatter plot charts to see the distribution of loan amount and interest rate across different applicants.


## After cleaning and analysis, we came across the following observations/findings:


1. Loan Amount: Higher loan amounts increase the probability of applicants not paying their debt on time and getting charged off.
2. Interest Rate: Applicants with higher interest rates on loan amounts are more prone to be in debt and get charged off.
3. Home Ownership: Applicants who stay in rented accommodation have a higher chance of default.
4. Purpose: Loans taken for/by small businesses are the riskiest since they have the highest default rate.
5. Annual Income: Applicants with higher annual incomes are more likely to pay their loans on time.
6. Address State: A very high percentage of defaults are happening for applicants from state NE. More stringent reviews need to be done for such applicants.
7. Verification Status: Applicants who are not verified before receiving a loan are likely to default.
8. Grade: B grade applicants are more likely to default.


