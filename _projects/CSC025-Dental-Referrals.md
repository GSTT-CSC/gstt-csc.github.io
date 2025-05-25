---
layout: project_page
title: Dental Referrals
status: Concluded
image: /assets/img/projects/dental_referral_logo.png
summary: Dental referral processing for SEL.
csc-lead: <a href="/team_member/anil.html">Anil</a> and <a href="/team_member/elise.html">Elise</a>
modality: Operational
pathology: Dental conditions requiring secondary care referrals
---
---

This project has been delivered and concluded. Despite the development of dedicated software, the problem was finally resolved by utilising native capabilities of the software currently in use to receive the referrals. 

---

<b>Clinical leads</b>: Joana Johnson, Poonam Kalsi
<br>
<b>Administrative leads</b>: Olivia White, Adma Mills


This application automatically processes dental referral questionnaire responses for South East London (SEL). SEL secondary care dental services are provided by Guy's and St Thomas' NHS FT, King's College Hospital, and Queen Mary Sidcup, where the referral process is the same for each care provider. Thus the application can be used in all three sites. 

Referrals to the GSTT dental department can represent up to 10% of all secondary care referrals. The manual referral checking, patient EHR (Electronic Health Record) upload, and vetting tasks can represent a significant burden to clinicians and administrative staff. This application assists staff in these tasks to improve speed and efficiency.

This project takes a staged approach to automating the referral vetting process. 
1. Automatically perform the first checks on the referrals to assist admin staff in the upload of the referrals to the EHR. This includes sending the referrals to the Trust with the shortest wait time (when applicable), and extracting/evaluating each attachment submitted from the referral questionnaires.
2. Automate the referral vetting process by providing a suggestion and rationale for accepting/rejecting/redirecting the referral for each specialism, implementing local and national vetting guidelines.
3. Automate the task of uploading the referral to the EHR for each Trust using HL7 or FHIR messaging.
