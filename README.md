# Shipment dataset
using shipment data to calculate patient's adherence to medicine
# Background
TEPMETKO is indicated for the treatment of adult patients with metastatic non-small cell lung cancer (NSCLC). 
The overall response to treatment was 43% with a median response duration of 10.8 months. 
In this analysis, I wanted to use the patient's shipment data to know more information about the patient's adherence to medicine.
# Analysis plan
1. Medication persistence = total time on treatment as days from the index Rx fill date to the imputed end date for the last Rx written 
(usually 30 days from the fill date), assuming not more than 40 days gap between last date of days supply of previous Rx and fill date of next Rx
2. Discontinuation date = run out date of last Rx observed
3. Discontinuation rate = percentage of patients who discontinued therapy before end of the follow up period
4. Breaks = days gap between last date of days supply of previous Rx and fill date of next Rx
5. Medication Possession Ratio (MPR) = sum of days of supply divided by total number of days in the follow up period (MPR >=0.8 will be classified as adherent) and/or 
Cumulative Medication Gap (CMG) = days gap between each Rx fill, divided by the number of days between the first and last medication fill during the study period
6. Dose titration (reduction), presented as categorical variables, will be examined for patients with >=2 maintenance doses in the follow up period
If the average dose is reduced from 2 daily tablets to 1 daily tablet the patient will be deemed to have had a dose reduction


   

# Outcomes
Treatment duration (persistence), discontinuation, and dose titration (reduction) for NSCLC patients 
