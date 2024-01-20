# HAN 462 Health Information Systems

### Course description: 
The HAN-462 curriculum covers a  range of topics related to health information systems (HIS). Starting with the foundational concepts and  operational landscape of the most common types of HIS. The course addresses the Software Development Life Cycle (SDLC) in healthcare, data requirements and standards, process capture in healthcare workflows, and the various types and roles of coding languages and database management solutions found within most HIS. Advanced topics include cloud computing, security, interoperability, and the application and adoption of artificial intelligence in HIS.

### Learning objectives: 
1. Identify and Explain HIS Core Concepts: Distinguish between various types of health information systems and their roles within the healthcare landscape, utilizing foundational knowledge in HIS, HIM, HIMS, HCIS, and HCIT.

2. SDLC in Healthcare: Understand and articulate the stages of the Software Development Life Cycle (SDLC) as they apply to healthcare, comparing traditional and modern methodologies such as Waterfall, Agile, Scrum, and Kanban.

3. Evaluate Data Management Tooling in HIS: Identify the types and sources of data in healthcare, apply coding standards like ICD and CPT, and assess the implications of data management practices within health informatics.

4. Map and Optimize Healthcare Workflows: Demonstrate the ability to capture, model, and analyze healthcare processes, utilizing techniques such as flowcharts, swimlanes, and process mining to improve efficiency and patient care.

5.  Coding Languages and Database Management: Evaluate the use of different coding languages and database solutions in HIS, understanding their application in the development and maintenance of health information systems.

6. Security and Interoperability Standards: Assess the importance of security frameworks and regulatory requirements in HIS, and develop strategies for achieving interoperability between disparate healthcare systems.

7. AI and Cloud Computing in HIS: Examine the role of artificial intelligence and cloud computing in healthcare, exploring how these technologies can be harnessed to enhance HIS functionality and patient outcomes.

### Additional resources: 

Cool open source books:
- Reference book 1: Simple - Data: https://www.ncbi.nlm.nih.gov/books/NBK543527/ 
- Reference book 2: Analytics - Examples: https://www.ncbi.nlm.nih.gov/books/NBK543630/
- Reference book 3: Bio - Complex: https://www.ncbi.nlm.nih.gov/books/NBK569562/ 
- Reference book 4: Simple Overall - https://omicstutorials.com/introduction-to-health-informatics-a-comprehensive-course-for-biologists/ 

