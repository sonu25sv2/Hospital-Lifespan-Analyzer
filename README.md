<h1 align="center">Hospital Mortality Rate SQL Analysis</h1>

<p align="center">
  <img src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/25aa4420-b6e8-458c-bc51-f6022b66d717)" />
</p>

[Dataset Used](https://www.kaggle.com/datasets/mitishaagarwal/patient/data)


**Tools Used:**

 • SQL - For analysing the data set and deriving insights by running queries


 • Microsoft Excel - For cleaning and understanding the data

**Aim of the project :** To study the mortality rate in hospitals, how does it relate to factors such as age, ethnicity, comorbidities, gender, weight, and BMI and come up with correlations that can help health care professionals to be better equiped with information to reduce the in-hospital deaths.

**Business Problem:** Health care professionals (HCPs) are trying to identify the reason why a patient succumbs to death while being admitted in a hospital. If they have a clear understanding of why they loose a patient, they will be able to reduce the mortality rate by implementing systematic interventions that treats the specific individual based on factors mentioned above. This will reduce the in-hospital mortality rate significantly.

**Approach & Solution:** To begin adressing the business problem at hand, I started by importing the data to MS Excel, I cleaned it up and then studied the dataset carefully to get a big picture view. I then imported it to an SQL editor and proceeded with the analysis by writing queries that extracted meaningful insights from the data. The granularities mentioned about patients such as age, gender, ethnicity, BMI, weight, height, illnesses, heart rates among others played a key role in my analysis. Through these queries, various patterns and correlations emerged that could provide HCPs significant insights and aid them in reducing in-hospital deaths.  

**Insights:** A thorough SQL analysis revealed some very interesting and some expected results from the dataset. Here are some of the findings from my analysis:

1. The hospital mortality rate is 6.34% i.e. for every 10,000 patiets admitted in the hospital, 634 patients passed away
   
    <img width="300" alt="Screenshot 2024-02-27 at 1 52 25 PM" src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/e457a431-0da9-4cb7-8eaa-5612b73677ca">

2. Age is big contributing factor for the mortality rate in patients. We can clearly see from the below output how each age group is affected:
   
    <img width="300" alt="Screenshot 2024-02-26 at 8 44 27 PM" src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/0e4aab99-15cc-4d6f-bd17-e0e33daec7df">

3. The below data categorizing people in a 10 year age interval reveals an interesting trend. The mortality rate in children aged 9 or below is the highest among all other age groups. The second highest, as expected, is of the people aged between 80 and 89. The nubmber of people admitted between the ages of 50 to 89 is almost 3 times the number of people admitted between 0 and 49 years. We can also observe that the mortality rate keeps on increasing with increasing age (except the outilier 0 to 9 years interval).
   
    <img width="500" alt="Screenshot 2024-02-26 at 8 32 19 PM" src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/632c687f-acbe-469d-87b1-b06be1528008">

4. The below data that shows the correlation between the reason a person was admitted to an ICU and their respective death rates. It's noteworthy that the maximum probability of death was "Floor" (11.8), while the highest number of people were admitted with in the "Accident and Emergency" icu_admit_source (i.e. the location of the patient prior to being admitted to the unit) and it also saw the highest number of deaths.

    <img width="425" alt="Screenshot 2024-02-26 at 9 18 55 PM" src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/146573a6-5052-4e4d-b65d-3cfa68d57c4a">

5. An unusual insight came to the surface when I analysed the death rate among the patients with different illneses i.e., diabetes was the top reason of death among patients, even more than any type of cancer. The data below shows the top 2 reason for death among patients.

    <img width="400" alt="Screenshot 2024-02-26 at 9 33 38 PM" src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/b5309b66-8853-4baf-972f-535aa265bb26">

6. Another interesting correlation emerged when I analysed the data for patients' stays in ICU wards. As demonstrated from the data below, the longer patients stayed in an ICU ward, lower were their chances of survival.
   
    <img width="500" alt="Screenshot 2024-02-26 at 9 34 30 PM" src="https://github.com/anuragagarwal96/Hospital-Mortality-Rate-SQL/assets/43496215/b5c18b44-b02c-4f00-a36d-15d19a0c0b8b">


**Conclusion:** The above analysis is a very strong indicator of several factors that contributes to an increased mortality for patients

  • Comorbidities: It's interesting to note that among all comorbidities, diabetes killed the maximum number of people (24.5%). This number is way ahead of people passing away even due to cancer. Apart from this, heart rate is an important indicator of the cardiovascular health and physiological status of a patient. Conditions such as tachycardia (increased heart rate) or bradycardia (low heart rate), is a strong sign of underlying cardiovascular dysfunction. There is enough documented research that shows that abnormal heart rates are directly or indirectly associated with increased mortality risk. Hospitals should educate their diabetes and heart patients about a healthy lifestyle so that their conditions remain stable. In the scenario of any cases going wrong, hospitals should be better prepared to administer treatment targetted to tackle these diseases.

  • Age: Increased age has been a major factor in higher number of in-hospital deaths. Nearly 20% of people aged 70 and above succumbed to in-hospital deaths. Another significant outlier was the death rate in children aged between 0 to 9 years which was the highest in 10 year aged intervals. Therefore hospitals need to be better equipped to deal with these age groups to help them reduce the mortality rate.

  • Length of ICU stays: From my analysis it has been shown that the patients who stayed in ICU wards for longer had a higher death rate.
