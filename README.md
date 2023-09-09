# CREDIT SCORE_UNIVERSITY PROJECT
This is a Python project that I worked on in university on Bussiness Artificial Intelligent subject
## 1. Target
- Enhance customer experience by reducing application processing time. 
- Improve the predictive capabilities of the credit scoring model using traditional methods to enhance the credit quality of installment loan customers, increase approval rates, and proactively manage bad debt. 

  => The 'Artificial Intelligence Credit Scoring' project provides a competitive advantage, increasing the bank's credibility in the market.
   
## 2. What is credit scoring?
This is a method implemented to assess the risk level of loan applicants based on both qualitative and quantitative factors, serving as the basis for determining credit limits for customers. Risk assessment of borrowers is conducted through statistical methods, data analysis, financial statement analysis, and balance sheet analysis. From this, certain indicators and maximum safe credit limits for a customer are determined, known as "scores," which banks use to evaluate and classify the credit risk of customers. This process involves analyzing past loan data to create an effective scoring model for customers.

## 3.The importance of credit scoring in the banking sector
- Commercial banks always encounter various risks in their operations, such as credit risk, interest rate risk, liquidity risk, and foreign exchange risk. Among these, credit risk is the most significant as credit activities form the core operations of commercial banks, serving as a constant thread throughout their activities. Credit scoring and customer rating are conducted to assist commercial banks in:
- Making credit decisions: determining credit limits, terms, interest rates, collateral, and approval or rejection of credit applications.
- Monitoring and assessing creditworthy customers when credit accounts are outstanding. Customer ratings allow commercial banks to anticipate signs of deteriorating loan quality and take timely measures. From a portfolio management perspective, credit scoring and customer rating systems also serve the purpose of:
- Developing marketing strategies to target less risky customers.
- Estimating the amount of non-recoverable loans to set aside as credit loss provisions.
  
## 4. MODEL IMPLEMENTATION
### 4.1. Construct a comprehensive model
With an ongoing stream of data from individual customers seeking substantial loans, which is continually updated through loan search websites or directly from Vietnamese commercial banks, the implementation of the Customer Credit Scoring process using artificial intelligence will streamline and expedite the customer credit rating process. Specifically, it involves applying classification methods to customer data to group customers. This procedure will consist of the following three stages:

Step 1: Gathering customer information.
Step 2: Utilizing artificial intelligence to perform credit scoring for individual customers.
Step 3: Generating a credit score report.

The process of collecting customer information will be assessed based on three primary criteria: Loan attributes, non-financial details, and customer financial information. This process is depicted in the following diagram.
        
The outcomes of the individual customer Credit Scoring process will be classified and specific determinations will be made for each category as outlined below:
	- Low-risk category: Offering loans with favorable terms.
	- Medium-risk category: Providing loans under standard conditions.
	- High-risk category: Possible exclusion from lending or lending with elevated interest rates or more stringent terms.
 ### 4.2. Model selection
 *Random Forest model:*
	Step 1: Select random samples from the given dataset.
 	Step 2: Establish a decision tree for each sample, receiving predictions from each decision tree.
  	Step 3: Cast votes for each prediction.
   	Step 4: Choose the most frequently predicted result as the final prediction.
    
### 4.3. The factors considered when rating individual credit – the selection of variables.
To apply to the credit rating problem for customers, we need to first establish evaluation criteria based on the following determinants that define the lending limits:
- The customer's capital involvement in projects, business plans, production, services, and lifestyle.
- The maximum loan-to-value ratio compared to the collateral's value, as stipulated in the bank's collateral regulations.
- The customer's debt repayment capacity.
- The capital capacity of each bank and not exceeding the lending limit authorized by the Bank's CEO.
=> Based on these lending determinants of the bank, we can derive specific benchmarks for assessing and determining the lending limits as follows:
#### Non-financial indicators:
+ Age
+ Education level
+ Number of workers in the family
+ Time attached to current job
+ Quantity of financial revenue sources
#### Fianacial indicators:
+ Fixed income per month
+ Value of collateral (house, car, land, etc.)
+ Savings account
+ Existing debt balance
#### Loan features:
+ Interest rate
+ Deadline
+ Loan rate
+ Payment method

### 4.4. Moody's ratign scale
This model places greater emphasis on assessing debt repayment capacity using eight evaluation criteria, while only four evaluation criteria are dedicated to assessing family members' characteristics. The program will validate the data for consistency according to index control principles and flag areas for review when inconsistencies are detected in legal criteria, scoring criteria, total scores, and customer class rankings. The individual rating system ranges from AAA to D, as illustrated in the table below, with rankings determined based on the decreasing total maximum score of 100 points per individual (adjusted by the specified weights).

![image](https://github.com/ThuHuong-Gina/Credit-Score-Prediction_Project/assets/141025228/c9bcb898-677c-4d47-88a2-ea0dacad47c7)


