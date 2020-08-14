# Loan_approval
The notebook is about housing data on who applies for a loan and if the loan gets approved or rejected. 

## Executive Summary
This document illustrates an analysis of data concerning mortgage application and predict the acceptance or denial of an application. This analysis encapsulates 500 000 observations of mortgage data from the Federal Financial Institutions Examination Council (FFIEC)

## The Data
The data had 21 features columns (except for row_id) and one label column. The features in the data were both numeric and categorical but the categorical features were encoded in numerical form. Before performing any summary statistics of the data and making any feature engineering, the categorical features were converted from their numeric representations in order to create a distinction between numerical and categorical features. After the encoding, some data cleaning was done and some feature engineering was performed to ensure the data was ready for building a machine learning model. The features were further used to create a binary classifier capable of predicting the success of failure of mortgage loan application with an accuracy of 72%. The xgboost Classifier was used.
After exploring the data by calculating summary and descriptive statistics, and by creating visualizations of the data, several potential relationships between features and label (accepted) were identified.

## Data conclusions
After performing the analysis, the author presents the following conclusions:
From the features given, most significant features identified using the Feature Selection module in Azure Machine Learning Studio were:
• loan_puropose (categorical): This feature indicates whether the purpose of the loan was for home purchase, home improvement, or refinancing;
• applicant_income (numerical): this indicates the annual income of applicant in thousands of dollars
• loan_amount (numerical): this is the size of the requested loan in thousands of dollars
• applicant race (categorical): this describes the race of the applicant, i.e. American Indian or Alaska Native, Asian, Black or African American,
Native Hawaiian or other Pacific Islander, White, Information not provided by applicant in mail, internet, or telephone application, Not applicable, No co-applicant
• Lender (categorical): a feature with no ordering indicating which of the lenders was the authority in approving or denying a one
• property type (categorical): it indicates whether the loan or application was for a one-to-four-family dwelling (other than manufactured housing),
manufactured housing, or multifamily dwelling.
• co_applicant (boolean): indicates whether there is a co-applicant (spouse) or not. This was encoded as true or false.
• tract_to_msa_md_income_pct (numerical): this is a census information that tells the percent of tract median family income compared to the
Metropolitan Statistical Area (MSA)/Metropolitan Division (MD) median family income.
• Minority_population_pct (numerical): this is the percentage of minority population to total population for tract.
• Applicant_ethnicity (categorical): this is part of applicant information and indicates the ethnicity of the applicant; Hispanic or Latino, Not
Hispanic or Latino, Information not provided by applicant in mail, internet, or telephone application, not applicable, no co-applicant.
• Ffiecmedian_family_income (numerical): FFIEC median family income in dollars for the MSA/MD in which the tract is located (adjusted
annually by FFIEC)
• Applicant_sex (categorical): an information about the gender of applicant whether male, female, or no information provided in mail, internet or
telephone application, or not applicable, or no co-applicant.
• Number_of_owner-occupied_units (numerical): this is an information on the number of dwellings, including individual condominiums, that are
lived in by the owner.
• State_code (categorical): this is a property information indicating the U.S. state of applicant
• Loan_type (categorical): a loan information that indicates whether the loan granted, applied for, or purchased was conventional, government-
guaranteed, or government-insured in the following values; Conventional (any loan other than FHA, VA, FSA, or RHS loans), FHA-insured
(Federal Housing Administration), VA-guaranteed (Veterans Administration), FSA/RHS (Farm Service Agency or Rural Housing Service)
• Msa_md (categorical): property location item with no ordering indicating MSA/MD
• Population (numerical): the total number of population in tract
• Number_of_1_to_4_family units (numerical): dwellings that are built to house fewer that 5 families.


## Conclusion
The accuracy of the binary classifier is well presented. An omission of a feature reduces the accuracy of the mode which shows the sensitivity of the data. The analysis shows white folks are far more likely to be successful in application for a mortgage loan and male applicants are more than twice likely to be successful than female applicants. Though there are some ethical concerns, the variables in the data incites management decision into who gets approval or not for a mortgage application.
