# Lending Club Case Study (Consumer Finance Company)
> Consumer Finance Company is specialised in lending different types of loans to urban customers.  
> This case study aims to understand the driving factors behind loan defaults, which can help in risk assessment of the company.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Recommendations](#recommendations)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Information
- **Background:** Lending Club provides personal loans to individuals. The company wants to minimize losses due to loan defaults by identifying key factors that lead to default.
- **Business Problem:** The goal is to analyze historical loan data to identify patterns and variables that are strong predictors of loan default. This will help the company improve its credit risk assessment and lending policies.
- **Dataset:** The dataset (`loan.csv`) contains information about past loan applicants, including loan amount, term, interest rate, employment length, home ownership, annual income, loan status, and more. The data has been cleansed to remove irrelevant columns, standardize formats, and handle missing values.

## Technologies Used
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- Jupyter Notebook

## Conclusions

### Key Findings

- **Loan Grade and Sub-Grade:**  
  Default rates increase sharply for lower grades (especially F and G). Sub-grades G3, G5, and F5 show the highest default rates. Grade is a strong summary indicator of risk, as it incorporates multiple borrower and loan characteristics.

- **Loan Purpose:**  
  Certain purposes are consistently associated with higher default rates, especially:
    - Small business
    - Renewable energy
    - Medical
    - House
    - Educational  
  These purposes are even riskier when combined with large loan amounts or low grades.

- **Loan Amount:**  
  Higher loan amounts are associated with higher default rates across most purposes. The risk is especially pronounced for small business, renewable energy, and medical loans at higher amounts.

- **Interest Rate:**  
  Higher interest rates are correlated with higher default rates, as riskier borrowers are charged higher rates.

- **Annual Income:**  
  Most defaults occur in the 30k–65k income range (due to volume), but lower income alone is not a strong predictor after controlling for other variables.

### High Risk Combinations

| Purpose            | High Risk Grades   | High Risk Loan Amounts     |
|--------------------|-------------------|-----------------------------|
| small business     | D, E, F, G        | Highest bins (largest loans)|
| renewable energy   | F, G              | Highest bins                |
| medical            | F, G              | High bins                   |
| house              | F, G              | High bins                   |
| educational        | F, G              | High bins                   |

## Recommendations

- Lending policies should be more conservative for loans with:
    - Low grades
    - High loan amounts
    - High-risk purposes (especially small business, renewable energy, and medical)
- These combinations have the highest observed default rates and should be prioritized for stricter credit assessment and monitoring.

## Acknowledgements
- Inspired by Lending Club’s open data and peer-to-peer lending research.
- Data dictionary and business context from Lending Club documentation.
- This project was based on [MTech AI/ML Course Lending Case Study](https://learn.upgrad.com/course/9258/segment/62981/383435/1155550/5764475).

## Contact
Created by [@githubusername] - feel free to contact me!