# Health Admission Prediction Project

## **Project Overview**

This project aims to analyze and predict health outcomes for patients admitted to a hospital based on various factors such as demographics, medical conditions, lab results, and duration of stay. The dataset includes detailed information about patient admission, diagnosis, and health status during their stay, which can be used to predict future patient outcomes, such as discharge or medical complications.

The project is part of my **final assignment** for the **"Introduction to AI & Data Science"** course at the **Faculty of Computer Science, Universitas Indonesia**.

## **Dataset Description**

The dataset contains information about patients admitted to the hospital, including general details, diagnosis, lab results, and duration of stay. Below is a description of the key columns in the dataset:

### **Data Columns:**

- **SNO**: Serial Number (unique identifier)
- **MRD No.**: Admission Number
- **D.O.A**: Date of Admission
- **D.O.D**: Date of Discharge
- **AGE**: Patient's age
- **GENDER**: Patient's gender (F for Female, M for Male)
- **RURAL**: Patient's household area (U for Urban, R for Rural)
- **TYPE OF ADMISSION-EMERGENCY/OPD**: Type of admission (O for Outpatient, E for Emergency)
- **month year**: Month and year of admission
- **DURATION OF STAY**: Duration of stay in the hospital (in days)
- **duration of intensive unit stay**: Duration of stay in the intensive care unit (ICU)
- **SMOKING**: Whether the patient smokes (1 for True, 0 for False)
- **ALCOHOL**: Whether the patient drinks alcohol (1 for True, 0 for False)
- **DM**: Diabetes Mellitus (1 for True, 0 for False)
- **HTN**: Hypertension (1 for True, 0 for False)
- **CAD**: Coronary Artery Disease (1 for True, 0 for False)
- **PRIOR CMP**: Cardiomyopathy (1 for True, 0 for False)
- **CKD**: Chronic Kidney Disease (1 for True, 0 for False)
- **TLC**: Total Leukocytes Count
- **PLATELETS**: Platelets count
- **GLUCOSE**: Glucose level in the patient
- **UREA**: Urea level
- **CREATININE**: Creatinine level
- **BNP**: B-type Natriuretic Peptide level
- **RAISED CARDIAC ENZYMES**: Elevated cardiac enzyme levels
- **EF**: Ejection Fraction
- **SEVERE ANAEMIA**: Whether the patient has severe anemia (1 for True, 0 for False)
- **ANAEMIA**: Whether the patient has anemia (1 for True, 0 for False)
- **STABLE ANGINA**: Whether the patient has stable angina (1 for True, 0 for False)
- **ACS**: Acute Coronary Syndrome (1 for True, 0 for False)
- **STEMI**: ST Elevation Myocardial Infarction (1 for True, 0 for False)
- **ATYPICAL CHEST PAIN**: Whether the patient has atypical chest pain (1 for True, 0 for False)
- **HEART FAILURE**: Whether the patient has heart failure (1 for True, 0 for False)
- **HFREF**: Heart Failure with Reduced Ejection Fraction (1 for True, 0 for False)
- **HFNEF**: Heart Failure with Normal Ejection Fraction (1 for True, 0 for False)
- **VALVULAR**: Valvular Heart Disease (1 for True, 0 for False)
- **CHB**: Complete Heart Block (1 for True, 0 for False)
- **SSS**: Sick Sinus Syndrome (1 for True, 0 for False)
- **AKI**: Acute Kidney Injury (1 for True, 0 for False)
- **CVA INFRACT**: Cerebrovascular Accident Infarct (1 for True, 0 for False)
- **CVA BLEED**: Cerebrovascular Accident Bleed (1 for True, 0 for False)
- **AF**: Atrial Fibrillation (1 for True, 0 for False)
- **VT**: Ventricular Tachycardia (1 for True, 0 for False)
- **PSVT**: Paroxysmal Supraventricular Tachycardia (1 for True, 0 for False)
- **CONGENITAL**: Congenital Heart Disease (1 for True, 0 for False)
- **UTI**: Urinary Tract Infection (1 for True, 0 for False)
- **NEURO CARDIOGENIC SYNCOPE**: Neuro Cardiac Syncope (1 for True, 0 for False)
- **ORTHOSTATIC**: Orthostatic Hypotension (1 for True, 0 for False)
- **INFECTIVE ENDOCARDITIS**: Infective Endocarditis (1 for True, 0 for False)
- **DVT**: Deep Venous Thrombosis (1 for True, 0 for False)
- **CARDIOGENIC SHOCK**: Cardiogenic Shock (1 for True, 0 for False)
- **SHOCK**: General Shock (1 for True, 0 for False)
- **PULMONARY EMBOLISM**: Pulmonary Embolism (1 for True, 0 for False)
- **CHEST INFECTION**: Chest Infection (1 for True, 0 for False)
- **OUTCOME**: Outcome of the patient (Discharge, DAMA - Discharged Against Medical Advice, Expiry)
- **HB**: Hemoglobin level

## **Project Objectives**

The goal of this project is to:

1. Analyze the health admission data to understand the relationships between patient demographics, medical conditions, and hospital outcomes.
2. Apply machine learning techniques to predict patient outcomes based on various factors.
3. Use statistical analysis and data visualization to explore and present insights.
