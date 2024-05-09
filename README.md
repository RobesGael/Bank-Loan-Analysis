# Bank-Loan-Analysis
## Overview
#### In this scenario, I'm a new data analyst hired within a bank. After a month of training, my lead data analyst took his vacation, and my manager assigned me my first project. The goal of this project is to build an interactive dashboard for loan applications. He provided me with the dataset of the loan applications of 2021 with all information I needed.
##### Dashboard1: Summary Key Performance indicators (KPIs) Requirements:
1.	Total Loan Applications: It’s the total number of loan applications received during a specified period. And it’s important to monitor the Month-to-Date (MTD) loan applications and track changes Month-over-Month (MOM).
2.	Total Funded Amount: Understanding the total amount of funds disbursed as loans is crucial. It’s also important to keep an eye on the MTD total funded amount and analyze the MOM changes.
3.	Total Amount Received: Tracking the total amount received from borrowers is essential for assessing the bank’s cash flow and loan repayment. We should analyze the MTD total amount received and observe the MOM changes.
4.	Average interest Rate: Calculating the average interest rate across all loans, MTD, and monitoring the MOM variation in interest rates will provide insights into our lending portfolio’s overall cost.
5.	Average Debt-to-Income Ratio (DTI): Evaluating the average DTI of our borrowers helps us to gauge their financial health. So, we need to compute the average DTI for all loans, MTM and track MOM fluctuations.


   
##### Good loan V Bad loan KPI’s
##### Good Loan KPIs:
1.	Good Loan Application Percentage: We need to calculate the percentage of loan application classified as ‘Good Loan’. This category includes loans with a loan status of “Fully paid’ and ‘Current’.
2.	Good Loan Applications: It’s the total number of all loan applications falling under the ‘Good Loan’ category, which consists of loans with a loan status of ‘Fully paid’ and ‘Current’.
3.	Good loan Funded Amount: Determining the total amount of funds disbursed as ‘Good Loan’. This includes the principal amounts of loans with a loan status of ‘Fully paid’ and ‘Current’.
4.	Good Loan Received Amount: Tracking the total amount received from borrowers for “Good Loan’, which encompasses all payments made on loans with a loan status of ‘Fully paid’ and ‘Current’.



 
##### Bad Loan KPIs:
1.	Bad Loan Application Percentage: Calculating the percentage of loan application categorized as ‘bad Loan’. This category includes loans with a loan status of “Charged off’.
2.	Bad Loan Applications: identifying the total number of all loan applications categorized as ‘Bad Loan’, which consists of loans with a loan status of ‘Charged off’.
3.	Bad loan Funded Amount: Determining the total amount of funds disbursed as ‘Bad Loan’. This comprises the principal amounts of loans with a loan status of ‘Charged off’.
4.	Good Loan Received Amount: Tracking the total amount received from borrowers for “Bad Loan’, which includes all payments made on loans with a loan status of ‘Charged off’.
Loan Status Grid View:
In order to gain a comprehensive understanding of our lending operations and monitor the performance of loans, we aim to create a grid view report categorized by “Loan Status”. By providing insights into metrics such as ‘Total Loan Applications’, ‘Total Funded Amount’, ‘Total received Amount’, ‘Mont-to-Date (MTD) Funded Amount’, ‘MTD Amount Received’, ‘Average Interest rate’ and ‘Average Debt-to-Income Ratio (DTI)’, this grid view will empower us to make data-driven decisions and assets the health of our loan portfolio.

##### Dashboard 2: Overview
In our Bank Loan report project, we aim to visually represent critical loan-related metrics and trends using a variety of chart types. These charts will provide a clear insightful view of our lending operations, facilitating data-driven decision -making and enabling us to gain valuable insights into various loan parameters. Below are the specific chart requirements:
1.	Monthly Trends by issue date (Line chart): To identify seasonality and long-term trends in lending activities.
2.	Regional Analysis by State ( Map): To identify regions with significant lending activity and assess regional disparities.
3.	Loan term Analysis (Dunot Chart): To allow the client to understand the distribution of loans across various term lengths.
4.	Employee Length analysis (Bar Chart): How lending metrics are distributed among borrowers with different employment lengths, helping us assess the impact of employment history on loan applications.
5.	Loan purpose breakdown (Bar Chart): It will provide a visual breakdown of loan metrics based on the stated purposes of loans, aiding in the understanding of the primary reasons borrowers seek financing.
6.	Home ownership Analysis (tree Map): For a hierarchical view of how home ownership impacts loan applications and disbursements.
Metrics to be shown: ‘Total amount of Loan Application’, ‘Total Funded Amount’ and ‘Total Amount Received’.


##### Dashboard 3: Details Grid
Need for comprehensive ‘Details Dashboard’ that provides a consolidated view of all the essential information within our loan data. This Details dashboard aims to offer a holistic snapshot of key loan-related metrics and data points, enabling users to assess critical information efficiently.
## Getting Started
•	Prerequisites: SQL SERVER MANAGEMENT STUDIO (SSMS), POWER BI, Python, Jupiter Notebook, Hypothesis Testing, Linear regression and Machine learning model, MS Office Word / Excel, PowerPoint.
## Usage
- Understand the business and the problem.
- Collect and gather the data. 
-	Data source: Bank Loan Project - Google Drive
-	Data format: The dataset financial_loan) is a CSV file and has 38 576 rows and 24 columns.
  
