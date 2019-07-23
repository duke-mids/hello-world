# Hello World Project Scope

Department of Surgery MIDS capstone project is as follows:  

# Background/Problem	
The Department of Surgery is one of the leading surgery programs in the world, committed to Duke Health's mission of providing outstanding and compassionate patient care, training tomorrow's leaders, and conducting innovative research. Two projects of focus for the MIDS Capstone Project include 1) optimizing block time and contingency responses in the OR, improving flow of patients through the hospital and more intelligent use of inpatient beds and 2) creating a Value Based Care model grouping OR case costs w/ surgical outcomes data, such as National Surgery Quality Improvement Program (NSQIP) data.

## Project 1:  OR Case Time Accuracy
Across Duke University Health System (DUHS) operating room blocks are completely allocated across all platforms, patient census is typically at 98% or greater, and the emergency departments are overflowing.  Given that additional capital infrastructure is not a viable option, the Department of Surgery wants to determine the best way to allocate its scarce resources.  The ability to predict actual case length and automate operating room scheduling will allow the department to optimize operating rooms and better sequence cases to manage patient flow throughout the hospital. 

Duke’s existing surgery scheduling process is highly variable.  Each type of surgery is assumed to require some standard amount of time in the operating room. The surgery team hypothesizes potentially confounding variables like patient comorbidities, seniority of surgeon, time of day, and time of year should be taken into account.  In some cases, a surgeon provides his/her own estimate of how long a surgery will last, which is also taken into consideration.  Lack of defined scheduling inputs for the surgeons and OR schedulers in the current scheduling process generates highly inconsistent and inefficient operating room usage (with frequent gaps and/or delays).  This is a suboptimal outcome, because more accurate surgery estimates and scheduling could better utilize surgeons’ time and improve patient flow throughout the hospital.  

### Approach/Goals  
The Capstone team will combine data about the type of surgery being performed from billed CPT codes with time stamps associated with operation room preparation, anesthesia, the surgery itself, and post-op to predict actual surgery durations. To do this, the team will:
•	Collaborate with various surgical specialties within Duke Surgery to discuss the current scheduling process, available data affecting actual surgery times that should be considered for predictions, and appropriate methods for segmenting procedure codes.
•	Combine, prepare, and clean any relevant data
•	Create data visualizations and use descriptive statistics to “tell the story” of what factors currently impact surgical lengths
Based on what they learn from these initial steps, the Capstone team will then create an algorithm that generates surgery schedules that more closely align with the actual lengths of surgeries, including the ability to estimate what surgical trays may be required for a given procedure based on the likely CPT codes for the procedure. To do this, the team will need to work with relevant stakeholders in the Department of Surgery and Epic analysts to “roll out” preference card changes with likely success and minimal disruption.  Some of the approaches the team will try include:
•	Using all available data to predict how long each specific surgery will take
•	Incorporating historical medical data from individual patients to improve predictions about which surgeries are likely to have complications
•	Working with medical experts to identify variables that health care providers intuitively know influence surgery times, but that may not be reflected in the available data directly without additional computations
The Capstone team will then work with the DUHS data warehouse developer to productionize their algorithm so it is implemented in the day-to-day functioning of the department. 
Anticipated Deliverables
•	An initial interactive data visualization that allows the surgery team to explore variables that influence surgery times
•	A careful analysis of the pros/cons of different prediction and optimization approaches, and a methodical description of where each approach tends to be successful or unsuccessful
•	Implementation of the best prediction approach in The Department of Surgery’s scheduling system

## Project 2:  Value Based Care Project – Surgical Procedures
The health care landscape is moving from a fee-for-service model to a value based care model to aid in controlling the United States’ ballooning healthcare expenditures in relation to other comparable countries.  This shift will require health systems to better understand surgical costs (expenses) and associated outcomes.  Beginning in 2021, medical institutions across North Carolina will begin incurring financial penalties if the value of care being provided is not up to standard. As such, it is important for Duke Surgery to understand their performance now to begin work to overcome obstacles. These obstacles will include optimizing patient outcomes while minimizing surgical expenses and process variability.

### Approach/Goals:
The Capstone project will involve the combining of numerous large databases to identify a means of optimizing patient outcomes while minimizing hospital surgical expenses and process variability. The data sources will include Duke Surgery billing, Epic CPT tables, NSQIP outcomes data, vendor contracts, and electronic health records. Optimization methods may include linear programming or differential evolution, though other techniques will be researched to identify the appropriate means of convergence. To do this, the team will:
•	Combine, prepare, and clean any relevant data.
•	Create data visualizations and use descriptive statistics to explain variation across surgeons for the same surgical procedure
•	Use learnings from Project 1: Case Time Accuracy to incorporate variables that increase length of case and thus, cost of the case
•	Identify the CPT path that optimizes patient outcomes while minimizing hospital expenditures.
Anticipated deliverables: 
•	An interactive visualization tool to feed to a “Value Based Care Scorecard” for each surgeon for each respective surgical procedure. This visualization should implement the optimal path identified.
Description of Protected Data Set and other Data
Data that will be used in support of the project will include:
•	Basic case information (log ID, surgery date, location, room, provider, patient class etc.)
•	Timestamp (from patient in facility to patient out of recovery room)
•	CPT list (all the procedures related to the single case)
Estimated number of records and size:
~365,000 rows, 62 columns; 	~200MB
•	NSQIP outcomes data
•	Billing data
•	Vendor contract data

## Presentation of Deliverables
There will be two presentations throughout the project duration:
•	A midway project presentation will be held within the timeframe of 11/27/2019 – 12/16/2019 on a day agreed upon by the MIDS student team, key project stakeholders, project mentor and/or MIDS faculty. 
•	A final project presentation will be held within the timeframe of 4/16/2020 – 5/2/2020 on a day agreed upon by the MIDS student team, key project stakeholders, project mentor and/or MIDS faculty.
 A member from the Duke Surgery Team will agree to attend both of these presentations.
Allowable Reference to Project/Data Provider 
Duke personnel may use the following description of project/data provider: 

Students may name the client and give a broad project description (topic, type of work performed, deliverable provided).

## Data Hosting and Computational Environment
PACE

Data Transfer
	N/A

Data Provider Technical contact for data transfer and/or student support: 
Wendy Webster for administrative surgical operations support
Erich Huang for data science support related to surgery – biweekly for one hour
