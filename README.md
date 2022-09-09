# Data Analysis Project _  Oral Diabete Drug Category Overview
* This is the **team project** that I was done at my university by using R.

* This paper is the result of data analysis project about the Oral Diabete drug category data. There are 4 main
parts in this paper, including background information, data description, model description and finding &
implementation. we estimate a factor-analytic choice model to identify what product benefits each physician primarily seeks for

* This paper will focus on only 4 medicines, including Actos, Lantus, Avandia and Glucophage/Metformin with the time is in the last 40 weeks

# Data Description

* The orginal data contain 182,680 patient visits where a prescription was written by 2,127 physicians.
This data was conducted for over an 18 month period from January 1st, 2007 to June 30th, 2008.

* we select “regular” physicians, those characterized by the following two conditions.
First, the doctor has made at least one prescription every month. Second, the doctor has changed the
prescription or not (switched brand). Moreover, we confine our attention in our analysis to 4 drugs
“Actos”,“Lantus”, “Glucophage/Metformin”, “Avandia”. 

* The top prescription share drugs are Glucophage/Metformin and Actos. Glucophage/Metformin, the largest prescription share drug (51.5%) is also the most requested by patients (53%). Actos is the second drug for prescription (24.8%) Avandia accounts for only 4.4% in prescription. 

![Team Project - AVG Secure Browser 9_9_2022 5_12_42 PM](https://user-images.githubusercontent.com/99704273/189304092-8bb3dbc2-6dfb-4d9a-a965-c15fb02615d4.png)
![Team Project - AVG Secure Browser 9_9_2022 5_13_52 PM](https://user-images.githubusercontent.com/99704273/189304329-acabcd20-de86-4949-8d18-6f5181e43ae6.png)

# Model description

**choice ~ goodwill|severity+age+insurance**

* goodwill - alternative specific variable and 3 patient specific variables (severity, age, insurance type)

* **PATIENT_AGE**  the age of the patien

* **SEVERITY**  the patient’s condition (mild, moderate and severe)

* **PATIENT_INSURANCE_TYPE_DESC**  the type of insurance plans that the patients own

# Findings

* The model estimation results show that Actos have a tendency to be prescribed more to senior patients, relative to the 3 other drugs.

* Glucophage/Metformin, Lantus and Actos are more likely to be prescribed to patients with private insurance, relative to Avandia.

* In terms of severity condition, Glucophage/Metformin turns out to have higher probability of prescription to mild patients, relative to Actos
