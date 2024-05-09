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

![1 display the data](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/c8488439-8535-45fc-a39f-a869474a711d)

2. Total Loan Applications
   
![2 total LOan APPP](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/54e52ba1-4dc2-4ddd-bda7-1225adae1dcb)

3. Month to Date Loan Applications
![3 mtd la](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/eb25b04a-56c2-4cda-b3e2-7c5a403f3aa2)
![4 pmtd la](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/f0185edb-2b98-4dc8-89d1-a60b5ca04bae)
![5 total amount funded](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/0546b1ae-c7ad-4511-a242-030b85dd1e36)
![6 mtd fa](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/8a5fb3d9-7c10-4a5e-8184-91f1e928f9d1)

![6' pmtd fa](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/f3878d23-83da-4b1b-be4a-cc297c0a92ab)
![7 total amount received](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/288f417e-ecac-49f1-b3e8-a719f43730ae)
![8 mtd ar](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/5517045f-0380-474a-ac2a-db78a8403184)
![9 pmtd ar](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/950d8dd6-e7bd-4b6e-9fa4-ffe13b728b7a)
![10 avg IR](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/9c1baeec-8a93-4cc4-b758-43af2cdcd778)
![11 mtd avg ir](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/e542d133-4f17-4ca7-8266-a7201928e6dc)
![12 pmtd avg ir](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/b440e3b5-9ee3-4ff8-bd93-cd73c48c4228)
![13 avg dti](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/25c53067-5695-46f5-8ca6-191de6cd8708)
![14 mtd avg dti](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/c42a81c3-9b1d-41c5-8252-9bcc19c36674)
![15 pmtd avg dti](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/005e3b17-b741-4b97-a01b-057c262b04c9)
![16 good loan percentage](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/ea15e61a-61e0-465c-a256-7c0d2b511203)
![17 total good laon](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/edc8e64a-20ae-49a9-a394-4fe00a3a9f99)
![18 good loan fa](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/b64399f3-21d0-4430-bcad-212a67f4db8e)
![19 good loan ra](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/6bdf1c99-4087-40e4-a205-e181f839f5a0)
![20 bad loan percentage](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/0e2cc1ce-9a8e-4bc7-8367-26817327cbf7)
![21 total bad loan appl](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/c42490bf-73ee-4599-a056-fa8bbc50bcdd)
![22 bad lon fa](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/b7712a20-323e-4853-aca7-36462f018211)
![23 bad loan ar](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/035e6941-8f2e-4dd3-92e4-39014ad99645)
![24 summary loan status](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/f64c54a3-5a74-4782-a6d8-a3052377b2e9)
![25 summary loan status mtd fa and ra](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/82bc54ff-fde6-4448-bec6-ae4f33ad97cd)
![26 monthly trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/d58dbe5b-de13-425b-af87-64188390f7bf)
![27 state trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/340055f4-d889-4e5d-9ab4-1b492ca84e42)
![27' state trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/d9615fdb-7ed4-464a-84df-a958e925544e)
![28 term trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/c4d4307f-955a-4f25-be67-555a35729185)
![29 emp_term trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/c34cb311-9c0e-4fc4-81e8-490daf306400)
![30 purpose trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/9b43e5ff-0f06-4dd5-8c2b-5c922b34d702)
![31 ownership trend](https://github.com/RobesGael/Bank-Loan-Analysis/assets/155399653/bd2d006f-fc92-40c2-a337-df56948bf1c0)




EDA: 
 In POWER BI, I imported the data from SQL Server
I used Power BI for visualization and analysis. I built an interactive Dashboard that contains many different charts. 

Dashboard Validation: 
I used SQL queries to validate the dashboard.

After two weeks, I delivered the interactive dashboard (You can find it within the Finding and insights files under the name of Bank Loan Analysis Interactive Dashboard) to my manager. Two days later, my manager called me to his office, and he appreciated the job I did; and he assigned me a second task related to the project. It was for analyzing the relationship between loan status and deb-to-Income. He asked me to perform a hypothesis test to do that (You can find the work within Jupiter notebook files).
