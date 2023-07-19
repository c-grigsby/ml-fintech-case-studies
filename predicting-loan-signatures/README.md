<div align="center">

  <img src="../images/loan-onboarding.jpeg" width="550" alt="Directing"/>

# Predicting Loan E-Signatures

### Predicting E-Signatures on Loan Applications via Financial History

[![Python](https://img.shields.io/badge/python-black?style=for-the-badge&logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/docs/getting_started/index.html)
[![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/doc/stable/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)](https://matplotlib.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)

</div>

## Project Overview

Lending companies work by analyzing the financial history of their loan applicants and evaluating whether or not the applicant is too high risk to be given a loan. If the applicant is not, the lender will determine the terms of the loan. To acquire these applicants companies can organically receive them through their websites or apps, often with the assistance of advertisement companies. Other times, lending companies partner with peer-to-peer (P2P) lending marketplaces in order to acquire leads to potential applicants. Examples of P2P lenders include Upstart, Prosper, and LendingClub. In this case study, we will asses the 'quality' of the leads our company receives from these marketplaces.

- **Market**: The target audience is loan applicants who reach out through an intermediary marketplace.

- **Product**: A loan.

- **Goal**: Develop a model to predict 'quality' applicants. In this case study, 'quality' applicants are those who reach a key part of the loan application process.

## Business Challenge

- In this case study, we will be working for a fintech company that specializes in loans. It offers low APR loans to applicants based on their financial habits, as most lenders do. This company has partnered with a P2P lending marketplace that provides real-time leads (loan applicants). The conversion rates for these leads are satisfactory.

- The company tasks you with creating a model that predicts whether or not these leads will complete the electronic signature phase of the loan application. The company seeks to leverage this model to identify less 'quality' applicants (those not responding to the onboarding process) and experiment with directing them to different onboarding screens.

- The reason for selecting the e-signing process as the response variable is due to the loan application structure:

  - Phase One: The official application begins with the lead arriving on our website after we opted to acquire it. Here the applicant begins the onboarding process to apply for a loan. The user then begins to provide more financial information upon every screen of the onboarding process. Phase One ends with the applicant providing their e-signature indicating that all of the submitted information is accurate.

  - Phase Two: Any of the following screens, in which the applicant is approved or denied and given the terms of the loan is dependent on the company, not the applicant. Therefore the effectiveness of onboarding is measured up to the moment the applicant stops having control of the application process.

## Data

- Because users arrive through a marketplace, we have access to their financial data before the onboarding process begins. This data includes personal information such as age, income, time employed, debt and other financial metrics. Our company utilizes these financial data points to create risk scores based on a variety of factors.

- In this case study, we are given a set of scores from algorithms built by the finance and engineering teams. Furthermore, the marketplace itself provides us with their own lead quality scores. Here we will leverage both sets of scores, as well as a small list of personal/financial features to predict if the user is likely to respond to the current onboarding process.
