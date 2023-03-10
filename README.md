# Analysis of Accident Victims Evaluation by Four Different Hospitals

## Project Objective

To compare the diagnosis by 4 different Hospitals of the Limbs of Accident Victims as to whether they can be Salvaged or have to be Amputated.

## Data Source

I was provided an excel sheet by the doctors of 4 leading hospitals - Mess, Ganga, LSI, OTA. I have combined the data from all 4 hospitals in the below Excel sheet:
<a href = "https://docs.google.com/spreadsheets/d/1YYBLJnrLSgD7jOrTILs2tOJVsBsBlw-4/edit#gid=1215070420"> Original Hospital Data from Ganga, LSI, Mess and OTA Hospitals </a>

The excel sheet in the following link contains 225 observations of accident victims from each of the 4 mentioned hospitals with the following data:

1. Age
2. Gender
3. Probability of Salvaging the Limbs
4. Probability of Primary Amputation Being Required
5. Probability of Secondary Amputation Being Required
6. Final Diagnosis

It also contains the count of True Positives (TP), True Negatives (TN), False Positives (FP) and False Negatives (FN) cases for each hospital. 

1. True Positives (TP) - The patient's limbs were Correctly evaluated as Salvaged.
2. True Negatives (TN) - The patient's limbs were Correctly evaluated as Amputated.
3. False Positives (FP) - The patient's limbs were Incorrectly evaluated as Salvaged.
4. False Negatives (FN) - The patient's limbs were Incorrectly evaluated as Amputated.

## Data Used

1. Probability of Salvaging the Limbs
2. Probability of Primary Amputation Being Required
3. Probability of Secondary Amputation Being Required
4. Final Diagnosis

## Tools Used

1. Excel
2. Minitab

## Data Transformation

To make things simpler, the following transformations were made on the data:

1. Amputation Probability was considered as the Sum of Probability of Primary Amputation and Secondary Amputation. 
2. The Salvaging and Amputation Prediction of the Final Diagnosis given in terms of probabilities were converted to binary nature by predicting the limbs to be Salvaged for any Salvage Probability above a certain Cut Off Value. 
3. The 6 cut off values chosen were - 

        (i) 0.92
        
        (ii) 0.88
        
        (iii) 0.87
        
        (iv) 0.80
        
        (v) 0.70
        
        (vi) 0.65

## Analysis

Using the TP, TN, FP & FN, the sensitivity of TP% was plotted against the specificity of TN% for the descending order of probability of salvage. This is shown in the excel sheets in the below links, which contain the data for each of the hospital, their cut off based calculations of TP, TN, FP & FN, as well as the graphs of TP% against TN%

### 1. Ganga Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Portfolio/main/Hospital%20Data%20Project/Ganga%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

### 2. LSI Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Portfolio/main/Hospital%20Data%20Project/LSI%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

### 3. Mess Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Portfolio/main/Hospital%20Data%20Project/Mess%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

### 4. OTA Hospital Data with TP% vs TN% graph

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Portfolio/main/Hospital%20Data%20Project/OTA%20Hospital%20Data%20with%20TP%25%20vs%20TN%25%20graph.png)

## Insights

1. Ganga hospital was better than the other hospitals in the evaluation at Salvaging or Amputating Limbs. 
2. LSI is second best at evaluation, going by the graphs, behind Mess and OTA only in the 0.70 Cut Off. 
3. Mess is better OTA in 4 out of the 6 Cut Offs under consideration, behind only in the 0.92 and 0.70 Cut Offs.

## Conclusion

Final Rankings of the 4 Hospitals at evaluation:

1. Ganga Hospital
2. LSI Hospital
3. Mess Hospital
4. OTA Hospital
