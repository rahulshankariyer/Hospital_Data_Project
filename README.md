# Hospital Data Analysis of Polytrauma Patients

## Indian Statistical Institute. June 2018

## Project Objective

The goal was to rank 4 hospitals based on the accuracy of their initial evaluation to final diagnosis, in the salvaging or amputating limbs of accident victims. The ranking was based on an analysis of 225 accident victims’ data (muscle, skin, bone) over one year, from the 4 hospitals. Using Excel to perform Regression Analysis, hospitals and created visual charts using Minitab to present the results. 

## Data Source

The data of 225 accident victims were collected from the 4 hospitals - Mess, Ganga, LSI, OTA - and combined into an <a href = "https://docs.google.com/spreadsheets/d/1YYBLJnrLSgD7jOrTILs2tOJVsBsBlw-4/edit#gid=1215070420"> Excel Sheet </a>

The data had the following information of victims:

1. Age & Gender
2. Muscle, Skin, and Bone scores
3. Probability of Salvaging the Limbs
4. Probability of Primary Amputation Being Required
5. Probability of Secondary Amputation Being Required
6. Final Diagnosis

## Data Used

1. Probability of Salvaging the Limbs
2. Probability of Primary Amputation Being Required
3. Probability of Secondary Amputation Being Required
4. Final Diagnosis

## Tools Used

1. Regression Analysis using Excel
2. Minitab to create visual charts

## Data Transformation

The following transformations were made on the data:

1. Amputation Probability was considered as the Sum of Probability of Primary Amputation and Secondary Amputation. 
2. In order to do a binary prediction, as to whether the limbs will be salvaged or not, six different cut-off values were considered for salvage probability. For any salvage probability above the cut-off, the limbs were predicted to be salvaged and for any salvage probability below the cut-off, they were predicted to be amputated.
3. The 6 cut-off values chosen were - 

        (i) 0.92
        
        (ii) 0.88
        
        (iii) 0.87
        
        (iv) 0.80
        
        (v) 0.70
        
        (vi) 0.65

## Analysis

Using the above cut-off values, the count of True Positives (TP), True Negatives (TN), False Positives (FP), and False Negatives (FN) cases were calculated for each hospital, where - 

True Positives (TP) - The patient's limbs were Correctly evaluated as Salvaged.

True Negatives (TN) - The patient's limbs were Correctly evaluated as Amputated.

False Positives (FP) - The patient's limbs were Incorrectly evaluated as Salvaged.

False Negatives (FN) - The patient's limbs were Incorrectly evaluated as Amputated.

The sensitivity % of TP% was plotted against the specificity % of TN% for the descending order of Salvage probability. This is shown in the graphs below (created in Excel) , for each hospital.

Sensitivity: the ability of a test to correctly identify patients with a disease.

Specificity: the ability of a test to correctly identify people without the disease. 

### 1. Ganga Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Hospital_Data_Project/main/Ganga%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

### 2. LSI Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Hospital_Data_Project/main/LSI%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

### 3. Mess Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Hospital_Data_Project/main/Mess%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

### 4. OTA Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Hospital_Data_Project/main/OTA%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

## Insights (from the graphs)

1. Ganga hospital was better than the other hospitals in the evaluation at Salvaging or Amputating Limbs. 
2. LSI is second best at evaluation, going by the graphs, behind Mess and OTA only in the 0.70 Cut Off. 
3. Mess is better OTA in 4 out of the 6 Cut Offs under consideration, behind only in the 0.92 and 0.70 Cut Offs.

## Conclusion

Final Rankings of the 4 Hospitals at evaluation:

1. Ganga Hospital
2. LSI Hospital
3. Mess Hospital
4. OTA Hospital
