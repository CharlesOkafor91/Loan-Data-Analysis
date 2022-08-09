# Data Exploration Of Prosper Loan Data
## by Charles Okafor


## General Description of The Project
In this project, we will be analysing the Loan data from Prosper, in an attempt to identify relationships between features of concern. I plan to analys the data to discover insights which will help us understand the effects and relationships between the variables in the dataset.

## List of Relevant and Required Software.
* Python is the basic language used here - libraries such as Pandas, Numpy, Matplotlib and Seaborn
* Jupyter notebook from anaconder is required to run this project
* Finally a good browser such as Chrome is needed to visualise the presentation

## List of Files Included in The Project.
* Part_I_exploration_template.ipynb
* Part_II_slide_deck_template.ipynb
* Part_I_exploration_template.html
* Part_II_slide_deck_template.slides.html
* README.md
* prosperLoanData.csv

## The Dataset

The data consists of information regarding 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found in the repository [here](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv%26amp;sa%3DD%26amp;ust%3D1581581520570000&sa=D&source=editors&ust=1659457547284019&usg=AOvVaw2eUmmBQPwNU5rtelXPh3T2),
with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
BorrowerAPR and LenderYield and a negative relationship between ProsperRating_numeric and EstimatedLoss whereas there seem be little down-slope relationship between ProsperRating_numeric and BorrowerAPR. The distribution of BorrowerAPR, LenderYield and BorrowerRate seemed to be Gaussian but a slightly right-skewed while that of ProsperScore seem to be flat with high spike at the left. I also found that there seem to be high EstimatedLoss for loans defaulted and past due

Outside of the main variables of interest, I discovered that LoanOriginalAmount were high for CreditGrade AA and majority of the loans were either Completed, Chargedoff or Defaulted. Also for every LoanStatus, ProsperRating_numeric and EstimatedLoss showed a negative down-slop relationship but with very little relationship for Cancelled and Past Due >120 loans.


## Key Insights for Presentation

For the presentation, I focused mainly on factors (variables) affecting BorrowerAPR and LoanStatus. I start by introducing the LoanStatus and CreditGrade variables, then showing the distribution of BorrowerAPR, BorrowerRate, LenderYield and ProsperScore. Then I showed the relationships between variables such as BorrowerAPR and LenderYield, BorrowerAPR and Term, ProsperRating_numeric and BorrowerAPR, ProsperRating_numeric and EstimatedLoss, EstimatedLoss and LoanStatus, LoanOriginationQuarter and BorrowerAPR, BorrowerState and BorrowerAPR, and finally Occupation and BorrowerAPR. Then I finally showed the multivariate relationships between some of these vairiables and how they impact on pr correlate with each other 

I used the violin plots and box plots for my categorical variables to show their relationship with BorrowerAPR. I' focused mainly on the relationships between BorrowerAPR and other variables and also determine how they affect the LoanStatus.

## Bugs

There is no bugs expected to be encou tered from this project. There are a few warnings however about the depreciation of some regex functions and factorplot
