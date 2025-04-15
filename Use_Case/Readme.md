# Nicko's Tech Shop
![image](https://github.com/NicolasLopera/Media/blob/2d4664c4e034757f50c0d6a2bec9678e23d44a5d/Use_Case/Credit_Card_banner.jpg)

## Use Case Description
Nicko's Tech Shop is a local shop selling electronics with 4 branches open in the town. As part of the Marketing strategy to drive more customers to the store, Nicko's Tech Shop made a partnership with MLG Bank to sponsor a Credit Card.
The associates from each branch will offer the Credit Card to their customers while they are assisting them with service, when a customer accepts to apply the assistant will open an MLG Bank form on their working tablets and guide the customer through the process, The shop has defined a target of applications by month, and if the goal is reached the associate will be eligible of a 10% bonus over the salary. 

To track the applications submitted by the associates, The data and BI department got the requirement from Marketing to create a report to follow up on: 
  * Total customer applications and total approved applications compared with Plan numbers.
  * Weakly trend of applications. 
  * Store with more applications monthly.
  * The associates that are eligible to get the bonus each month. 

Due to budget restrictions and resource limitations on the data engineering team, data integration between MLG Bank and Nicko's Tech Shop is not possible. Therefore, Nicko's Tech Shop has requested that MLG Bank email a daily CSV file to a generic account used for the Analytical department. 

## Solution Design
The Senior Data Analyst assigned to give a solution has come up with the following plan: 


The Files emailed by the MLG Bank daily will be downloaded to a OneDrive folder by an automated process using Power Automate as soon as the email arrives. Then, another flow will append the data to a table in a SQL Server. 

### Data Flow in Power Automate
1. Email Flow
   

3. Data Ingestion Flow

### Power BI