##### Features used in data:
- Loan ID: It’s a unique identifier assigned to each loan application or loan account.
- Address State: Address state indicates the borrower’s location. It helps assessing regional risk factors, compliance with state regulations, and estimating default probabilities. Banks use this information to identify regional trends in loan demand, adjust marketing strategies, and manage risk portfolios based on geographic regions.
- Employee Length: Employee length provides insights into the borrower’s employment stability and longer employment durations may indicate greater job security. Banks consider employment length when assessing a borrower’s ability to repay. Stable employment often translates to a lower default risk.
- Employee Title: Employee title specifies the borrower’s occupation or job title. It helps lenders understand the source of the borrower’s income. Banks use this field to verify income sources, assess the borrower’s financial capacity, and tailor loan offers to different professions.
- Grade: Grade represents a risk classification assigned to the loan based on creditworthiness. Higher grades signify lower risk. Banks use the grade to price loans and manage risk. Higher-grade loans typically receive lower interest and are attractive to investors.
- Sub Grade: Sub Grade refines the risk assessment within a grade, providing additional differentiation. It offers a finer level of risk assessment, helping banks tailor interest rates and lending terms to match borrower risk profiles.
- Home Ownership: it indicates the borrower’s housing status. It offers insights into financial stability. Banks use this field to assess collateral availability and borrower stability. Homeowners may have lower default rates.
- Issue Date: Issue date marks the loan’s origination date. It’s important for loan tracking and maturity calculations. Banks use issue date to track loan aging, calculate interest accruals, and manage loan portfolio.
- Last credit Pull Date: its records when the borrower’s credit report was last accessed. It helps monitor creditworthiness. Banks use this date to track credit history, assess credit risk, and make lending decisions.
- Last payment Date: Its marks the most recent loan payment received. It tracks the borrower’s payment history. Banks use this date to assess the payment behavior, calculate delinquency, and project future payments.
- Loan Status: It indicates the current state of loan (i.e. ‘fully paid’, ‘current’, ‘default’). It tracks loan performance. Banks use this field to monitor loan health, categorize loans for risk analysis and determine provisioning requirements.
- Next Payment Date: Next payment date estimates the date of the next loan payment. It assists in cash flow forecasting. Banks use this date for liquidity planning and to project revenue from loan portfolios.
- Purpose: Purpose specifies the reason for the loan. It helps understand borrower intentions. Banks use this field to segment and customize loan offering, aligning loan term with borrower needs.
- Term: Term defines the duration of the loan in months. It sets repayment period. Banks use this field to structure loan agreements, calculate interest payment, and manage loan maturities.
- Verification Status: It indicates whether the borrower’s financial information has been verified. It assesses data accuracy. Banks use this field to gauge data reliability, verify income, and evaluate loan application credibility.
- Annual Income: Annual income reflects the borrower’s total yearly earnings. It assesses repayment capacity. Bank uses this income figure to determine loan eligibility, calculate debt-to-income ratios, and evaluate creditworthiness.
- DTI (Debt-to-Income): DTI measures the borrower’s debt burden relative to income. It gauges the borrower’s capacity to take on additional debt. Banks use DTI to assess a borrower’s ability to handle loan payments and make responsible lending decisions.
- Installment: It is the fixed monthly payment amount for loan repayment, including principal and interest. Banks use this field to structure loan terms, calculate amortization schedules, and assess payment affordability.
- Interest rate: The interest rate represents the annual cost of borrowing as a percentage. It determines the loan’s cost. Banks use interest rates to price loans, manage profit margins and attract investors.
- Loan Amount: Loan amount is the total borrowed sum. It defines the principal amount. Banks use loan amounts to determine loan size.
- Total Payment: It tracks the total amount borrowers have already paid. It includes the principal amount and interest.
- Next Payment Date:
- Member ID:
- Total acc:


Data type: No idea. (It’s important to know if the data along the first-party data, the second-party data, or the third-party data. That could be helpful when dealing with missing values) 


Data cleaning and preprocessing
*	The data has 1433 missing values especially in the Emp_title column. We used =COUNTBLANK(RANGE) using excel to check that. We believe that this could be normal because it’s not easy sometimes to categorize or understand the customer’s job. Thus, we are going to leave this column that way.
*	No duplicates records found.


Everything looks good. It’s time to import the data within the SQL Server Management Studio and perform the following queries. These queries will be used to validate our interactive dashboard.

1. Display the data

![1 display the data](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/70411e25-2581-41de-a8c0-db143fd78a56)



EDA: 
 In POWER BI, I imported the data from SQL Server
I used Power BI for visualization and analysis. I built an interactive Dashboard that contains many different charts. 

Dashboard Validation: 
I used SQL queries to validate the dashboard.

After two weeks, I delivered the interactive dashboard (You can find it within the Finding and insights files under the name of Bank Loan Analysis Interactive Dashboard) to my manager. Two days later, my manager called me to his office, and he appreciated the job I did; and he assigned me a second task related to the project. It was for analyzing the relationship between loan status and deb-to-Income. He asked me to perform a hypothesis test to do that (You can find the work within Jupiter notebook files).
