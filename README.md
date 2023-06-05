# SepsisProject
## Overview  
The Sepsis project involved the analysis of a vast dataset comprising over 1.5 million data points from more than 40,000 ICU patients. This dataset included hourly records, demographic information, and the presence of a sepsis label indicating the hour of sepsis diagnosis. Additionally, the project included the bloodwork test results of 34 key biomarkers associated with sepsis.  
The project aimed to achieve the following objectives:
- Demographic and ICU Stay Information: Analyze the demographic information and ICU stay details of the patients to identify potential patterns and calculate key performance indicators(KPIs).  
- Biomarker Correlation Analysis: With a specific focus on Hematocrit (Hct), Platelets, and White Blood Cell (WBC) counts, investigate their relationship with sepsis to gain valuable insights. 
- Analysis of Sepsis Effects on Organs: Utilize a combination of crucial biomarkers and specific criteria to examine the impact of sepsis on various organs. Focus specifically on utilizing the Acute Respiratory Distress Syndrome (ARDS) criteria for lung analysis.  
- SIRS (Systemic Inflammatory Response Syndrome) Task: Lead the identification of early signs of sepsis by applying SIRS criteria. Develop a conditional formatting spreadsheet with email alert functionality to promptly notify responsible hospital staff when patients meet pre-alert criteria, ensuring immediate attention.    
- Apache II(Acute Physiology and Chronic Health Evaluation II) Score Analysis: Utilize the Apache II scoring system as a tool to assess the severity of illness and accurately predict patient mortality rates.  
  
By conducting these comprehensive analyses, the project sought to deepen our understanding of sepsis, identify critical factors related to its development and progression, and provide valuable insights that can potentially assist in early detection and treatment strategies.  
Check the interactive dashboards on my [Tableau Site](https://public.tableau.com/app/profile/xinchen)   

### Dashboard 1: Demographic and ICU Stay Information  
**Advanced Features**  
- Utilized **Calculated Fields**, **Level of Details Expressions(LOD)** with the "FIXED" keyword to accurately classify patients into sepsis, non-sepsis, and onset sepsis  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/0bcd7e06-a4ca-49c9-8a4c-9b2e7cf9322c)  
- Employed **Dual Axes** to create visually appealing **donut chart** and **lollipop chart**  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/66e8477d-6dab-467b-afdc-15b3e69cd80d)  
**Insights**:  
- 6% of ICU patients developed Sepsis during their stay.  
- 51% of ICU patients had a hospital stay duration of 2 days.  
- 96% of patients were admitted by the hospital before being transferred to the ICU.  

### Dashboard 2: Correlation between the Complete Blood Count  
**Advanded Features**  
- Employed a **statistical tool** to calculate the median and visually represented the **median distribution** through a **histogram chart**.  
- Utilized **bin** to  segment a specific patient's Hct test results and analyzed the resulting distribution.    
- Demonstrated the correlation between median Hct, Platelets, and WBC through a **pairplot** visualization.      
![alt text](https://github.com/chen8122/SepsisProject/blob/master/Sepsis2%20-%20Correlation%20between%20CBC%20biomarkers.png)
**Insights**:  
- Observed that patients undergo varying combinations of bloodwork tests, indicating that not all patients receive the same set of tests each time.  
- 95% of ICU patients underwent Hct tests, with one patient having a remarkable 114 instances of Hct tests during the stay.  
- Utilized the median values of specific bloodwork results and identified that patients with onset sepsis exhibited the highest correlation between WBC and Platelets.    
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/2afc7e99-519b-484d-9c25-21bae2bfed5a)  

### Dashboard 3.1: Lung Analysis - ARDS Criteria  
**Advanded Features**  
- Implemented **parameters** and **filters** to create interactive **swap sheets** functionality, enabling users to effortlessly select and display their preferred sheet.  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/efc3f595-7775-463b-9516-910c397350b2)  
- Added **custom icons** to enhance the visual appeal and user experience.  
- Added **navigation bottom** to hide/show **slider controler**.  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/c4f42327-f9f1-4c59-ad2a-1fbda9e921f8)    
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/4a878ec8-aabf-47a8-ac82-0bfcb52b98a0)  
**Insights**:  
- By conducting a comparative analysis with PaO2, it has been demonstrated that the PaO2/FiO2 ratio can be served as an economical alternative measurement utilized in the detection of lung injury.  
- A higher proportion of ARDS normal patients tend to have longer lengths of stay in the ICU, whereas a higher proportion of ARDS critical patients exhibit shorter lengths of stay.  

### Dashboard 3.2: Lung Analysis - Ventilation Usage



### Dashboard 4: SIRS(Systemic Inflammatory Response Syndrome) Analysis  
**Advanded Features**  
- Utilized **calculated fields**, **Level of Details Expressions(LOD)** with the "FIXED" keyword to specifically target and identify the SIRS trigger hour for patients.    
- Implemented **dummy axes** technique and formatted cell colors to effectively highlight abnormal test results, enabling quick identification and analysis.  
- Added URL actions to implement email alerts, ensuring the prompt notification of responsible hospital staff when patients meet the pre-alert criteria, facilitating timely attention and response.   
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/badbfcc7-cff1-4148-828d-32715470b8cf)  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/f793236e-bb6d-455d-bb15-89e632eb9e95)  

### Dashboard 5: Acute Physiology and Chronic Health Evaluation II(APACHE II) Score  
**Advanded Features**  
- Utilized **parameters** to enable real-time access for doctors, allowing them to check the current distribution of APACHE II scores for all patients.  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/24db0b59-c48a-480c-9d56-d05c56c4ff84)  
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/685d4263-196f-4c38-9ff0-1e0af7e0be17)  
- Applied a complex calculation methodology to incorporate criteria based on all 13 biomarkers, thereby deriving the APACHE II score. Take `Creatinine` for an example: 
![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/003dbd4e-a895-4feb-af6e-a823d1fbbad7)  

![image](https://github.com/chen8122/SepsisData_Tableau/assets/9794705/27c2f7e6-e230-4d2f-9399-1e6f0137f14a)

