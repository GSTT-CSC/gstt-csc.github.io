---
title: OMOP
shorthand: OMOP
---


#### What is it?
OMOP is a common data model designed for standardising and analysing healthcare data from different sources for observational research. The OMOP Common Data model enables the structured examination of diverse observational databases. This methodology involves converting data from these databases into a unified format (data model) and consistent representation (terminologies, vocabularies, coding schemes). Subsequently, researchers can conduct systematic analysis using a set of standardised analytic routines specifically designed for the common format.

#### Importance of Data Standardisaiton
Data standardisation plays a crucial role in establishing a unified format of data. Allowing for collaborative research, enabling large scale analysis, and promoting the sharing of advanced tools. The importance of this arises due to significant variations in healthcare data across different organisations. Data is collected for various purposes consequently, it can be stored in diverse formats, using different systems and information models. Despite the increasing use of standard terminologies in healthcare, identical concepts can be represented differently at different organisations.  

#### OMOP and the OHDSI standardised vocabularies
OHDSI developed the OMOP Common Data Model (CDM), which is a global standard for observational research. As part of the CDM, the OMOP Standardised Vocabularies serve two main purposes: they act as a common repository for all vocabularies used in the community, and they provide standardisation and mapping for use in research. The Standardised Vocabularies are freely available to the community and are mandatory for use as a reference table in OMOP CDM instances.
To build the Standardised Vocabularies, all vocabularies are consolidated into a common format, simplifying the researchers' work by eliminating the need to understand multiple formats and conventions. The OHDSI Vocabulary Team manages and updates the vocabularies regularly using the Pallas system. Researchers can access the Standardised Vocabularies from ATHENA, where they can select and download the vocabularies needed for their OMOP CDM. OHDSI prefers adopting existing vocabularies instead of building new ones due to their complexity and the existence of well-utilised vocabularies in the community. Concepts, representing the semantic notion of each clinical event in the OMOP CDM, are stored in the CONCEPT table, forming the foundation of the data records.

#### Converting into OMOP data model 
An Extract, Transform, and Load (ETL) approach is used to convert source data into the OMOP CDM.

#### Designing the ETL 
In the first stage of the process, both data experts and CDM experts work together to design the ETL. It helps to have prior experience in the implementation of ETLs to improve efficiency during this process, which requires an in-depth knowledge of  the source data. Softwares such as [WhiteRabbit](https://www.ohdsi.org/analytic-tools/whiterabbit-for-etl-design/) and [Rabbit-in-a-Hat](https://ohdsi.github.io/WhiteRabbit/RabbitInAHat.html) can be used during the ETL design stage.

WhiteRabbit creates a scan of the source data and creates a report which includes:
- a list of tables in the source database 
- a list of fields per table
- a list of distinct values found in a field,
- the frequency at which a value occurs

This report gives you a good idea of the general structure of the source data and can help with mapping of the data later on. The Rabbit-in-a-Hat software shows both the source data and the CDM. This is useful during the data mapping process as it shows how tables interlink.

##### Creating the Code Mappings
For the next stage of the process, people with medical and clinical coding knowledge will help create the code mappings. There is often a use of standard vocabularies such as the OHDSI vocabularies, RxNorm, ICD, and SNOMED. Data mapping is a big task and can be complex depending on the original source data format and quality. To make the process easier, it is best to focus on the most frequently used codes and either (1) exclude or (2) group codes which come up less often i.e., due to their relatively limited individual significance.

##### Implementing the ETL Design 
After receiving the design of the ETL with the complete code mappings, a technical person can use this information to implement the ETL via a coding language such as Java. 

##### Quality Control 
Finally, quality control is essential, especially in a medical context, therefore everyone is involved in ensuring there is good [data quality control](https://ohdsi.github.io/TheBookOfOhdsi/DataQuality.html#data-quality-in-general) throughout the design process. Tools such as [Achilles](https://ohdsi.github.io/TheBookOfOhdsi/DataQuality.html#achillesInPractice) are useful for spotting abnormal data inputs and data distributions and hence alerting the designers of data quality issues.

#### The potential of OMOP within the NHS
OMOP has the potential to revolutionise decision making and healthcare research within the NHS. It would facilitate the standardisation of healthcare data providing a unified data model that allows all healthcare data sources within the NHS to be accumulated and mapped onto a common format. This will enable researchers to analyse and compare data from multiple sources with more ease and on a larger scale leading to valuable insights being made to inform clinical decision making, drive evidence-based policies as well as allowing for a more collaborative style of research within the NHS. Secondly, the standardisation of data will increase data quality and data sharing capabilities, laying the foundations for a robust healthcare system.

In addition, OMOP could be used within the NHS to create large scale patient databases with real-time treatment patterns and outcomes. OMOP's data analytics capabilities also enable the identification of patient subgroups based on shared characteristics, such as genetic predispositions or response patterns to treatments. This stratification can help identify patient populations who are more likely to benefit from specific therapies, allowing for more personalised and effective healthcare approaches.

#### The benefits of OMOP over other CDMs 
OMOP provides a standardised, open-source data model that allows for the integration of diverse healthcare data sources. This standardisation ensures that data from various systems, institutions, and countries can be easily mapped and harmonised, promoting interoperability. Common data models often lack this level of standardisation, leading to challenges when attempting to combine data from different sources. Whereas, whilst some common data models support large-scale analytics, they may not be specifically tailored for observational research. This limitation can restrict researchers from conducting population-level studies efficiently and may require additional efforts to achieve comparable results
 
#### Adoption and Implementation of OMOP
- Larger healthcare companies often have significant investments in their existing proprietary systems, data formats, and medical devices. Adopting OMOP or any other standardised data model would require significant resources and efforts for data transformation, staff training, and system updates. They may resist these changes due to the perceived costs and efforts involved.
- Big healthcare organisations might be concerned about losing control over their data if they adopt a standardised data model like OMOP. Proprietary data formats may provide them with more control over how data is structured, stored, and accessed, whereas a standardised model could limit their autonomy over data management.
- Big healthcare organisations often operate on complex and diverse IT systems, and switching to a new data model like OMOP might create compatibility and integration challenges. They may fear disruptions to their existing workflows and operations during the transition.
