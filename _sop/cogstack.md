---
title: CogStack
order: 
image:
shorthand: cogstack
---


CogStack is an information and extraction platform which allows us to search the EPR (electronic patient records). It is a catalogue of hospital documents and can be used to identify patient cohorts as well as search for clinical information for other purposes (e.g. AI software evaluation). Please note that CogStack is an index of documents and not an index of patients, so many answers will be buried in the free text of each document that will need analysis. Please also note that access to CogStack needs to be requested by your line manager. There are also two levels of access: a reader and an admin. If you are granted reader access, you will be able to search CogStack but not to export any data. If you need data export, please talk to a colleague with admin access and they can help you retrieve your CSV files.

1.	Log into the GSTT network and open a browser. Please note that if you are using Citrix, you need to use Chrome -- it does not work with Internet Explorer. <br>
2.	Go to https://cogstack.gstt.nhs.uk:5601 and select 'Log in with GSTT authentication'. You may be prompted to input your GSTT Username and Password.
3.	An Access Agreement notice will appear warning you that you are about to see sensitive information. Press the 'Acknowledge and continue' button.
4.	You wil be presented with your home dashboard. Click on the three lines (the menu) on the left-hand side of the screen, just under the 'Elastic' logo and under 'Analytics' tab select 'Discover'.
5. 	You will be then presented with a search bar (at the top), the results panel (centre right) and the index panel (centre left).
6. 	CogStack is built upon ElasticSearch and follows its query logic. Most of the fields within each document are tagged with an ID by which you can use to search through the documents, e.g. 'patient_TrustNumber'. The syntax in general is 

    keyword : "search term" AND keyword : "second search term" OR keyword : "third search term" AND NOT keyword : "exclusion term"

    You can use as many or as few keywords as you wish. You can find the keywords by either inspecting a document or by scrolling through the options that drop down when you click on the search bar. NB that 'body_analysed' means the free text area of the document - your search terms are most likely to appear there. When you are happy with your query, press the 'Enter' or click on 'Update' buttom at the end of the search bar.

7.  The results panel will populate with documents that match your search terms. If your search is very broad, this may take a few seconds. An error box will appear on the bottom right corner if there are errors with the search term itself. To investigate your results, click on the arrow on the left-hand side of each search result to expand it.
8.	The index selected as the default is e&#42;. Different indexes are catalogues of different documents. For most of our purposes, you will want to access either gstt_clinical_documents_letters or gstt_clinical_epr&#42;. The latter contains observations, orders and results and will contain things such as blood test orders and results, pathology results, and radiology reports. The former will contain the letters sent to patient's primary care clinician (usually GP or whoever referred them for treatment) which will contain things such as diagnosis and reports on treatment completion.
9.  If you're looking for images, the index you need is the gstt_clinical_epr_results. The accession numbers for the images are stored under the keyword 'document_AncillaryReferenceID'. The accession numbers in this field may sometimes miss some letters, may be amended to include a hyphen, may be missing a number or have a 1 after 'RJ'. This is an indexing issue. If you find error, you can use the scan date and patient MRN to find the relevant imaging. Both will be exported along with the accession number in your CSV file.
10. To save the results of your query and export them for further processing, first save your query by clicking on the saving menu on the left-hand side of the search bar and click on 'Save current query'. Name your query something sensible that will be easy to recognise. Once your query is saved, click on 'Share' on the top right corner, then select 'CSV Report'. You will then be able to export your results in a CSV file.