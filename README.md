# CapcoHackathonTeamAUC

**The Files are**
1.LPD_Merged
2.Final Code in .py and .ipynb fofomat
3.Loan Details-File showing the assumed Interest rates and Tenure for differnt loans
4.CleanFileUsedforAzureML-Cleaned file used for running ML algorithms in Azure ML

Apart from this two more ML models (Classification to predict the Loan eligibility and Regression to predict the Spread(Risk Profile) are created in Azure ML Studio


**Important Links**

1.The below link is a web app containing details of all existing users (This is used by the chatbot to retrieve existing customer details and predict loan eligibility)

https://script.google.com/macros/s/AKfycbzQCLQLM6PMW3D-OSovBuHxWUvPjmD2UbkrEUvpYQyZQiyLVOD5E5tV9SbWM_C1QeBe/exec

i)This was created using Google Sheets and App script
ii)A web app was deployed and the Chatbot queries the Web app through an API to get customer details
iii)These customer details are then used to predict eligibility

2.The below link is a Website where the Chatbot is hosted

www.a-win-in

The website was created from scratch using wordpress and the chatbot was deployed.A form is also created to capture information from users who are uncomfortable sharing details using the chat window

3.Chatbot was created using Bot Press 

https://botpress.com/

Chatbot as claimed by the website 'The first next-generation chatbot builder powered by OpenAI'

4.Basic Flow chart on how solution was created

**ML Model and Chatbot**
1.The two original datasets were merged and the Age and Gender column were used from the Product recommender Dataset along with the Loan predction dataset.
2.The merged Dataset went through Data ingestion,Data preprocessing,EDA,Outlier handling,normalization and Feature engineering by using google collab notebook.A csv dump was taken of the data after cleaning.
3.The cleant csv file was used to run Classification models  on the notebook and the model was pickled
4.The clean csv file was also used to run ML models in Azure ML Studio to check for better models
5.The best model was deployed on Azure
6.As part of risk profiling the Spead of every customere was calculated.This was done by runnung a linear regression model with the same dataset but with the target varaible being Current Loan Amount (Loan Status column was dropped),The spread was used an an indicator to predict the loan exposure the Bank could have while giving out the loan
6.The Chatbot was created in Bot press and used an API to talk to the deploed ML model
7.A web app was created using google sheets and App script which served as a database to retrive customer deatils while predicting loans for existing customers
8.The chatbot talked to the Web app through an API- to retreive customer details
9.In order to hedge risks associated with lending,The chatbot incorporated dynamic interest rates for loans based on the final loan prediction score.
10.A website was created to simulate a bank website and the chatbot was depoloyed into the website
11.A Form was also created on the website to collect details from customers who were not comfortable giving details via chat



