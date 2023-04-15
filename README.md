# PORTUGUESE-BANK-MARKETING-ANALYSIS

## **Problem Statement**

Task 1:-Prepare a complete data analysis report on the given data.

Task 2:-Create a predictive model which will help the bank marketing team to know which customer will buy the product.

Task3:-Suggestions to the Bank market team to make customers buy the product.


## **About Dataset**

This dataset is about the direct phone call marketing campaigns, which aim to promote term deposits among existing customers, by a Portuguese banking institution from May 2008 to November 2010. 


## Data Description

* age (numeric) age of customers

* job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')

* marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)

* education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')

* default: has credit in default? (categorical: 'no','yes','unknown')

* housing: has housing loan? (categorical: 'no','yes','unknown')

* loan: has personal loan? (categorical: 'no','yes','unknown')

### Related with the last contact of the current campaign:

* contact: contact communication type (categorical: 'cellular','telephone')

* month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')

* day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')

* duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

###  other attributes:

* campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)

* pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)

* previous: number of contacts performed before this campaign and for this client (numeric) 

* poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')

###  social and economic context attributes

* emp.var.rate: employment variation rate - quarterly indicator (numeric)# it represents how many people were hired or fired due to the shift in the condition of economy.

* cons.price.idx: consumer price index - monthly indicator (numeric) # It represents the measurement of trends in the price of products,at constant quality.

* cons.conf.idx: consumer confidence index - monthly indicator (numeric)# It shows the future development of households consumption and savingsbased upon answer regarding there expected financial situation.

* euribor3m: euribor 3 month rate - daily indicator (numeric)# Its an interbank market where bank borrow loan from other bank for which they pay interest. 

* nr.employed: number of employees - quarterly indicator (numeric)

Output variable (desired target):

* y - has the client subscribed a term deposit? (binary: 'yes','no')

## Model Comparison Report

* On comparing the accuracy of all the models we got good accuracy of 94 % in Random Forest Classifier algorithm. Hence we will use Random Forest algorithm for our future predictions.

## Conclusions and recomendations

What general recommendations can be offered for a successful marketing company in the future?

This analysis can be carried out at the level of individual bank branches as does not require much resources and special knowledge (the model itself can be launched automatically with a certain periodicity). 

Potentially similar micro-targeting will increase the overall effectiveness of the entire marketing company.

1. Take into account the time of the company (March,September and october)

2. Increase the time of contact with customers (perhaps in a different way formulating the goal of the company). we should try to contact the people via cellular mode and it is also possible to use other means of communication.

3. Focus on specific categories. The model shows that students and senior citizens respond better to proposal.

4. It is imperative to form target groups based on socio-economic categories. Age, income level (not always high), profession can accurately determine the marketing profile of a potential client.

Given these factors, it is recommended to **concentrate on those consumer groups** that are potentially more promising.

The concentration of the bank’s efforts will effectively distribute the company’s resources to the main factor - the bank’s contact time with the client - it affects most of all on conversion.

The continuation of such a study may be the **formation of a clear customer profile** - by age, gender, income and other factors, as well as the adaptation of the product itself (deposit) for a specific category of consumer.

## Report on Challenges faced

* While encoding catagorical data into numerical data, for certain features we cannot predict the numerical values manually as it depend on domain knowledge. hence we have used Label encoder for these features.

* In EDA some feature showing uniform distribution so it was difficult to predict the relationship between features.
