# Loan-Prediction

### Business Understanding:

Lending Club is a US peer-to-peer lending company, headquartered in San Francisco, California. It was the first peer-to-peer lender to register its offerings assecurities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. Lending Club operates an online lending platform that enables borrowers to obtain a loan, and investors to purchase notes backed by payments made on loans. Lending Club is the world's largest peer-to-peer lending platform.

Lending Club enables borrowers to create unsecured personal loans between \\$1,000 and \\$40,000. The standard loan period is three years. Investors can search and browse the loan listings on Lending Club website and select loans that they want to invest in based on the information supplied about the borrower,
amount of loan, loan grade, and loan purpose. Investors make money from interest. Lending Club makes money by charging borrowers an origination fee and investors a service fee.

### Motivation:

People often save their money in the banks which offer security but with lower interest rates. Lending Club operates an online lending platform that enables borrowers to obtain a loan, and investors to purchase notes backed by payments made on loans. It is transforming the banking system to make credit more affordable and investing more rewarding. But this comes with a high risk of borrowers defaulting the loans. Hence there is a need to classify each borrower as defaulter or not using the data collected when the loan has been given.

### About Dataset
The dataset was collected from [Lending Club website](https://www.lendingclub.com/info/download-data.action). It contains complete loan data for all loans issued through the 2007-2015, including the current loan status (Current, Late, Fully Paid, etc.) and latest payment information. The file containing loan data through the "present" contains complete loan data for all loans issued through the previous completed calendar quarter. Additional features include credit scores, number of finance inquiries, address including zip codes, and state, and collections among others. The file is a matrix of about 890 thousand observations and 75 variables. A data dictionary is provided in a separate file called LCDataDictionary

### About This Analysis
The analysis consists of three parts:

**[Part I: Exploratory Data Analysis](#Exploratory_Data_Analysis)**<br>
Major questions to answer:<br>
[1. Does the installment amount affect loan status ?](#Installment_amount)<br>
[2. Does the installment grade affect loan status ?](#Grade)<br>
[3. Which grade has highest default rate ?](#Home_Status)<br>
[4. Does annual income/home-ownership affect default rate ?](#annual_income)<br>
[5. Which state has highest default rate ?](#State)<br>

**[Part II: Text Analysis](#text_analysis)**<br>
[1. Is it that a people with a certain empoyee title are taking up more loans as compared to others ?](#debt_title)<br>
[2. Does a specific purpose affect loan status ?](#debt_purpose)

**[Part III. Model Building](#model_building)**<br>
[1. Cleaning the data](#cleaning_data)<br>
   * Selecting necessary features
   * Taking care of nan values <br>
 
[2. Model Selection](#ModelSelection)<br>
Comparison accuracies of 6 models
   * Model 1 - XGBoostClassifier
   * Model 2 - Support Vector Classifier(SCV)
   * Model 3 - RandomForestClassifier
   * Model 4 - Logistic
   * Model 5 - BalancedBaggingClassifier
   * Model 6 - Decision Tree
