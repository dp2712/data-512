<h2>Abstract </h2>

I explored how COVID-19 severity is related to patient's medical history / pre-existing conditions to understand if knowledge of patient's medical history can be helpful for hospitals to forecast number of patients who can witness severe outcomes if tested COVID-19 positive and plan for the resources and medical supplies better.
As COVID-19 rapid growth thorughout the world has caused huge spike in demand of hospital supplies and care, hospitals across the world have been struggling greatly with the problem of allocating right resources to the right cases and also forecasting the resources required. It becomes crucial for hospitals to understand every factor that can potentially be utilized in demand forecasting of the resources for COVID patients and be helpful in saving lives. In these circumstances, this information can be proved really useful for hospitals and medical practicioners across teh world and benefit them in planning resources better.
After the analyzing the data I found that - 

<ul>
    <li>People above age of 60 ; with pre-existing condition of Pneumonia and COPD are at really high risk of dying if tested positive for COVID-19</li>
    <li>Intubation rates for patients with above characteristics are not satisfactory which suggests either hospitals do not have resources or they lack methods or knowledge to appropriately allocate resources to high risk prone patients</li>
    <li>Acceptable accuracy of prelimanary logistic model suggests us that patients medical history can tell us a lot about the severity of COVID-19 symptoms and hospitals must utilize this data to forecast the cases and their severity , which can help in preparation of medical care resources beforehand and act as an proactive measure for hospitals rather than preventative</li>
    </ul>

<h2>Background and Related Work</h2>
This article summarizes the condition Mexico government is facing very well - https://www.aa.com.tr/en/latest-on-coronavirus-outbreak/pandemic-reveals-mexicos-social-economic-disparities/2002155 and though there are multiple prediction models which have been made on the dataset to predict if patients with certain pre-conditions are more susceptible to death due to covid, I wish to use this datset for more detailed level study exploring specifically age and pre-existing conditions variables.

<h2>Dataset information</h2>
This dataset is published by Mexican governement and updated on the daily basis. The data includes details about COVID-19 patients in Mexico and contains information such as Age, Gender, data of first covid symptom, date of entry to the hospital, patient's medical history, and whether patient died or recovered. This dataset is published in Spanish language and due to time constraints and lack of Spanish language knowledge, I will be utilizing the dataset that was translated, cleand and published as a Kaggle dataset under the name <i>'COVID-19 patient pre-condition dataset'</i>. The links to Raw Datasource, Cleaned Dataset and Dataset License are below - <br />
<b>Dataset Source :</b> https://www.gob.mx/salud/documentos/datos-abiertos-152127 <br />
<b>Cleaned Dataset Link :</b> https://www.kaggle.com/tanmoyx/covid19-patient-precondition-dataset?select=covid.csv <br />
<b>Dataset License :</b> https://creativecommons.org/publicdomain/zero/1.0/ <br />


  
