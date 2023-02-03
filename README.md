# (Loan Data from Prosper)
## by (Myra Lugwiri)


## Dataset

This dataset consists of 113,937 loans taken with 81 variables on each loan including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. After looking at the data I discovered a lot of the columns had missing values, hence these columns were dropped to remain with columns that would provide accurate insights.



## Summary of Findings
> During the exploration phase, I discovered that the loanStatus of an individual is affected by EmploymentStatus. As expected we have a high number of individuals with the Current LoanStatus whose EmploymentStatus is Employed. While Full-time EmploymentStatus individuals take the lead in  Completed LoanStatus.

> A large number of individuals who are houseowners are employed and have full-time employmentStatus while individuals who are self-employed, other, part-time, Not employed and retired have a large number of individuals who are not homeowners.

> Also a large number of individuals who are houseowners have a Current LoanStatus as compared to the number of individuals with the other LoanStatuses. Indicating the IsBorrowerHouseowner variable affects the LoanStatus

> As would be expected Chargedoff and Defaulted LoanStatuses have high BorrowerAPR and BorrowerRate. The LoanStatus with the highest BorrowerRate and BorrowerAPR is Past-Due(91-120 Days). I found out that a relationship exists between BorrowerAPR, BorrowerRate and LoanStatus, where LoanStatus is affected by the given variables e.g Defaulted, Past-Due(1-15 Days) and Past-Due(31-60 Days) LoanStatuses are not present for low values of BorrowerAPR and BorrowerRate below 0.05.

> Interestingly the relationship that exists between BorrowerAPR, LoanStatus and IsBorrowerHomeowner is that Individuals who are not house owners have a higher BorrowerAPR for all the loanStatuses. While individuals who are houseowners do not have Cancelled LoanStatus for any value of the BorrowerAPR.

> A linear relationship exists between BorrowerAPR and BorrowerRate, also MonthlyLoanPayment and LoanOriginalAmount  have a linear relationship with a strong positive correlation.

> It was very unexpected to discover that the other numerical variables(TotalCreditLinespast7years, StatedMonthlyIncome, Investors and Term) in the dataset did not have a strong correlation between them. Where the correlation coefficient between Term and StatedMonthlyIncome was low


## Key Insights for Presentation

> For the presentation, I focus on the influence of 2 numerical variables( BorrowerAPR and BorrowerRate) and the 2 categorical variables(IsBorrowerHomeowner and EmploymentStatus). I will start with introducing the LoanStatus distribution followed by the relatinship that exists between the 2 categorical variables with the LoanStatus using a barplot.

> Afterwards I introduce the numerical variables distribution and using a scatterplot to showcase the relationship that exists between the variables then I will introduce how the 2 variables interact with the LoanStatus variable where I will separate the LoanStatus into a set of 3 on scatterplot to show how they interact with the BorrowerAPR and BorrowerRate.
