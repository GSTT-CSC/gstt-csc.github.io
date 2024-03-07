---
layout: project_page
title: Dental Referrals 
status: Developing
image: 
summary: Automated dental referral vetting at GSTT
csc-lead: <a href="/team_member/Anil.html">Anil Mistry</a> <a href="/team_member/Anil.html">Anil Mistry</a> 
modality: Text / NLP / Email
pathology: Dental 
rationale: Dental referrals are a large administrative burden of admin staff and dental consultants at GSTT.     
patient-pathway: Dental Services admissions at GSTT
training-data: N/A
errors:  
goals: Create an application that can extract relevant information from incoming dental referrals to ease the administrative workload in uploading new referrals to EPIC upload. Automate the referral vetting decisions to reduce administrative workload of Dental Consultants.   
success-criteria: Reduction in referral upload time allocated to admin staff. Reduction in dental referral vetting tasks completed by Dental consultants. Additional clinics attended by dental consultants. 
---

<b>Clinical lead</b>: Dr Poonam Kalsi, Dr.Jo Johnson, 
<br>
<br> **Rationale:**
<br>
<br>

The Dental Directorate receives approximately 1 in 10 of all secondary care referrals from primary care. This presents 
a significant administrative burden on both the Dental Admin staff for processing and uploading there referrals to 
EPIC, and for dental consultants to vet each referral to accept/ reject/ redirect. 

Dental services in South East London are provided by Guys and St thomas, King's College Hospital and Queen Mary Sidcup,
where all referrals are received through a common entry point and referrals requesting the shortest wait time will be 
given to the trust with the most free capacity at that point. All hospitals use EPIC.

This application aims to automate the referrals admin and vetting process to reduce the burden on staff, by delivering in two phases

**Phase 1**
<br>
Use the current referral software API to intercept the referral, analyse the content and organise the information in a
way that can vastly speed up the administrative task of uploading the referral to EPIC. 


**Phase 2**
<br>
The free text for the reason for referral will be passed through an LLM to extract all relevant and appropriate
information to suggest if the referral should be accepted / rejected / redirected, based on a decision tree of vetting
questions (a combination of local and national vetting guidelines for each dental specialism.)

The result and explanation will be uploaded to EPIC to assist dental consultants vetting decisions. With improved 
confidence in the result, certain vetting tasks could be reviewed by administrative staff, where only more complex 
referrals will need a review by a consultant. 


<b>Project Plan</b>:

1. Proposal
2. Scoping
3. Requirement gathering
4. Clinical Risk Management 
5. Design Specification 
5. Development
6. Proof of Concept
7. MVP

<br>
<br>

<b>References</b>: 
