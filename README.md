# (Analysis of the Loan Data from Prosper)
## by (Stacey Samoe)


## Dataset

> The following steps were taken during the analysis
     - Data Wrangling 
        1. Gathering Data 
        2. Assessing Data 
        3. Cleaning Data
     - Exploratory Data Analysis
        1. Univariate Analysis
        2. Bivariate Analysis 
        3. Multivariate Analysis
     - Conclusion 

**1. Summary of Assessed Data**
> Loan data from prosper is the dataset that is being used for this analysis. 
> It contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

> For detailed information on the various variables please find link to data dictionary: 
https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0


**2. Data Assessment Findings**

> The dataset has a total of 113937 rows and 81 columns 
> Out of the 81 columns, some have missing values to the tune of more than 50% of the data. All columns with missing data will be cleaned on a case by case basis. 

**Note: considering that fact this is a financial dataset, imputing missing data will be avoided. The aim is to ensure that insights give an accurate picture of the dataset characteristics.** 

**3. Data Cleaning**
  
   >  Credit Grade Column - Will be dropped as it has more than 50% missing data. 
   
   > Close date - Will also be drop as it has more than 50% missing data.
   
   > Missing values in the Estimated Effective Yield, Estimated Loss, Estimated Return, Prosper Rating (numeric & alpha), and ProsperScore among other columns who’s missing values is not less than or equal to 50%. 
   
   > Group Key column, will be dropped.
   
   > Column Total Prosper Loans all the way to ScorexChangeAtTimrOfListing column will be drooped, more than 50% missing data. 
   
   > Column LoanFirstDefaultedCycleNumber will be dropped. 


## Summary of Findings

> Some of the findings as a result of exploratory data analysis include; 

> **Univariate Analysis**

> The most popular product offered by the financial institution is 36 months loans. 

> When it comes to loan status the majority of the clients are either current or in completed loan status. Few clients were in charge-off, defaulted, past due (1-15), and past due (31-60). There were no clients in past due status more than 60 days. 

> The distribution of estimated loss is slightly right skewed. 

> Open revolving accounts distribution is also right skewed and leptokurtic in nature. 

> The nature of majority clients in the portfolio when it comes to employment status, are either employed or full time. 
 
>**Bivariate Analysis**

>36 term loans have a higher median lender yield compared to the other terms. 

>Income range 1-24,999 has the highest median lender yield followed by 25,000-49,999. 

>As the borrow rate increases, the estimated loss also increases. 
 
>**Multivariate Analysis Findings** 

>As the estimated loss increases, the lender yield also increases. With 50,000-74,999 and 25,000-49,999 income range dominating at the top of the estimated loss against lender yield curve. 



## Key Insights for Presentation

> Question: Should the investors INVEST or NOT INVEST in the subject portfolio? 

> The subject financial institution has a total of three products; 12, 36 and 60 term loans. Within the portfolio clients are marketed with different status; current, completed, charge-off, defaulted and past-due. Majority of the clients in the portfolio are either in current or complete status.

> When it comes to the estimated loss, its distribution is slightly right skewed. This indicates estimated losses are of lower figures. 
The above point is complimented by the fact that the majority of the lender yield data points are towards the right. Meaning, the yields are of higher values.  
 
> In an attempt to further understand the performance of the portfolio, the relationship between term and lender yield was investigated. The 36 term loans which are the most popular products have a higher median lender yield compared to the other products. 
 
>We also observed as the estimated loss increased, the lender yield also increased. This is expected as the higher the risk the higher the return.
Going forward and breaking down the relationship between lender yield and estimated loss by product; term 36 loans are seen to cover about three quarters of the curve. They are seen to have a realistic risk appetite. 



