# Credit Card Client Default Analysis

## Overview

This code performs an analysis of a dataset containing information on credit card clients in Taiwan from April 2005 to September 2005. The dataset includes demographic factors, credit data, payment history, and bill statements. The goal is to understand the factors that contribute to default payments.

## Dataset Description

The dataset contains 25 features, including:

- **ID:** Client identification.
- **LIMIT_BAL:** Maximum credit available (NT dollar).
- **SEX:** Gender (1 = male, 2 = female).
- **EDUCATION:** Education level (1 = graduate school, 2 = university, 3 = high school, 4 = other, 5 = unknown).
- **MARRIAGE:** Marital status (1 = married, 2 = single, 3 = other).
- **AGE:** Age in years.
- **PAY_0, PAY_2, PAY_3, PAY_4, PAY_5, PAY_6:** Repayment status in September, August, July, June, May, and April 2005 respectively. (-1 = not due, 1 = 1-month delay, 2 = 2-month delay,... 9 = 9-month delay).
- **BILL_AMT1, BILL_AMT2, BILL_AMT3, BILL_AMT4, BILL_AMT5, BILL_AMT6:** Bill statement amounts (NT dollar) in September, August, July, June, May, and April 2005.
- **PAY_AMT1, PAY_AMT2, PAY_AMT3, PAY_AMT4, PAY_AMT5, PAY_AMT6:** Previous payment amounts (NT dollar) in September, August, July, June, May, and April 2005.
- **default.payment.next.month:** Default payment status in October (1 = yes, 0 = no).

## Code Description

1. **Import Libraries:**
    - numpy for numerical operations.
    - pandas for data manipulation.
    - matplotlib.pyplot for plotting.
    - seaborn for enhanced visualizations.
2. **Load Dataset:**
    - Reads the dataset from a CSV file into a pandas DataFrame.
3. **Data Inspection:**
    - Displays the first few rows of the DataFrame.
    - Prints the number of rows and columns.
    - Checks for missing values.
4. **Education Level Analysis:**
    - Counts the occurrences of each education level.
    - Recodes education levels 0 and 6 to 5 (unknown).
    - Calculates the percentage of each education level.
    - Generates a count plot to visualize the distribution of education levels.
5. **Marital Status Analysis:**
    - Counts the occurrences of each marital status.
    - Recodes marital status 0 to 3 (other).
    - Calculates the percentage of each marital status.
    - Generates a count plot to visualize the distribution of marital statuses.
6. **Age Analysis:**
    - Creates a box plot to visualize the distribution of age.
    - Creates a histogram to visualize the frequency of different age groups.
7. **Credit Limit Analysis:**
    - Creates a box plot to visualize the distribution of credit limits.
    - Creates a histogram to visualize the frequency of different credit limit amounts.
    - Creates another histogram (with 50 bins) of credit limits using matplotlib.pyplot.hist.