## 1. Intro Day 
- Who I am 
    - Hants Williams: Nurse, Data Engineer, etc...
    - Recent projects 
        - SDoH resources v1 - external community (https://inclusion.appliedhealthinformatics.com/)
        - SDoH resources v2 - internal SBM (https://sdoh.ahi-projects.com/)
        - Data discovery tool - external (https://discover.appliedhealthinformatics.com/)
    - You are now t-minutes 4 months till graduation; on average it can take on average 3-6 months
        - Average: link [https://www.washington.edu/doit/what-can-students-do-improve-their-chances-finding-employment-after-college#:~:text=The%20fact%20is%20that%20approximately,to%20secure%20employment%20after%20graduation]
        - Average means average...it could be a month, or it could be 9 months
        - Hospitals usuaully open up positions, and keep them open for a month or two and then close, then spend rank order them, do interviews - few weeks later (month or two) - perhaps looking at a 3-4 month period on average for application opening to someone filling the position 
    - Masters program: AHI, 15 month program - still accepting applications for Summer 2024
- Basic definitions - HIS / HIM / HIMS / HCIS / HCIT / HCIS / HCIT
    - AMIA def of Health Informatics: the science of how to use data, information and knowledge to improve human health and the delivery of healthcare services 
    - AMIA def of HIM: the practice of acquiring, analyzing, and protecting digital and traditional medical information; it is a combination of business, science, and information technology; 
    - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8649705/ 
- Opearting Landscape for Health Care/Information Management Systems: 
    - Hospitals
    - Insurance (payers)
    - Consulting
    - Pharma(biotech)
    - Tech/Vendors
- Health Information Systems Components and Department Sub-systems // Types of software systems and services: [https://www.beckershospitalreview.com/finance/the-31-best-rcm-tools-per-klas.html]
    - Medical and Health Records (EMR, EHR) - Epic, Cerner 
    - Patient Portals (PHR) - MyChart, MyHealth, etc. (typically tied to EMR/EHR)
    - Patient Monitoring (RPM) - 
    - Customer Engagement (CRMs) - 
    - Planning, Management, Oprations (ERPs, PMS) - ERPs: SalesForce, Yext, Hubspot, Oracle, SAP; PMS: Athena, Practice Fusion, Kareo (note - PMS usually smaller versions of EMR for independent/small practices)
    - Medications, Pharmacy, Prescribing (E-prescribing, PBMs, Pyxis) - Eprescribe: surescripts, FDB-vela; 
    - Labs (LIS) - Sunquest (Clinisys), Cerner [https://www.sciencedirect.com/topics/medicine-and-dentistry/laboratory-information-system]
    - Scheduling, Patient - Phreesia, Yosi 
    - Scheduling, Staff - QGenda Nurse and Staff Scheduling
    - Credentialing - ASM MD-Staff
    - Imaging (RIS, PACS) - Sectra, Carestream, Merge Healthcare (IBM), McKesson, GE, Philips, Siemens
    - Billing and Revenue (RCM) - RCM: Revecore, Epic Resolute Hospital Billing, RSi RCM (Debt Collection) 
    - Claims/Insurance (UM, CDSS) - Experian Health ClaimSource,
    - Supply Chain/Medical Equipement: SAP, Oracle, Mkesson, Securitas Healthcare MobileView (hardware and software);
    - Clinical Trials (CROs): IQVIA, Parexel, LabCorp
    - Analytics and Reporting: Tableau, PowerBI 
- Current challenges of HIS (Current challenges in health information technology–related patient safety) 
    - Design and Development challenges
        1. Developing models, methods, and tools to enable risk assessment
        2. Developing standard user interface design features and functions
        3. Ensuring the safety of software in an interfaced, network-enabled clinical environment
        4. Implementing a method for unambiguous patient identification
    - Implementation and Use challenges
        5. Developing and implementing decision support which improves safety
        6. Identifying practices to safely manage IT system transitions
    - Monitoring, Evaluation, and Optimization challenges
        7. Developing real-time methods to enable automated surveillance and monitoring of system
        performance and safety
        8. Establishing the cultural and legal framework/safe harbor to allow sharing information about hazards
        and adverse events
        9. Developing models and methods for consumers/patients to improve Health IT safety
- Important term: Technology stack (front-end, back-end, database, etc.) - https://stackshare.io/stacks 
- Important deciding factor: When dev/selecting systems - depend on environment - deliver modalities (async, sync; in-person, remote) 
- Multiple Roles Supported by Health Information Systems (CIO, CTO, CMIO, CNIO, CISO, CDO, etc.)
- Other roles that you will likely be if you go into the field: https://blog.appliedhealthinformatics.com/posts/job-titles-informaticists 

## 2. SDLC for Health System 
- SDLC 
    - Plan
    - Analysis
    - Design 
    - Implement & Test (Article on Production Testing)
    - Evaluate & Support 
- Executing with: 
    - Waterfall vs Agile
    - Scrum vs Kanban
    - Lean/6 Sigma
- Communication breakdowns lead to failures (nurses and IT dept article)
- Example of NLP rollout by VA with SDLC framework (PPT from VA)
- SAFER deployment framework for EMR rollout 

## 3. Data Requirements for Systems  
- Data Types 
    - Structured
    - Unstructured
    - Semistructured
- Common Data sources 
    - EMR 
    - Claims 
    - PBMs 
    - Patient apps / wearables
- Data Codes (ICD, CPT, SNOMED, DIACOM, LOINC, etc.)
- Data Models
    - HL7
    - FHIR 
    - FAIR 
- Big Data Challenges (article)
    - The four Vs 
    - Types (omics, vitals, labs, imaging)
    - Privacy, incompletness, heterogenity 
- Where to find data 
    - data.gov
    - healthdata.gov
    - AHRQ 

## 4. Process Capture / Workflows
- General (article: Health care process modelling: which method when?)
    - Stakeholder 
    - Information 
    - Process
    - Flowcharts
    - Swimlanes 
    - State transition
    - Communication 
    - Data Flow
- Processing Mining Framework 
    - Article: Process mining framework with time perspective for understanding acute care: a case study of AIS in hospitals
- Care Pathways 
    - BPMN (Business Process Modeling Notation)
    - CMMN (Case Management Model and Notation)
    - DMN (Decision Modeling Notation) 
    - Care Pathways 
        - Sharable Care Pathways (article) 
- Problems with BPMN 
    - Article/Perspective: Why BPMN doesn’t work for healthcare
- Example - ICU 
    - Article: Workflow Modeling in Critical Care: Piecing your own Puzzle.
    - Criticle Zones 
    - Cognitive Workflow Model 
- Examples (article: Module 10 mapping): 
    - Fig 10.2: PA Office Visit 
    - 1b: Lab result followup 
    - 2a: Rx fills (bad)
    - 2b: Rx fills (good)
- Examples - Telehealth Workflow 
    - Article: Planning your telehealth workflow
- Example - eHealth Implementation 
    - Article: Using a Clinical Workflow Analysis to Enhance eHealth Implementation Planning: Tutorial and Case Study
    - Case study technology: Protect Me 4 / use by parents of adolescents at the beginning of their child’s appointment to help parents learn about recommended vaccines and explore educational information addressing common hesitations
    - Steps: 
        - Identification discrete steps 
        - Workflow assessment 
        - Triangulation 
        - Stakeholder proposal 

## 5. Coding Languages 
- Should expand this section to include a summary of different types of coding languages, coding environments (on your device versus the cloud), types of roles 
    - C++, Javascript, Go, Python, R, SQL, etc.
    - Different languages uses do different things better/worse - depends on what you need 
        - E.g., mobile first: swift, C#, kotlin, react native, flutter, etc.
        - E.g., web first: javascript, python  
        - E.g., desktop first: C++, Java 
    - Online article - bytebytego // how the common ones (C++, Java, Python) work [https://www.linkedin.com/posts/alexxubyte_systemdesign-activity-7154146888085106688-MarG?utm_source=share&utm_medium=member_ios] 
- Python in healthcare companies (article: BELITSOFT)
    - Roam Analytics - Ai platform - web frameworks
    - AiCure - medication tracking - web frameworks 
    - DrChrono - EMR - API development
    - Qventus - predictive Ai - API, Ai, web framework 
    - Sempre - PBM - API dev, Ai 
    - Fathom Health - unstructured notes - Ai 
- Python in healthcare examples (article: TECHVIDVAN)
    - Analysis: medical images 
    - Analysis: medical records
    - Drug Discovery and Development 
    - Omic Research and analysis 
    - NLP for clinical notes 
- Python
    - Python Basics
    - Python for Data Science
    - Python for Web Development
    - Python for Machine Learning

## 6. Saving Data: DBMS for Systems 
- How data is stored: databases, data warehouses, data lakes, blob storage; 
- Data Modeling for databases: (ERD, UML)
- Relational
    - SQL (MySQL, PostgreSQL) 
    - Common tools: MySQL Workbench, pgAdmin
    - Common cloud: AWS RDS, Azure SQL, GCP Cloud SQL
    - Try it: mysql client/db: [https://shell.cloud.google.com]
- Non-Relational
    - NoSQL (MongoDB, Cassandra, etc.)
    - Common tools: MongoDB Compass
    - Common cloud: AWS DynamoDB, Azure CosmosDB, GCP Cloud Datastore
    - Try it: mongo client/db: [https://atlas.mongodb.com]
- Future / Other: 
    - Graph 
    - Blockchain
    - Federated
    - Vector
    - In-memory

---

## 7. Midterm
## 8. Break
## 9. Microsoft Power Automate
- Power Automate
- Power Apps
- Power BI
## 10. Security Requirements for Systems 
- Regulatory Frameworks (HIPAA, HITECH, etc.)
- Security Frameworks (NIST, HITRUST, etc.)
- Security Controls (NIST 800-53, etc.)
- Security Operations (SOC, SIEM, etc.)
- Ideas from AMIA [https://amia.org/education-events/education-catalog/amia-health-informatics-essentials-health-information-systems]: 
    - Security, Privacy, and Confidentiality Regulations - HIPAA
    - Data Security Standards, Threat Identification and Mitigation Strategies
    - User Types and Roles for Access Control
    - Health Information Communication Channels
## 11. Interoperability (HIEs, TEFCA) Requirements for Systems 
- Frameworks (HL7, FHIR, etc.)
- Standards (CCD, CDA, etc.)
- APIs (SMART, etc.)
- HIEs (CommonWell, Carequality, etc.)
- TEFCA
- Ideas from AMIA [https://amia.org/education-events/education-catalog/amia-health-informatics-essentials-health-information-systems]: 
    - The Need for Interoperability
    - Seven Layers of Interoperability Architecture
    - Health Data Exchange Standards
    - Terminology Standards
    - Health Information Exchanges
    - Health Information Exchanges, Data Aggregation and Population Health
## 12. Cloud Computing (AWS, Azure, GCP) for Systems 
- Cloud providers (AWS, Azure, GCP, etc.)
- Types (IaaS, PaaS, SaaS, etc.)
- Core services (compute, storage, databases, networking, etc.)
- Healthcare related services in Azure (Azure API for FHIR, etc.), GCP (Cloud Healthcare API, etc.), AWS (Amazon HealthLake, etc.)
## 13. Ai (CDSS, LLMs, NLP, CV, etc.) for Systems 
- Machine Learning (supervised, unsupervised, reinforcement, etc.)
- Deep Learning (CNN, RNN, etc.)
- Natural Language Processing (NLP)
- Computer Vision (CV)
- Clinical Decision Support Systems (CDSS)
## 14. Review
## 15. Final 



| Week | Date          | Topic                                              |
|------|---------------|----------------------------------------------------|
| 1    | January 23    | (Intro) Introduction to Health Information Systems         |
| 2    | January 30    | (SDLC) Systems Development Life Cycle (SDLC) in Healthcare|
| 3    | February 6    | (DATA) Data Types and Modeling in Healthcare              |
| 4    | February 13   | (PROCESSES) Process and Workflow Modeling in Healthcare Settings|
| 5    | February 20   | (PROGRAMMING) Programing Languages for Healthcare Applications|
| 6    | February 27   | (DMBS) Database Management with MySQL in Health Information Systems|
| 7    | March 5       | Midterm                                            |
| 8    | March 12      | Spring Break (no class)                            |
| 9    | March 19      | (MICROSOFT POWER) Developing Custom Healthcare Applications with Power: Automate, Pages, and Apps|
| 10    | March 26      | (SECOPS) Security, Privacy, and Compliance in Healthcare IT |
| 11   | April 2       | (INTEROP) Interoperability and Health Information Exchanges (HIEs)|
| 12   | April 9       | (AI) Artificial Intelligence and CDSS                   |
| 13   | April 16      | (CLOUD) Cloud Computing for Healthcare                     |
| 14   | April 23      | Review                                             |
| 15   | May 7         | Final                                              |