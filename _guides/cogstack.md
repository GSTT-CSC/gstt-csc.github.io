---
title: CogStack
order: 
image:
shorthand: cogstack
---


[CogStack](https://cogstack.org/) is an application framework that allows us to extract information from unstructured data sources, e.g. electronic health/patient records (EHR/EPR).
At Guys and St Thomas' NHS Foundation Trust (GSTT), it contains a catalogue of hospital documents from several of our clinical data sources and can be used to identify patient cohorts, as well as search
for clinical information for other purposes, such as AI software evaluation. 

⚠️ Please note that CogStack is an index of documents and **not** an index of patients, so much of the data's worth will be focused in the free text of each document and will consequently require further analysis.

To gain access to CogStack, your request will need to be issue via your line manager to the CogStack team. This request should indicate which level of access you require, i.e. reader and/or admin. 
If you are granted reader access, you will be able to search CogStack but not export any data. 
If you do need to export data but do not/were not granted admin access, you will need to speak with a colleague who does have admin access and they will be able to help you export your data.

1. Log into the GSTT network and open the Chrome web browser (it does not work with Internet Explorer).
2. Go to https://cogstack.gstt.nhs.uk:5601 and select **Log in with GSTT authentication**. You may be prompted to input your GSTT username and password.
3. An Access Agreement notice will appear warning you that you are about to see sensitive information. Press the **Acknowledge and continue** button.
4. You wil be presented with your home dashboard. Click on the three lines (the menu) on the left-hand side of the screen (just under the **Elastic** logo and under **Analytics** tab) and select **Discover**.
5. You will be then presented with a search bar (at the top), the results panel (centre right) and the index panel (centre left).
6. CogStack is built upon [ElasticSearch](https://www.elastic.co/) and follows its query logic. Most of the fields within each document are tagged with an ID by which you can use to search through the documents, e.g. `patient_TrustNumber`. The syntax in general is: `keyword : "search term" AND keyword : "second search term" OR keyword : "third search term" AND NOT keyword : "exclusion term"`. You can use as many or as few keywords as you wish, and you can find the keywords by either inspecting a document or by scrolling through the options that drop down when you click on the search bar.
  - Please note that `body_analysed` means the free text area of the document, i.e. your search terms are most likely to appear there.
7. These documents are collated into catalogues represented by indexes, and although the default index is a good place to start, we recommend accessing `gstt_clinical_documents_letters`, `gstt_clinical_epr`, and/or `gstt_clinical_epr_results` for most purposes.
   - The first will contain the letters sent to a patient's primary care clinician (usually their GP or whoever referred them for treatment), which will contain details such as diagnosis and reports on treatment completion.
   - The second contains observations, orders and results, such as blood test orders and results, pathology results, and radiology reports.
   - The third will enable you to find accession numbers for the images stored under the keyword `document_AncillaryReferenceID`.
8. When you are happy with your query, press the **Enter** or click on **Update** button at the end of the search bar.
9. The Results panel will populate with documents that match your search terms. If your search is very broad, this may take a few seconds. An error box will appear on the bottom right-hand corner if there are errors with the search term itself.
   - To investigate your results, click on the arrow on the left-hand side of each search result to expand it.
10. If you have admin access, you will be able to save your query results and export them for further processing. To do so:
    - First, save your query by clicking on the saving menu on the left-hand side of the search bar, click on 'Save current query' and use a sensible name that will be easy to recognise later. 
    - Once your query is saved, click on **Share** on the top right-hand corner, then select **CSV Report**. This will output your results as a CSV file.