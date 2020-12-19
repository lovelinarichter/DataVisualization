# Data Visualization
Project: Communicate Data Findings

## Description
This project has two parts. 
1. Use Python visualization libraries to systematically explore a selected dataset, starting from plots of single variables and building up to plots of multiple variables.
2. Produce a short presentation that illustrates interesting properties, trends, and relationships that you discovered in your selected dataset. 

## Installation
Install Anaconda libraries of Python. The code should run with no issues using Python versions 3.*.

## File Descriptions
The files included in this repo are:
1. exploration_project.ipynb - code in Jupyter notebook
2. exploration_project.html - HTML copy of code
3. exploration_project-slide.slides - converted Jupyter Notebook into slides format.
4. output-toggle.tpl - This template file can be used with nbconvert to export slide deck. <br>
<b>Usage from the command line:</b> jupyter nbconvert Example_Project_Diamonds_Part2.ipynb --to slides --post serve --template output_toggle

## Project Details
The data is provided by Udacity. The data set contains 113,937 loan records with 81 variables on each loan. 
Variables included in the data set are Loan amount, Borrower rate (or interest rate), Current loan status, Borrower Income, Employment Status, Occupation, and many others.
The data dictionary is provided with defintion of each variable. The project requirement is to explore 10 to 15 variables only. 

Data Dictionary: Variables to be used in analysis

1. ListingKey:	Unique key for each listing, same value as the 'key' used in the listing object in the API.
2. LoanStatus: The current status of the loan: Cancelled,  Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, PastDue. The PastDue status will be accompanied by a delinquency bucket.
3. BorrowerAPR:	The Borrower's Annual Percentage Rate (APR) for the loan.
4. EstimatedReturn:	The estimated return assigned to the listing at the time it was created. Estimated return is the difference between the Estimated Effective Yield and the Estimated Loss Rate. Applicable for loans originated after July 2009.
5. ProsperRating (numeric): 	The  Prosper Rating assigned at the time the listing was created: 0 - N/A, 1 - HR, 2 - E, 3 - D, 4 - C, 5 - B, 6 - A, 7 - AA.  Applicable for loans originated after July 2009.
6. ListingCategory: 	The category of the listing that the borrower selected when posting their listing: 0 - Not Available, 1 - Debt Consolidation, 2 - Home Improvement, 3 - Business, 4 - Personal Loan, 5 - Student Use, 6 - Auto, 7- Other, 8 - Baby&Adoption, 9 - Boat, 10 - Cosmetic Procedure, 11 - Engagement Ring, 12 - Green Loans, 13 - Household Expenses, 14 - Large Purchases, 15 - Medical/Dental, 16 - Motorcycle, 17 - RV, 18 - Taxes, 19 - Vacation, 20 - Wedding Loans
7. BorrowerState:	The two letter abbreviation of the state of the address of the borrower at the time the Listing was created.
8. Occupation:	The Occupation selected by the Borrower at the time they created the listing.
9. EmploymentStatus:	The employment status of the borrower at the time they posted the listing.
10. IsBorrowerHomeowner:	A Borrower will be classified as a homowner if they have a mortgage on their credit profile or provide documentation confirming they are a homeowner.
11. CreditScoreRangeUpper:	The upper value representing the range of the borrower's credit score as provided by a consumer credit rating agency. 
12. CurrentCreditLine:s	Number of current credit lines at the time the credit profile was pulled.
13. IncomeRange:	The income range of the borrower at the time the listing was created.
14. IncomeVerifiable:	The borrower indicated they have the required documentation to support their income.
15. LoanOriginalAmount:	The origination amount of the loan.

There are 113,937 loan records from Prospect. There are 81 variables in the dataset. Variables included Loan Status, Borrower's APR, Borrower's Interest Rate for the specific loan. Prosper's rating at the time of listing was created. 

<b> Questions to investigate or main interest in the dataset: </b> I am most interested in figuring out What factors affect the loan status?  Does Borrower's profile is sole determining factor of the loan status? How many investors are interested in the loan? 

Variables that could help in analysis of data:
1. Prospect's data
2. Borrowers's data
3. Investor's data

## Summary 
Overall, I think the result of data analysis is expected. The profile of the borrower such as employment status, income range, credit score, credit lines are strong indicators if the loan is going to result to good performance or note. Although the distribution of data is expected, it also showed interesting result like even those employed and full-time have loan status of default and past-due loans.

For this project, I initially did a data assessment and data cleanup. I removed records with duplicate listing keys, to make sure that the borrower's information and loan information are unique. I did a univariate analysis, wherein i plotted each variable that I am interested to analyse. I also did a bivariate analysis to see correlation between two variables, loan status against each categorical variables. Finally, in mulitvariate analysis. I explored one categorical variable, Loan Status and four numerical variables such as Loan Amount, Prosper Rating, Credit Line and Credit Score.

## Project Limitations
Although the data provided consist of 81 variables, the project only requires 10 to 15 variables to analyze. There are other variables that can be considered to produec a more meaningful and useful result.

## Licensing
Must give credit to Udacity for the data.
