# Diamonds Data Exploration

## Dataset
This notebook explores a dataset containing peer-to-peer loan information of 113,937 loans with 80 variables on each loan from Prosper Funding LLC. The variables are a mix of quantitative variables and categorical variables. Along with the dataset, a feature dictionary describing the variables was also provided [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).

You will find that the file (prosperLoanData.csv) isn't uploaded in the repository since we have added it to the google drive then extracted here in this colab notebook for analysis.


## Summary of Findings

When doing data exploration, I found that generally, there was a strong relationship between Estimated Returns for Prosper against Prosper Ratings. When Prosper Ratings increases, the general trend is that there will be lower returns for Prosper.

Exploring the data through different plotting techniques, I also found a couple additional interesting insights related to term length, credit score & income ranges.

###Term
*   For high-rating borrowers (A or AA), 60-month loans usually have a higher Estimated Return vs. 12-month loans. The longer the loan, the riskier the transaction is for Prosper; more often than not leads to higher returns
*   When it comes to lower credit rating borrowers (E), 36-month loans actually give the highest returns than 60-month ones. 

###Income range
*   Generally, seeing higher Estimated Return with higher income ranges. But once income = $0, Estimated Return is highest.

###Credit score
Estimated return vs. average credit score. The negative relationship is particularly strong when the Employment Status is Employed, Full-time, Part-time, or Retired.


## Key Insights for Presentation
For the presentation, I will primarily be focusing on features/variables that could affect the Estimated Return on loan for prosper.

Starting with distribution of Estimated Return first to visualise the distribution of returns, I plotted it against Prosper Rating (Alpha) after as they had a strong negative correlation with each other.

After that, I examine other features such as loan term length, income range, employment status as well as credit score to see how that might affect estimated return on loan.