<h2><i> Motivation and problem statement</i></h2>
As COVID-19 rapid growth thorughout the world has caused huge spike in demand of hospital supplies and care, Hospitals across the world have been struggling greatly with the problem of allocating right resources to the right cases and also forecasting the resources required. It becomes crucial for hospitals to understand every factor that can potentially be utilized in demand forecasting of the resources for COVID patients and be helpful in saving lives. In these circumstances, there could potentially be useful information realted to patient's history and severity of COVID symptoms.  
Hence, I would like to explore how COVID-19 severity is related to Patients Medical History procuring patient data of COVID-19 containing specific information regarding patient's history. The dataset was released by the Mexican government which contains a huge number of anonymised patient-related information on their medical history and their data post admittance in hospital due to COVID-19.


<h2> <i>Dataset information</i></h2> 
This dataset is published by Mexican governement and updated on the daily basis. These data include information about COVID-19 patients in Mexico and includes demographic information such as Age, Gender as well as information on patient's medical history such whether the patient has: diabetes, chronic obstructive pulmonary disease (COPD), asthma, immunosuppression, hypertension, obesity, pregnancy, chronic renal failure, other prior diseases, and whether was or is using tobacco. This dataset is published in Spanish language and due to time constraints and lack of Spanish language knowledge, I will be utilizing the dataset that was translated, cleand and published as a Kaggle dataset. The links to Raw Datasource, Cleaned Dataset and Dataset License are below - 
<h4>Dataset Source :</h4> https://www.gob.mx/salud/documentos/datos-abiertos-152127 
<h4>Cleaned Dataset Link :</h4> https://www.kaggle.com/tanmoyx/covid19-patient-precondition-dataset?select=covid.csv
<h4>Dataset License :</h4> https://creativecommons.org/publicdomain/zero/1.0/ 



<h2> <i>Dataset limitations / Unknowns </i></h2> 
Procuring patient data of COVID-19 patients containing patient-specific information regarding patient history and habits is extremely hard. This is mainly due to the regulatory security laws such as HIPAA and GDPR which makes it almost impossible for anyone to get hands-on PHI data. The dataset was released by the Mexican government which contains a huge number of anonymised patient-related information.

<h2> <i>Research questions and hypotheses</i> </h2>

Some of the questions I want to answer from this datset are - 
<ul>
<li> <i><b>Question 1 - </i></b> How did different age group of people get impact by COVID according to their medical history?</li>
  <ul> <i>Hypothesis - </i> People above 60 years of age and severe health conditions are more prone to death by Covid than people with younger age and severe disease conditions </ul>
<li><i><b>Question 2 - </i></b> How their medical history played a role in severity of COVID?</li>
  <ul> <i>Hypothesis -</i> People with diseases such as diabetes and high blood pressure show symptoms earlier and have higher chances of death  </ul> 
<li><i><b>Question 3 - </i></b> Is there one particular disease history that is proving to be deadlier or severe than any other?</li>
   <ul> <i>Hypothesis - </i> Disease that directly impact immune systems and respiratory systems have higher death ratio than other diseases </ul> 
<li><i><b>Question 4 - </i></b> Can we find a pattern in the data to help us decide on the factors which can later be proven helpful in predicting the cases?</li>
   <ul> <i>Hypothesis - </i> Age, gender , type of medical history can be strong predictors of propensity of death from Covid or requirement of Intubation </ul> 
</ul> 


<h2> <i>Background / Related work</i></h2> 
ventilator.
A health crisis of massive proportion such as the current COVID-19 pandemic provides us with an opportunity to ponder and reflect over what we can better in the way we deal with healthcare to make us humans be more prepared and enabled to combat such an event in the future.
During the entire course of the pandemic, one of the main problems that healthcare providers have faced is the shortage of medical resources and a proper plan to efficiently distribute them.
This article summarizes the condition Mexixo is facing very well - https://www.aa.com.tr/en/latest-on-coronavirus-outbreak/pandemic-reveals-mexicos-social-economic-disparities/2002155

<h2> <i>Methodology</i></h2> 

<h4><b>Step 1 - </h4></b> Performing the exploratory data analysis to understand the trends and distribution of time between 'date admitted to hospital' and 'date of death' for Age groups and Gender according to medical history of patients. I will then try to investigate how these different age groups and gender had different death ratios due to COVID-19 

<h4><b>Step 2 - </h4></b> I will further also build a linear regression model to understand the role of age, gender and historical diseases impacting in death due to COVID-19. This will highlight if certain medical history has higher chances of causing a death in patient if infected with COVID-19

<i><h2>Ethical considerations of dataset</h2> - As this dataset contains PII information of patients and each individual can easily be identified with their medical history pattern, it is imporatnt to hadle this data with great care and ananimization </i>
