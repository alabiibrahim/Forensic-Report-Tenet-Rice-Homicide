
### INVESTIGATIVE FINDINGS - TENET RICE HOMICIDE

## *Table of Contents*

- [Project brief](#Projectbrief)
- [Objective](#Objective)
- [Methodology](#Methodology)
- [Tools](#Tools)
- [DataModeling](#Data-Modeling)
- [ProcessingAnalysis](#Processing-&-Analysis)
- [Dashboard](#Dashboard)
- [EventReconstruction](Event-Reconstruction)
- [Findings](#Findings)
- [SuspectElimination](#SuspectElimination)
- [Recommendations](#Recommendations)
- [Conclusion](#Conclusion)


**Project brief**

This report investigates the circumstances surrounding the Tenet Rice homicide, focusing on evidence collection, analysis, and interpretation to determine the sequence of events and potential responsible parties.


#### Objective
The objective of this forensic report is to systematically analyze physical, digital, and testimonial evidence to reconstruct the events of the Tenet Rice homicide and provide an unbiased foundation for legal and investigative decision-making


### Methodology
All suspects were evaluated using a weighted behavioural scoring model built on four forensic indicators:

1. **Opportunity:**: This is used to get knowledge of physical presence and door access within the critical time window
2. **Capability:**  failed or forced access attempts indicating restricted-area targeting
3. **Intent:**  abnormal communication activity compared to personal baseline behaviour
4. **Concealment Behaviour:**  sudden silence or activity drop after the event
5. **Confidence:** Calculated score given to individuals based on behavioral activities to helps in investigative findings.
6. **Motive Proxy:**  relationship risk level to the victim

Each suspect received a quantified suspicion score based on deviations from their normal behaviour rather than overall activity totals.


#### Tools


| Tools | Purpose |Dataset|
|---|---|---|
|Power BI| dax measures, Power query |![data](https://github.com/alabiibrahim/Forensic-Report-Tenet-Rice-Homicide/tree/6bcb81e4bd36d8bb3134ef22f7a6c019e84429a3/Datasets) |


## Data Modeling

Datasets contains 4 tables; Suspect, CallRecords, AccessLog, ForensicEvent. All tables are modeled via One to Many relationships using the Suspect_ID column (PK) and Date column (PK)  Star flake schema. A customized CalendarTable, ActivityLog table  for (event timeline analysis), and a customized measures table.

![Image](images/Data%20Modeling.PNG)



#### Processing & Analysis

- Consistent datatype format - Ensure datatypes is consistent across all tables to help prevent data breakage.
- Duplicates removal - Ensures all duplicates records are eliminated.
- EDA - Exploratory analysis was performed using statistical method to calculate needed metrics for report accuracy.
- DAX - measures for report interactivity and dynamism


*Forensic Method* -Applied

- CCTV footage records (For where, when
- Digital forensic like call records (before or after)
- Door Accessed (access attempt)

*Comparative Analysis* 

- After/Before Event call, access.
- Change in behavior activity
- Surveillance



### *Dashboard*


![image](images/T1.PNG)



![image](images/t2.PNG)



![image](images/t3.PNG)



![image](images/t4.PNG)




### Event Reconstruction


Between the victim’s last confirmed sighting and the emergency call, building activity narrowed significantly to a small subset of individuals.

During this period:

* Access attempts became concentrated rather than distributed
* Communication behaviour shifted from routine patterns to targeted bursts
* Multiple individuals ceased activity immediately after the event window

This pattern is inconsistent with routine workplace behaviour and consistent with a coordinated or intentional action period.



### Findings

The scoring model identified three behavioural markers strongly associated with involvement:

 • Presence at secured locations during the event.
 
 • Access attempts inconsistent with job role
 
 • Abrupt behavioural silence following the incident
 
 • The victim was last seen alive at 7:57pm and gunshot heard at 8:00pm.
 
 • Call records show a call between the victim and the primary suspect shortly before the estimated time of death.

 • Failed access attempts to non-restricted areas, indicating suspicious motives.

 • No forced entry was detected, suggesting the victim allowed entry to the attacker (Hotel staff).

 • Suspect made a call immediately after event to the victim's former partner. Susan knight appeared as a staff and investor.

One individual displayed multiple markers simultaneously, Alex Shaw.



### Suspect Elimination

The majority of suspects were eliminated for the following reasons:

* No presence within the event window.
* Behaviour consistent with normal baseline patterns.
* No restricted-area interaction.
* Continuous communication activity after the incident (indicating normal routine).

These individuals are statistically consistent with uninvolved actors or witnesses.

*Prime Suspect Determination*

One subject demonstrated a unique convergence of indicators:

* Verified activity within the critical time window.
* Repeated non-restricted-area access behaviour.
* Communication pattern deviation from baseline.
* Immediate behavioural silence after the incident.
* Relationship category associated with elevated conflict probability.

This combination of opportunity, capability, behavioural deviation and concealment behaviour produced the highest suspicion score among all subjects.



#### RECOMMENDATIONS: 
 
• Conduct a formal interrogation of the suspect focusing on the event time frame.

• Verify the suspect’s alibi against phone tower and CCTV movement records.

• Interview Individuals tagged as "witness" and "person of interest" they might have had involvement directly or indirectly.

• Check for additional camera footage covering exit routes.

• Perform digital forensics on the suspect’s phone few hours to event period.



#### CONCLUSION:

• Based on the timeline correlation, location tracking, and call records, Alex Shaw was present at the crime scene at the estimated time of death.

• The absence of forced entry and the communication between the victim and Alex Shaw shortly before the incident suggest the victim willingly met the suspect.

• The attempts to non restricted areas indicates bad intentions. 

Taken together, the evidence strongly supports the suspect’s involvement in the incident and justifies further legal investigation and interrogation.
