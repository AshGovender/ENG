# Academic Qualifications
> * Bsc. Chemical Engineering (University of Kwazulu Natal)
> * Msc. Mechatronics Engineering (University of Kwazulu Natal)
> * Mediventors Integrated Skills Development Program (University of Cape Town)
>> * Medical Device Sector Essentials
>> * Systems Engineering and Product Lifecycle Management
>> * Tooling, Manufacturing and Industrialization

# Licenses and Certificates
> * Lean Six Sigma Greenbelt

# Courses
> * [Data Science Methadology (Coursera - IBM)] - [View Certificate](https://www.coursera.org/account/accomplishments/certificate/NXGZBLFKJ8QR)
> * Machine Learning With Python (Coursera - IBM) - [View Certificate](https://www.coursera.org/account/accomplishments/certificate/VZTZQQPXC4SB))
> * Lean Six Sigma Yellow Belt (2014) – Dow Chemicals
> * Other Internal Company Courses (CAPA Work Process Overview, Common Improvement Tools, Exposure to Hazardous Chemicals, Reactive Chemical Training, Fault Tree > > * Analysis, Ergonomic Awareness Training, ISO 14001 Understanding, Root Cause Analysis, Paint Technology, Diversity and Inclusion, Lean Basics (2013-2014)
> * Pressure Vessel and Tank Design (2017) – Engineers for Africa
> * Chemical Risk Assessment Masterclass (2022) – Sedulitis
> * Investigate and Intiate Hearings (2022) - Global Business Solutions
> * Occupational Health and Safety Act Workshop (2022) - Bosman Attorneys

<br />

# Project 1: Backorder Reduction Using DMAIC Methadology

![](/assets/img/Back.PNG)

## Problem Statement
Backorders at a paint company was resulting in 50 million rands loss of revenue. This was also resulting in poor customer satisfaction and poor service levels. With impending market share competition, this needs to be resolved to ensure mainteanance and further entry into the market.

## Task/Action
As part of my positions as process engineer, I worked with the head of supply chain as project lead to employ the DMAIC methadology to reduce backorders through identification and mitigation of pertinent issues. The tools below were used:

* Define: developed project charter, benefits analysis, Pareto analysis to identify focus area, high level process map, VOC, CTQ's, Metrics Tracking, tollgate review
* Measure: Detailed swimlane, SIPOC analysis, Gemba walks, 8 waste identification, Value stream mapping, Spaghetti diagram, MSA and capability analysis, tollgate review
* Analysze: Potential X's(Fish bone diagram), XY diagram (vital few X's), Root cause analysis, graphical and statistical analysis,hypothesis testing, FMEA development
* Improve: 5s and flow implementation, Kanban development, Correlation and regression, Pilot testing, Solution development using thinking methods and implementation
* Control: Mistake proofing, Visual management controls, Statistical Process Control, updating of SOP's, Control Plans, Training and handover, tollgate review

## Data Sources
Backorder reports, Sales Reports (Qlikview and SAP)

## Results 
The backorder investigation identified various reasons for backorders across the value chain. This included issues with forecasting and sales, as well as production related issues for certain process streams, stock health issues, lead time issues, production complexities. Mitigation measures were put in place such as capacity and manpower increases in certain sections, forecast accuracy improvements, re-adjustment of stock health monitoring tool zones, lead time adjustments, recipe formulation changes and product cycle time improvements. Overall loss of sales revenue reduces by 15% compared to the benchmark year and ultimately increased capacity in pivotal process streams.

## Python libraries
PyPI(pymsavis) for MSA ,scipy(stats) for capability analysis & hypothesis testing & SPC, matplotlib, seaborne, Pandas, Numpy etc.

## Data Analytics Methods
Text cleaning, exploratory data analysis, hypothesis testing, MSA, statistical and graphical analysis

<br />
<br />

# Project 2: Boiler Optimization and Environmental Compliance

![](/assets/img/Boiler.PNG)

## Problem Statement
The boiler at Kansai plascon was not adhering to environmental compliance in terms of particulate matter and sulphur dioxide fumes. This was resulting in fines and other prosecutions on site until compliance could be achieved. In addition, the boiler was operating inefficiently resulting in an increase of operating cost.

## Understanding the chemical engineering processes:
>* Optimizing the air fuel ratio - mimimizes excess air which increases efficiency by reducing heat loss throught the flu gas. Excess air absorbs more heat, too little air results in incomplete combustion, reducing efficiency and increasing pollutants (PPM) and resulting in soot build up. 
>* Reduce flu gas temperature - need to be hot enough to prevent condensation of acids but low enough to prevent excessive heat loss
>* This can be automated with control systems for controlling air and fuel supply (also saving fuel costs)
>* Prior to this tuning of the burner can be done - for optimal combustion while reducing PPM emissions
>* To recover heat: can ensure optimal condensate recovery (stream traps working well, condensate sending water to make-up water tanks), installation of economizers to re-use heat from waste gas to heat make-up water
>* Adjusting fuel source - effect on calorific value. Cleaner fuel has lower sulphur dioxide (good for emission reduction) but more expensive. Need balance.
>* heat loss minimization: repair leaks in steam system, use insulation on piping
>* the same logic of heat transfer as cooling towers applies. The heat load is how much steam is required by the process and boiler capacity is what the boiler can supply: difference will be in the values of heat transfer coefficient and the actual temperature vs idealized conditons for the heat load requirement:

![image](https://github.com/user-attachments/assets/ac940011-2357-4c92-a1be-2bd0d1d1694b)

![image](https://github.com/user-attachments/assets/ed6ff132-8362-4bfa-b791-7c1861143b21)

 ![image](https://github.com/user-attachments/assets/a7610ff7-4aea-412c-aee1-71ce7cfcd709)

![image](https://github.com/user-attachments/assets/a61e7104-f50a-447c-9015-09e5bdbaacc9)

>* At the same time boiler heat transfer rate is important (UAdeltTLm) - this need to be sufficient enough to achieve the boiler capacity requirements

![image](https://github.com/user-attachments/assets/c46a0fcb-7ed8-4f70-ac59-a618e77cdaff)


>* Increasing boiler water flowrate increases heat transfer rate but reduces boiler capacity as less water is going throught the boiler - however a balance between these two are required
>* Important to note that flow patterns affect the overall heat transfer coefficient. You can determine if flow is laminar or turbulent using Reynolds number and then determine the value of U accordingly, as shown below:

![image](https://github.com/user-attachments/assets/8d339158-b27c-4550-9227-43bd971aa4d9)

![image](https://github.com/user-attachments/assets/074c92bd-782f-4dce-987e-18f7feaf3a4e)

![image](https://github.com/user-attachments/assets/312fbcf8-8cc4-4530-837c-d61f7c869af3)

>* Higher flowrate results in turbulent flow which increaseses the temperature gradient at the surface due to more mixing
>* Lower flowrate results in laminar flow - howevere due to increase in resonance time can increase heat transfer coefficient in a laminar state
>* the choice between laminar and turbulent flow will depend on application. With laminar flow preferred when flow patterns need to be more uniform, less erosion and wear is required and lower energy
>* We can also increase the heat transfer area as seen by the equation to improve the heat transfer rate. This can be done by ensuring proper blowdown or ensuring proper chemical treatment to prevent scaling
>* Ensure water treatment is working effectively - to prevent scaling and corrosion. Monitor PH, dissolved solids and alkalinity of boiler water regularly
>* the optimum blowdown rate can be given by:

![image](https://github.com/user-attachments/assets/9f49e522-0c6b-498a-8df6-89504da90a45)

>* The overall boiler efficiency can be given by - which is different from cooling towers:

![image](https://github.com/user-attachments/assets/b8bc41d8-47c1-4497-832f-d9684c60d8dd)

![image](https://github.com/user-attachments/assets/3694f7ac-5d0a-4329-aa2b-4356d1a877e7)

>* this can be decomposed into the equation below; using this decomposition, you can identify whether improvements need to be made in the combustion process (e.g., adjusting air-fuel ratio), heat transfer (e.g., cleaning heat exchangers), or load management (e.g., operating the boiler closer to its design capacity).

![image](https://github.com/user-attachments/assets/cb6db5ad-671d-4216-80df-f6e03b7f390f)

>* the mass balance equation across the boiler is given by:

![image](https://github.com/user-attachments/assets/8fe40089-1d5f-4e9a-a4a7-82fe3e3fad8e)

>* the energy balance equation across the boiler is given by:

![image](https://github.com/user-attachments/assets/033a6e64-c911-413b-832d-e96fda88ee45)

![image](https://github.com/user-attachments/assets/468cbe77-83c7-4338-8ad2-012036dcd60f)

>* for saturated and superheated steam the terms for vaporization and superheated steam must be added:

![image](https://github.com/user-attachments/assets/a3af5968-40d6-4803-a416-74a25bd277e9)

>* the temperature of steam can be given by:

![image](https://github.com/user-attachments/assets/8516df9f-e3ef-4150-a926-a86da257514b)


## What can typically go wrong in a fire tube boiler:
>* Fouling and scaling (due to inadequate water treatment or blowdown)
>* Water levels too low (leading to tube exposes to excess heat - resulting in tube rupturing or boiler blowing up)
>* Corrosion on boiler internals due to water quality and inadequate treatment
>* Soot accumulation of fire tube surfaces affecting heat transfer (due to incorrect air/fuel ratio)
>* Pressure build up as a result of pressure safety valves not working effectively
>* Inadequate airflow resulting in incomplete combustion
>* Excessive airflow leading to excess heat loss and PPM levels exceeding legislative requirements
>* Thermals stresses on fire tubes as a result of sudden temperature changes e.g. feed water temp
>* water quality or water carry over issues e.g. incorrect steam traps/seperation equipment
>* High pressure can increase the saturation temperature of steam



## Task/Action
My role as process engineer was to assist the SHERQ department in not only ensuring adherence to environmental regulations but also to improve efficiencies in the boiler to reduce cost. The following was achieved:

> * Walked the process and developed a P&ID representing the system
> * Developed a mass balance to account for water and steam losses
> * Identified and mitigated issues for loss of steam (steam survey), loss of condensate, increase fuel usage, particulate matter and sulphur dioxide increases
> * Developed a comprehensive report back to management for changes to be complete
> * Carried out implementations
> * Improvement of risk assessments, FMEA
> * SOP modifications
> * Improvement of plant maintenance schedules
> * Carried out steam and energy calculations
> * Installed new measurement devices and carried out a guage R&R study to ensure reliability of measurement system

Key implementations:
> * Re-designed maintenance schedules to reduce fowling in the boiler and improve chemical treatment to improve heat transfer and reduce fuel usage
> * Identified condensate losses which resulted in wastage of heat and treatment chemicals through steam trap damage and incorrect condensate recovery control logic
> * Ensured air/fuel ratio was corrected which fixed the particulate matter issue
> * did a cost benefit analysis and implemented a new fuel changeover from HFO to LFO that resulted in sulphur dioxide emissions compliance without a significant capex and operating cost
> * Led the installation of an autoflam unit which ensured optimized air fuel ratio and reduced fuel usage
> * Led the correction of the steam control system which ensured optimum maintenance of feedwater to the boiler reducing the amount of fuel required to heat the water to saturated steam
> * All steam trap and leaking lines were fixed resulting in optimum condensate recovery as well as steam
> * Carried out various engineering calculations to quanitify and identify cost savings and benefits analysis

## Data Sources
Operational reports, meter readings, operator reports

## Software libraries
Excel was utilized for all calculations, Visio for P&ID

## Data Analytics Methods
Statistical and graphical analysis, mass and energy balances

<br />
<br />

# Project 3: Maintenance System Upgrade

![](/assets/img/Maintenance.PNG)

## Problem Statement
The maintenance system at Kansai Plason was suffering from several operational issues that were resulting increased downtimes and lack of traceability. Upon further investigation it was found that the planned maintenance system was not working effectively and there was no maintenance reporting tool that was available to identify an mitigate maintenance related job card issues. 

## Task/Action
My role as process engineer was to assist the maintenance department by redesigning the planned mainteance system as well as developing a reporting tool that would allow for transparency within the maintenance department. The following was done:

PM Restructure: 
> * Reviewed maintenance process and SAP structure with MES engineer and TL
> * Developed "As is Process" flow with gaps
> * Developed "To be" process flow
> * Developed  "Future state" process flow
> * Developed and reviewed final process flow with stakeholders and developed an action list
> * Extracted information from SAP transaction showing PM's over the last few years and created an Excel based databack showing gaps in data structure
> * Developed an equipment KPI tree to determine resources on site
> * Developed and utilized an equipment frequency matrix to determine gaps in PM alerts and to reassign frequencies based on legal and operational requirements, remove redundant PM activities and include missing PM's based on all equipment identified
> * Worked with MES engineer to redesign and install functional locations based on site plan and SAP rules
> * Created and Excel based control document for PM Checksheets, PM's and functional locations that would work in tandem with SAP to streamline planned maintenance activities
>* worked with team to carry out detailed analysis of PM tasks for each checksheet (required indepth plant study of exactly what maintenance would be required for each piece of equipment based on OHSA and operational requirements for various frequencies)
>* Installed new equipment, PM's onto SAP
> * Training and SOP modification

Maintenance Analytics:
> * Identified SAP sources of maintenance info and generated a draft visual dashboard of key KPI's
> * Reviewed changes and ammended with key stakeholders
> * Trial tool and made ammendments
> * Creation of final dashboard
> * Created and enforce correct data entry on SAP with mistake proofing
> * Training and handover

Key Implementations:
> * Developed a maintenance reporting tool which was capable of identifying job card related information such as overdue job cards, employee utilization, scheduled vs unscheduled maintenance, employee utilization, sections and equipment with the most breakdowns etc. This tool helped with cost savings and job card closure rate
> * Re-designed the planned maintenance system which effectively reduced plant downtimes through effective scheduled maintenance 

## Data Sources
SAP

## Software libraries
Excel for development of maintenance reporting tool, Visio for flowcharts, SAP for system integration

## Data Analytics Methods
Data visualization

<br />
<br />

# Project 4: Planned Adherence Optimization Using Lean Six Sigma Approach

![](/assets/img/PA.PNG)

## Problem Statement
The planned adherence within the Johannesburg and DBN site of Kansai Plascon was poor and lacked a common measurement tool to account for the complexities within scheduling and planning.

## Task/Action
My role as process engineer was to assist the head of supply chain with streamlining and addressing issues with the entire value chain to effectively identify and mitigate issues with the poor plan adherence. As part of this iniative, I developed a tool to measure planned adherence and schedule adherence separately while also considering batches that were pushed forwards or backwards. The following was done:

>* had a massive brown paper session in both the JHB and DBN sites including all stakeholders across the value chain: manufacturing, filling, maintenance, raw materials, procurement, supply chain, MRP, planning and scheduling and factory technical - this was to identify the current state, brainstorm gaps and develop a future state and develop a plan of action based on findings
>* Worked with team to action plans to improve planned adherence through strategic projects at each department
>* Developed a measuring tool for planned and schedule adherence and benchmarked across both sites - this highlighted a critical finding that schedule adherence was not the issue but rather planned adherence as opposed to prior beliefs
>* Communicated findings to director of operations

Key Implementations:
>* Standardization of planned adherence measure
>* Finite planning (including re-order level management of INT's, MPS with frozen reliable planned elements)
>* Scheduling optimization (backward scheduling, scheduling based on constraints, factoring re-work times, Heijunkai, develop buffer for raws)
>* QC projects (stricter rejection policies, establishment of escalation protocol for long adjustment times, calculation of exact quantity of packaging required, establishing scap rates for adjustment material, different recipe versions on SAP,prediction around first adjustments)
>* Procurement projects (assign packaging to batches and reconcile)
>* Labelling (trigger points for labelling)
>* Inspection of QI system fails
>* Manufacturing issues (improve nossil inefficiencies, improve lead time for grind batches, improve expediting with online tools, reduce expired raws on site, run plant in full auto)
>* Physical validations before sign-off
>* fix of master data to align schedule time with product lead time

## Data Sources
SAP, SAP(MII), Qlikview

## Software libraries
Excel for development of reporting tool, Visio for flowcharts

<br />
<br />

# Project 5: Solvent Recycling Plant Optimization

![](/assets/img/Solvent.PNG)

## Problem Statement
The solvent recycling plant at kansai plascon was not producing the desired recovery quality of solvent. This was resulting in more money being spent on buying virgin solvent. In addition to this, operators complained that the fumes released by the system was not in compliance

## Task/Action
My role as process engineer was to investigate and resolve environmental compliance issues as well as improve the efficiency of the system. A mass balance was carried out on the system as well as a kaizen walk. The tool showed that recovery rate was poor because the upstream processes were sending through much more dirtier solvent compared to the past, the settling tanks were not working which means heavier solids were not separated and lastly the handling mechanism for dirty solvent was no longer active. This coupled with the fact that the solvent recyclers were not optimized in terms of settings. 

Key implementations:
> through trials optimum setting were established
> Re-commissioning and maintenance of the settling tanks significantly improved pre-treatment reducing the strain on solvent recycling machines
> Upstream processes were instructed to not use solvent on too many runs of cleaning to reduce the dirtiness of the solvent
> Maintenance assisted with fixing the handling mechanism for the solvent recyclers

## Results
All the above actions were addressed which increased the solvent recovery reclaimation rate by 30%. A future study was then done to utilize unoccupied reactor to carry out solvent recycling which completely eliminated the need for virgin solvent purchasing and drastically reduced the cost of solvent recyling.

## Data Sources
Plant meters

## Software libraries
Excel 

<br />
<br />

# Project 6: Lead Time Reduction Using Lean Six Sigma & Theory of Constraints

![](/assets/img/Cycle2.PNG)

## Problem Statement
Cycle times for the Durban and Johannesburg plants were too high - this was resulting in an increased in backorders and affecting the activity costing model negatively.

## Task/Action
My role as process engineer was to lead a cross functional team (maintenance, production, filling, packaging, raws and procurement) to effectively identify issues with cycle time and reduce this accordingly. By job was also to establish a tracking measure to identify improvement over time. The following was accomplished:

>* Developed the sites first statistical process control model and rolled out in both Johannesburg and Durban sites
>* Developed a annual reporting measure using MES data and carried out monthly reporting and troubleshooting with team to identify and mitigate issues
>* Tracked and worked with team to implement various projects

Example implementations:
>* Implementation of Overall Equipment effectiveness (OEE) in filling hall
>* Carried out a detailed capacity calculation across the manufacturing floor to identify bottleneck streams and re-assign capacity and manpower
>* Implemented a finite capacity scheduling modelling which improved scheduling while controlling cycle time
>* Developed an Excel based heijunkai model that was utilized in conjunction with a packaging supplier for load levelling
>* Optimized fill rates with nossil optimization and best practice maintenance
>* Carried out a finishing tank optimization exercise to reduce head losses and improve filling line hopper filling
>* Developed a pressure drop model which was used in the Johannesburg new automated robotics line
>* Implemented improved campaign scheduling on the shop floor
>* Implemented andon lights to identify when beads need changing as well as various 5s and 7W projects
>* Changed over from pot washing to high pressure cleaning which improved clean pot throughput and improved quality
>* Addressing FTR(first time right) issues
>* Lean six sigma project to reduce extras (which is left over product in the tank which can't be filled due to incorrect labelled packaging being supplied). This enabled a reduction in lead time
>* Carried out a PDCA project on slow resins which were resulting in increased cycle times. Evaluated and identified that the resin was thixotropic and heat sensitive and this was not catered for when it was outsourced. The lack of using a thinning time to warm the product as was done on site when it was internally manufactured resulted in colder months making the product much more viscous and slowing the fill rate. Adjusted specification and adjusted pump pressure to cater for the increased head losses. Lab experiments were also done to prove the dependency on temperature. 


## Results
Managed to reach a 10% reduction in average cycle times across the Johannesburg and Durban sites.

## Data Sources
Plant meters

## Software libraries
Excel, Python

<br />
<br />

# Project 7: Paint Floor Re-design

![](/assets/img/Layout2.PNG)

## Problem Statement
The manufacturing floor was not meeting the production volumes required and this was resulting in increased backorders and customer disatisfaction

## Task/Action
My role as process engineer was re-design the paint floor considering future capacity requirements while also ensuring adherence to quality requirements. The following high level activities were done:

>* Analyze Product Mix: Review the current and planned product mix to understand the variety and volume of products.
Determine Economic Batch Quantities (EBQ): Calculate EBQ for each product to optimize production efficiency and minimize costs.
>* Evaluate Existing Equipment: Assess the compatibility and capacity of existing equipment with the new product mix and production requirements.
Identify Equipment Gaps: Identify any equipment that needs upgrading or replacement to meet the new requirements.
>* Determine Production Capacities: Calculate the required production capacities based on product demand and EBQ.
>* Plan for Capacity Expansion: Develop a plan for expanding capacities, including the addition of new equipment or modifications to existing equipment.
>* Develop Functional Descriptions (FDS):
>* Process Breakdown: Break down the manufacturing process into individual sequences and operations for each product type.
>* Component Identification: Identify all components involved, including tanks, mixers, pumps, valves, and instrumentation.
>* Operation Description: Write detailed descriptions of each operation, including start-up, shut-down, interlocks, alarms, and failure modes.
>* Sequence of Operations: Define the sequence in which operations will occur for each product type, ensuring proper process flow and safety.
>* Control Philosophy: Document the overall control philosophy, explaining how the system will achieve control objectives like temperature, pressure, and flow rate control.

## Results
The new design was able to improve throughput and increased capacity substantially - eliminating a large proportion of backorders preventing profit loss.

## Data Sources
Plant meters, SAP, MII

## Software libraries
Excel, Python, AutoCad, Visio

<br />
<br />

# Project 7: Cost Savings Process Improvement Headed by CFO

![](/assets/img/CostSavings.PNG)

## Problem Statement
There was massive pressure on the Kansai Plascon SA group to reduce cost to maintain profitability.

## Task/Action
I was given the task to carry out a cross functional process improvement cost reduction initiative on behalf of the site executive. This would involve collaborating with cross functional management teams to identify and carry out projects with cost savings in mind. My job would also be to mentor and guide the team with process improvement methadologies while also carrying out my own improvement initiatives. Consolidated and tracked savings and presented directly to the CFO. 

Example projects:
>* Waste disposal cost avoidance
>* Packaging and material reworking initiatives
>* Solvent reduction and recycling exercises
>* Formulation changes to optimize recipe cost
>* Electricity cost reduction
>* Changeover time reduction
>* Stock accuracy improvement
>* Maintenance costs reductions
>* Supplier cost optimizations
>* Yield losses reductions
>* Warehouse outsourcing and implementation of a day warehouse to house temporatory product

## Results
Overall the Mobeni site was able to carry out 25 improvement projects with an overall saving of over R25 million rands. 

## Data Sources
Plant meters, SAP, MII

## Software libraries
Excel, Python, Visio

<br />
<br />


# Project 8: Cooling Tower Optimization for Cost Savings and Efficiency

![](/assets/img/Cooling.jpg)

## Problem Statement
The Cooling Towers at Kansai plascon were not operating efficiently resulting in an increase of operating cost.

## Task/Action
My role as process engineer was to the operations manager to optimize the cooling towers for efficiency and cost reduction

> * Walked the process and developed a P&ID representing the system
> * Developed a mass balance to account for water losses
> * Identified and mitigated issues for poor efficiency and cooling as well as increased cost
> * Developed a comprehensive report back to management for changes to be complete
> * Carried out implementations
> * Improvement of risk assessments, FMEA
> * SOP modifications
> * Improvement of plant maintenance schedules
> * Carried out cooling tower efficiency calculations to quantify benefits
> * Installed new measurement devices and carried out a guage R&R study to ensure reliability of measurement system

## Understanding the Chemical Engineering Processes
>* In crossflow cooling towers, water flows vertically while air flows horizontally across the water stream.
>* In counterflow towers, air flows upward while water flows downward - this design allows for more heat transfer 
>* The cooling capacity of the cooling tower can be given by the equation:

![image](https://github.com/user-attachments/assets/91eafb15-251f-4725-b5d9-8ef08622bd57)

>* Decreasing the flowrate of water, decreases the cooling capacity but increases the heat transfer as a result of increase in resonance time - more contact time between water and cold air (laminar flow)
>* flow patterns affect the overall heat transfer coefficient as with boilers - Re number can calculate whether turbulent or laminar flow. Then can determine Nu number and U value:

![image](https://github.com/user-attachments/assets/8d339158-b27c-4550-9227-43bd971aa4d9)

![image](https://github.com/user-attachments/assets/074c92bd-782f-4dce-987e-18f7feaf3a4e)

![image](https://github.com/user-attachments/assets/312fbcf8-8cc4-4530-837c-d61f7c869af3)

>* The design cooling capacity of the cooling tower is the maximum capacity that can be reached based on conditions at the time e.g. inlet temp, wet bulb temperature, filling etc.
>* The actual cooling capacity is what the tower can actually do with inefficiencies
>* The heat load calculated also by mcpdeltaT is what heat removal is required by the cooling tower
>* If the cooling tower can't match this - the output water temperature required would not be reached in the given time
>* Reducing the inlet temperature with pre-processing can reduce heat load required by cooling tower.

![image](https://github.com/user-attachments/assets/f6381561-f6a6-4741-9b32-9d22c58c7951)

>* the heat transfer rate can be given by the above equation, as can be seen, the larger the surface area for heat transfer the greater the Q
>* Heat transfer area can be improved by increasing the tower height, packing and decreasing the fowling and scaling which decreases the area
>* The fowling can be prevented by making sure there is sufficient blowdown and chemical treatement/dosing
>* When the heat transfer rate increases, the cooling capacity increases
>* Proper distribution in the tower can also ensure maximum usage of heat transfer surface area

![image](https://github.com/user-attachments/assets/566c0411-7975-4223-bcd3-fef1aedd19d4)

>* Increasing the air flow will increase the cooling efficiency by increasing the heat transfer coefficient (turbulent flow - air heat transfer coefficient increases), but also increase the fan power at a cubic increase. This means a balance must be achieved.

![image](https://github.com/user-attachments/assets/92e1484e-3506-481e-944a-7a629d9806a9)

>* the efficienct of the cooling tower is defined as the actual change in temperature over the approach ( the max amount of heat that can be removed due to the wet bulb temperature)
>* The wet bulb temperature is the lowest temperature that can be achieved due to evaporative cooling. It is dependent on the humidity and temperature of the air
>* you can change the location of the cooling tower to increase the wet bulb temperature and approach thus increasing the potential cooling capacity
>* The mass balance equation is given below:

![image](https://github.com/user-attachments/assets/dccd4ef6-7fcc-4dc8-bfec-64079fb2891e)

>* This can tell us if there is significant loss in system e.g. blowdown or drift losses or insufficient make up water replenishment
>* The energy balance across the cooling tower can be given by:

![image](https://github.com/user-attachments/assets/0d696dbf-b401-4796-8f2f-aecd3fa1fae1)

![image](https://github.com/user-attachments/assets/a1b27cb8-9620-42c4-937a-ee3e20bd2537)

![image](https://github.com/user-attachments/assets/3b9ce42e-24e5-4552-afa7-7ed471c1a482)

![image](https://github.com/user-attachments/assets/5c8dcf11-a174-4576-b7ba-fd36051bf79b)

What typical operational issues to look out for:
>* poor airflow as a result of blockages in air inlets, fans, or fill material due to debris, dirt, or mechanical issues
>* Excessive drift from too high airflow or drift eliminators not working efficiently
>* Corrosion from corrosive nature of water - can occur due to lack of corrosion inhibitors during treatment. Can lead to structural damage, leaks and equipment failure
>* Biological growth causing fowling as a result of incorrect treatment and lack of sufficient blowdown
>* Excessive water loss due to too much blowdown, or drift or leaks
>* Airflow reduction from mechanical issues in fans and motors
>* Improper water distribution as a result of spray nozzles not working efficiently results in hot spots and reduces cooling efficiency
>* Make-up water not at the required quality resulting in scale build up etc.
>* Temperature control issues for measurement of inlet and outlet water temperature.

Key implementations:
> * Re-designed maintenance schedules to reduce fowling in the cooling tower and improve chemical treatment to improve cooling and reduce energy use
> * Identified issues for fowling such as inadequate blowdown and poor chemical treatment - fixing this improved efficiency 
> * Varied the chemical usage based on months when bacterial growth varies and this resulted in cost savings of chemical treatment
> * Investigated the option of VSD for the fans to optimize energy use, improve efficiency. Increasing the fan airflow increases the rate of heat transfer but increases fan power with the cube of airflow. VSD's can balance this
> * Optimizing of the water flow rate was done. Reducing the water flow rate increases the residence time in the cooling tower, improving heat transfer but also reducing the cooling capacity (rate of cooled water leaving the tower)
> * Looking at ensuring maintenance of the filling - was able to improve heat transfer efficiency 

## Data Sources
Operational reports, meter readings, operator reports

## Software libraries
Excel was utilized for all calculations, Visio for P&ID

## Data Analytics Methods
Statistical and graphical analysis, mass and energy balances

<br />
<br />

# Project 9: ISO-18001 Recertification

![](/assets/img/18001.png)

## Problem Statement
The site was at risk of losing it's ISO-18001 certification. This would have resulted in huge fines and also loss of customer faith and market share loss. In addition safety of onsite personnel would not be maintained.

## Task/Action
My role as process engineer was to assist the SHERQ department as lead in facilitating the effective risk assessment across site. This included gap analysis, technical assistance and consolidating the completion of all risk assessments across site against a stringent 6 month deadline.

## Result
The site was re-accredited and maintained its ISO-18001 certfication within the designated time frame.

<br />
<br />


# Project 9: Reactor heating and cooling automation (Capex: R300000)

![](/assets/img/P&ID.PNG)

## Problem Statement
The Kansai Plascon K6 reactor temperature control has a partial automation. This posed several business risks from an efficiency, safety and ergonomics risk. The reaction within the reactor was highly exothermic, which means that the case of a runaway reaction was possible and in cases such as this a fully automated system would be much more safer as opposed to operators manually operating valves during a dangerous situation that is highly time intensive. 

## Task/Action
My role as process engineer was to facilitate the automation of the heating and cooling cycle for the reactor considering process and safety requirements. The following was done:

Project scoping/Preliminaries
>* Evaluate current system of operation and identify issues
>* Evaluate safety requirements and legislature

Complete preliminary documentation
>* Project brief
>* Process flow diagram & P&ID
>* Control narrative/ functional requriements specification/ control philosophy
>* Alarm/trip lists
>* Work with automation to evaluate options
>* Apply for quotations and selection of suppliers based on cost and quality
>* Risk assessments
>* CAPEX application 
>* CAPEX approval

PLC and SCADA upgrades (outsourced to automation - managed the process)
>* System capability check and card installation
>* ladder logic diagrams on PLC
>* Control tuning
>* HMI upgrade on SCADA
>* Testing 

Training and handover
>* Train opeators on new controls
>* Observe processes to determine if controls are effective
>* SOP modifications
>* FMEA modifications

## Result
The system changed were achieved within budget

System before changes:
![](/assets/img/Current.PNG)

<br />
<br />

System after changes:
![](/assets/img/Proposed.PNG)

<br />
<br />

# Project 10: Linear Programming Model to Optimize product mix

![](/assets/img/Linear.PNG)

## Problem Statement
The Kansai Plascon group was under pressure to reduce cost and improve efficiencies. One such path to that was optimizing product mix to achieve maximum profit.

## Task/Action
I explored the option of developing a linear programming model within a pilot area (Lean GP section). A model objective function was developed to maximize profit based on all products in the lean GP section. The model was constrained by several factors:
>* Capacity constraints
>* Demand constraints
>* Cost/L constraints
>* Manpower constraints

## Result
The exercise was successful in indicating the optimum product mix to achieve the highest cost, however due to customer requirements it was not practical to implement the model results, as the model indicated a higher sales of a product that usually has a lower demand yet higher sale price. The results did however give further insight into SKU rationalization as a potential future activity within the business.


<br />
<br />

# Project 10: Product Costing Model Update

![](/assets/img/Activity.PNG)

## Problem Statement
The Kansai Plascon group had issues with the costing model. 1) The recipe hours were not a true reflection of the physical process. Cost recoveries were low and understated the COGS value of products.

## Task/Action
Investigate and implemented ways to improve the model. Initially manufacturing overheads was caculated using a fixed dwell time based on the machine hours. So the fixed, variable and labor hours were the same. This was redefined:

Fixed hours: usable machine capacity constrained by bottleneck
Labor hours: no. of operators * hours per month * efficiency factor
variable hours: budget hours based on forecast requirements

Recipe hours were split into fixed, labor and variable as opposed to a single dwell time value
Activity rate can be calcualted for each category of fixed, labor and variable costs which is a better indicator of efficiency and improves costing estimation

## Result
40-60 % accuracy improvement in model i.e. reduction in under recoveries value.

<br />
<br />

# Project 10: Water Base Production Facility (CAPEX - R15 000 000)

![](/assets/img/Water.PNG)

## Problem Statement
The Kansai Plascon group had issues with maintaining waterbase products. A new plant was to be designed and installed to meet requirements.

## Task/Action
To design new plant configuration and assist with installation of new plant. The following was accomplished:

* Pre-planning phase (Envisioning)
>* Completion of Project Brief document
>* All stake holders endorse Project Brief document

* Design Phase
>* Product Mix identification & procesing requirements
>* PFD & Operations Philosophy design
>* Technology Selection & Equipment Sizing
>* P&ID and Workflow design
>* Utilities required
>* Legal assessments (E.g. EIA)
>* Equipment Selection

* Approval Phase
>* RFQ & Costing
>* Project Execution Plan
>* Memo of Justification
>* CAPEX & MOJ Approval
>* Project approved

* Procurement Phase
>* Long-lead time items
>* Local equipment orders

* Execution Phase
>* Plan submission
>* EIA & other surveys
>* Civil Structures & Utilities
>* Equipment Installation
>* Automation & SAP

* Commisioning Phase
>* Plant Commisioning
>* Snaglist completion
>* ISO Documents and training
>* Sign-off & Handover

>* ## Result
Plant was successfully commissioned within budget.

<br />
<br />

# Project 11: RMS Dust Extractor Installation (CAPEX - R500 000)

![](/assets/img/Dust.PNG)

## Problem Statement
The Kansai Plascon group was facing audit compliance issues at the RMS in the Mobeni site. The dust emissions were deemed too high for safe work. This posed a hazard to workers

## Task/Action
To investigate and install a new dust extraction system in RMS powder weighing area to eliminate risk to employees while weighing dangerous powders. To improve overall area to ensure safety and eliminate risk while working. The following was accomplished: 

* Project scoping/preliminaries
>* Task 1 : on the field observations to determine viability of dust extraction
>* Task 2 : Develop project brief/scope/initial timelines/ safety concerns & legislation
>* Task 3 : Determine unit design based on particles being extracted
>* Task 4 : Confer with contractors about options/configurations (obtain quotes)
>* Task 5: Choose an appropriate option and design review
>* Task 6 : Capex application and approval
>* Task 7: Unit ordering
>* Task 8: Confirm if old positioning of system is still viable
>* Task 8 : Risk assessments

* Install local exhaust ventillation (LEV) system
>* Task 1 : Unit installation (first installation showed poor workmanship - time spent also fixing snags)

* Ensure that relevant SOP's are updated
>* Task 1 : Determine which SOP's are affected or if it any need to be created
>* Task 2 : Updating and creating new SOP's

* Train staff on new equipment and protocols/commissioning
>* Task 1 : Train staff on new equipment
>* Task 2 : Observe if operators are using equipment correctly/commissioning
>* Handover

## Result
Unit was successfully installed and safe operation was achieved. Area was tested and dust levels were within requirement of OHSA.

# Project 12: Plate and Frame Heat Exchanger Optimization

![image](https://github.com/user-attachments/assets/e7430a56-934f-40c4-aab1-31349c23229e)

## Problem Statement
The heat exchanger at Kansai plascon were not operating efficiently resulting in water temperature not reaching desired ranges for steam bath. This was affecting the raw material and causing batch rejects.

## Task/Action
My role as process engineer was to assist the operations manager to optimize the plate and frame heat exchanger for efficiency and cost reduction

> * Walked the process and developed a P&ID representing the system
> * Developed a mass balance to account for water losses
> * Developed an energy balance to account for energy losses
> * Identified and mitigated issues for poor efficiency and heating as well as increased cost
> * Developed a comprehensive report back to management for changes to be complete
> * Carried out implementations
> * Improvement of risk assessments, FMEA
> * SOP modifications
> * Improvement of plant maintenance schedules
> * Carried out heat exchanger efficiency calculations

## Understanding the Chemical Engineering Processes
>* The heating capacity of the heat exchanger can be given by the equation:

![image](https://github.com/user-attachments/assets/c5748086-e144-435b-b318-c47150cb4508)


>* Decreasing the flowrate of water, decreases the heating capacity but increases the heat transfer as a result of increase in resonance time - more contact time between water and cold air (laminar flow)
>* flow patterns affect the overall heat transfer coefficient as with boilers - Re number can calculate whether turbulent or laminar flow. Then can determine Nu number and U value:

![image](https://github.com/user-attachments/assets/8d339158-b27c-4550-9227-43bd971aa4d9)

![image](https://github.com/user-attachments/assets/074c92bd-782f-4dce-987e-18f7feaf3a4e)

![image](https://github.com/user-attachments/assets/312fbcf8-8cc4-4530-837c-d61f7c869af3)

>* The design exchanger capacity of the heat exchanger is the maximum capacity that can be reached based on conditions at the time e.g. inlet temp, wet bulb temperature, filling etc.
>* The actual heating capacity is what the exchanger can actually do with inefficiencies
>* The heat load calculated also by mcpdeltaT is what heat addition is required by the heat exchanger or how much the water needs to be heated
>* If the heat exchanger can't match this - the output water temperature required would not be reached in the given time
>* Increasing the inlet temperature with pre-processing can reduce heat load required by heat exchanger 

![image](https://github.com/user-attachments/assets/f6381561-f6a6-4741-9b32-9d22c58c7951)

>* the heat transfer rate can be given by the above equation, as can be seen, the larger the surface area for heat transfer the greater the Q
>* Heat transfer area can be improved by increasing the dimension of plates, decreasing fowling/scaling
>* The fowling can be prevented by making sure there is sufficient blowdown and chemical treatement/dosing
>* When the heat transfer rate increases, the heating capacity increases
>* the efficiency of the heat exchanger is defined by the equation below:

![image](https://github.com/user-attachments/assets/3a42ead4-d044-46b7-a2a2-36a9e9bbd9a5)

![image](https://github.com/user-attachments/assets/b9ac1f95-942b-45d9-bc4e-55a37748b846)

>* You can change the value of the Cp by changing the liquid to get better heat transfer

![image](https://github.com/user-attachments/assets/dccd4ef6-7fcc-4dc8-bfec-64079fb2891e)

>* This can tell us if there is significant loss in system e.g. blowdown or drift losses or insufficient make up water replenishment
>* The energy balance across the heat exchanger can be given by:

![image](https://github.com/user-attachments/assets/5da0ce3e-945c-4bdf-b0d3-381f5b135cfc)

>* the mass balance can be given by:

![image](https://github.com/user-attachments/assets/fa5e7de9-637e-4c56-a680-4c155d57682a)


What typical operational issues to look out for:
>* Increase in pressured drop, reduces flow, reduces U and reduces heat transfer rate - this occurs as a result of blockages
>* Corrosion from corrosive nature of water - can occur due to lack of corrosion inhibitors during treatment. Can lead to structural damage, leaks and equipment failure, mixing of chemicals, thinning plates, holes in plates
>* fowling and scaling as a result of incorrect treatment and lack of sufficient blowdown
>* large temperature gradient as a result of inlet temperature being too low - causes mechanical stresses, warping etc.. which disrupts fluid flow
>* Air entrapment causing air pockets in system which affects heat transfer - need venting valves
>* Gasket failure resulting in leaks and cross contamination

Key implementations:
>* Re-designed maintenance schedules to reduce fowling in the heat exchanger and improve chemical treatment to prevent fowling and corrosion
>* Gaskets were changed to prevent cross contamination and leakages
>* Increased inlet temperature of water through process changes
>* Reduced blockages in system - increasing system flow to turbulent conditions increasing the heat transfer coefficient and the heat transfer rate

## Data Sources
Operational reports, meter readings, operator reports

## Software libraries
Excel was utilized for all calculations, Visio for P&ID

## Data Analytics Methods
Statistical and graphical analysis, mass and energy balances

<br />
<br />

# Feasibility Studies

![](/assets/img/Feasibility.jpg)

The following feasibility studies were done to assist R&D, operations and manufacturing to make decisions and implement projects:

* Benefits of outsourcing filling operations e.g. 1L lines
* Removal or replacement of raws in batches and its effect on cost e.g. INT replacement
* Determining feasibility of new equipment installation of efficency and cost e.g. introduction of a bag destuffing unit
* Switch pot cleaning from pot cleaner to HP cleaning and its effect on cost
* Boiler fuel replacement
* Recipe formulation changes and its impact
* Effect of changing product streams
* Effect and benefit of increasing capacity on a particular stream
* Moving products to other sites e.g. Durban to PE and its impact
