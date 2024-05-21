# Academic Qualifications
> * Bsc. Chemical Engineering
> * Msc. Mechatronics Engineering

# Licenses and Certificates
> * Lean Six Sigma Greenbelt

# Courses
> * [Data Science Methadology (Coursera - IBM)] - [View Certificate](https://www.coursera.org/account/accomplishments/certificate/NXGZBLFKJ8QR)
> * Machine Learning With Python (Coursera - IBM) - [View Certificate](https://www.coursera.org/account/accomplishments/certificate/VZTZQQPXC4SB))



# [Project 1: Python Based Evaporation Loss Calculator](https://github.com/TheProcessBoy/Evaporation-Loss-Calculations)

![](/assets/img/case-study-solvent-tank.jpg)

## Problem Statement
There was huge losses in solvent that could not be accounted for. As a result, all avenues of solvent loss needed to be catered for. Solvent losses are possible through open tanks and could have possibly been contributing to the variance identified.

## Task/Action
My job was to utilize my chemical engineering knowledge and determine if the tank losses were significantly impacting the stock take shortages. I calculated losses through the solvent tanks using python to carry out the calculations.

## Data sources
Plant data such as tank dimensions, thicknesses and design factors were obtained from the maintenance department. Other unknown coeffiecients and factors were estimated using theoretical data obtained online and engineering judegment played a big role.

## Results 
The caculations showed negligible losses of solvent from the tanks, hence we could rule this out as a potential issue for the solvent losses. After re-looking at the process we found that losses were attributed to calibration issues during PLC loading of solvent.

## Python libraries
Math

## Data science Methods
Functions


# [Project 2: Stock Health Improvement Project ](https://github.com/TheProcessBoy/Stock-Health-Improvement)

![](/assets/img/Stockhealth.PNG)

## Problem Statement
Company X had issues with their stock health system. The head of supply chain had created a stock health tool that had various zones to trigger re-order points, however this was still resulting in stock-outs and dips in the red zone (safety stock level). This was unhealthy practice and resulted in consistent backorders.

## Task/Action
My task as process engineer was to work with the head of supply chain and the managers of the entire supply chain to identify and mitigate reasons for the stock-outs. I utilized elements of lean six sigma and Python to carry out rigorous data analysis using Qlickview and production data. 

## Data sources
Utilized production planning data, sales data, SKU Master data, Forecast data, sales and volumes data from Qlickview, SAP and MII to carry out the investigation

## Results 
The combined approach of lean six sigma and data analysis yielded positive results. Results showed that there were several issues :
> * Forecast values missing for certain products - this list was sent and corrected by the forecasting team (Quick win)
> * Scheduling unable to build stock to plan as a result of production capacity issues - manpower shift alignment was done to ensure no rollovers
> * Forecasting inaccuracies - this was taken as a side project to optimize forecast accuracy on the selected products
> * Filling bottleneck i.e. filling unable to start batch on time due to reprioritization - capacity increased on the plant through a side project that looked at nozzil optimization, faster hopper fill rate, SMED practices.

## Python libraries
Matplotlib, Pandas, Numpy, itertools

## Data science Methods
Feature addition, feature extraction, data merging, data visualization, data aggregation, data transformation(column renaming, column splitting)

# [Project 3: Customer Complaints Clustering Model ](https://github.com/TheProcessBoy/Customer-Complaints-)

![](/assets/img/Main.PNG)

## Problem Statement
Company X had several customer complaints issues and wanted to develop a clustering model to cluster their different customer complaints group to get an indication of how to handle each group.

## Task/Action
My task was to develop a clustering algorithm that looked at customer returns data and develop a clustering alogorithm to group the data accordingly to gain further insight into the customer complaints experienced. Since it was numerical data, A K-modes algorithm was utilized to develop the clusters. The algorithm starts by picking some random points which will be considered the first cluster centers (centroids). In other words, the clusters will be defined based on the number of matching categories between data points that means using the highest frequency to form the clusters. As in more categories two points overlap, the higher their probability to belong to the same cluster. Below indicates the process:

![](/assets/img/Picture1.png)

Drawback of K-Modes is that we need to input the final number of clusters by which to split the data points
To find the optimum number of splits, the Elbow method with the cost function is used. A cost function to determine how scattered the points are from the cluster needs to be established. The lower the cost, the nearer the points in the cluster. With K-Means the Euclidean distance is used whereas in K-Modes, it is replaced by the Hamming distance  
∑_(𝑖=1)^𝑛▒∑_(𝑖=1)^𝑘▒𝑑_𝑥𝑐 

By plotting the cost function against the number of clusters, an elbow should be found. During the clusters number growth, there is a point where the drop starts to change smoothly, and the increase of k does not give significant improvements. The number where the cost begins to slightly decrease is the number that best fits data-set sub-grouping. For the given project, the curve levelled off at around a K value of 7 which indicated optimum number of clusters.

Exploratory data analysis was done on the individual dataframes and then joined together and filtered based on necessary columns to create one dataset and the model was fitted with the data using a K value of 7. Other intial model parameters were selected based on best practice.

## Data sources
Utilized customer complaints data from the call centre, production planning and MasterSKU data

## Results 
The results were as follows :
> * 3 clusters were developed
> * Each cluster had a specific sales category and a major bulk purchaser attributed to it
> * Each cluster indicated product specific issues and problematic customers to be addressed that were frequently returning items for no real reason and as a result of their poor forecasting
> * The data also pointed to sales reps that were not effectively controlling the customer complaints returns processes i.e. they were approving all returns without a proper investigation
> * The most problematic customers in terms of returns were also identified

## Python libraries
Matplotlib, Pandas, Numpy, itertools, K-modes algorithm

## Data science Methods
Dimensional reduction(feature addition), data imputation and cleaning(removing null values), feature selection.

# [Project 4: Customer Quality Complaints NPL Model ](https://github.com/TheProcessBoy/Customer-Quality)

![](/assets/img/Paint.jpg)

## Problem Statement
Company X had issues with classifying their customer complaints into specific groupings on a manual basis. Grouping would help them identify problematic issues that they should focus their efforts on resolving. Although the team had worked to create a comprehensive labelled dataset, this was becoming a laborious task to re-label new data from the call centre.

## Task/Action
My task was to develop a NPL model(Multi-class text classification) to identify what customer complaints descriptions correlate to which customer issue. The text was first cleaned and tokenized before being converted to numerical values for classification. The conversion to numerical values was done using the TF-IDF Vectorizer. The data was split into a training, test and validation set before fitting various models (random forest, SVM, decision trees, Naive Bayes. The model were then tuned using the GridsearchCV method and the LeaveOneOut() cross validation method. Each models accuracy was calculated and remaining F1, Precision and accuracy scores were calculated for the best performing models using a classfication report. A correlation matrix was also done.

## Data sources
Utilized customer complaints data quality data from the call centre

## Results 
The resulting model could classify new customer orders into their relevant quality reason code groupings. This saves manual labor time and allows concentrated efforts on specific quality reason codes e.g. Bittyness was found to be a recurring issue across a certain range of product and upon closer observation it was found that a raw material change resulted in the recurring issue. After implementing changes on a recipe level, the problem was not a recurring theme in upcoming customer quality complaints.

The model was best fitted with a SVM and decision tree algorithm, however certain classes were under-represented and therefore more data collection is needed to improve the model reliability.

## Python libraries
Sklearn( DecisionTreeClassifier,metrics, naive_bayes,svm,model_selection,feature_extraction.text), matplotlib, seaborne, Pandas, Numpy,nltk(tokenize,corpus,stem)

## Data science Methods
Text preparation (conversion to lower case, removing stop words, removing whitespaces and punctuation, tokenization, lemmatization), training and test split, model tuning, model fitting, cross-fitting, model evaluation, exploratory data analysis

# [Project 5: Stroke Prediction Using a Binary Classification Model ](https://github.com/TheProcessBoy/Customer-Quality)

![](/assets/img/Stroke.jpg)

## Problem Statement
Stroke is a serious condition that affects millions of people in the world. Although its exact causes can't be pinned down to specific issues, there are potential physiological and lifestyle characteristics that could put a person at greater risk of having it. However many people are not aware of these factors and how they can contribute to the likelihood of getting cancer.

## Task/Action
As part of my Masters in biomechatronics, I developed a ML model that was initially hosted on MS Azure and consumed by a Mobile & web application developed. The model was re-produced on python and is basically looked at classifying whether a person is likely to get a stroke based on various different factors. The data was cleaned and exploratory data analysis was used to identify patterns in the features and in relation to the target variable. The categorical data was one-hot-encoded after removing outliers and normalizing the dataset. A smote analysis was also used to rectify the imbalanced dataset. A train, test and validation data split was done. The various models were tuned using GridsearchCV and the k-folds algorithm. 

## Data Sources
Online medical health repository

## Results 
The classification scoring was done and showed that the model was good at predicting negative cases however data imbalance in the test set showed a weak model in predicting the postive class. A learning curve showed that more data was required to improve the model with more positive case predictions required to strenghthen the models ability to predict the positive stroke class.

## Python libraries
Sklearn( DecisionTreeClassifier,metrics, naive_bayes,svm,model_selection,feature_extraction.text), matplotlib, seaborne, Pandas, Numpy etc.

## Data science Methods
Text cleaning, SMOTE analysis, training and test split, model tuning, model fitting, cross-fitting(k-folds), model evaluation, exploratory data analysis



# Project 6: Backorder Reduction Using DMAIC Methadology

![](/assets/img/backorder-tag-feature.jpg)

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


# Project 7: Boiler Optimization and Environmental Compliance

![](/assets/img/Boiler.PNG)

## Problem Statement
The boiler at Kansai plascon was not adhering to environmental compliance in terms of particulate matter and sulphur dioxide fumes. This was resulting in fines and other prosecutions on site until compliance could be achieved. In addition, the boiler was operating inefficiently resulting in an increase of operating cost.

## Task/Action
My role as process engineer was to assist the SHERQ department in not only ensuring adherence to environmental regulations but also to improve efficiencies in the boiler to reduce cost. The following was achieved:

> * Walked the process and developed a P&ID representing the system
> * Developed a mass balance to account for water and steam losses
> * Identified and mitigated issues for loss of steam, loss of condensate, increase fuel usage, particulate matter and sulphur dioxide increases
> * Developed a comprehensive report back to management for changes to be complete
> * Carried out implementations
> * Improvement of risk assessments, FMEA
> * SOP modifications
> * Improvement of plant maintenance schedules
> * Carried out steam and energy calculations
> * Installed new measurement devices and carried out a guage R&R study to ensure reliability of measurement system

Key implementations:
> * Re-designed maintenance schedules to reduce fowling in the boiler to improve heat transfer and reduce fuel usage
> * Identified condensate losses which resulted in wastage of heat and treatment chemicals through steam trap damage and incorrect condensate recovery control logic
> * Ensure air/fuel ration was corrected which fixed the particulate matter issue
> * did a cost benefit analysis and implemented a new fuel changeover from HFO to LFO that resulted in sulphur dioxide emissions compliance without a significant capex and operating cost
> * Led the installation of an autoflam unit which ensured optimized air fuel ratio and reduced fuel usage
> * Led the correction of the steam control system which ensure optimum maintenance of feedwater to the boiler reducing fuel necessary to heat the water to saturated steam
> * All steam trap and leaking lines were fixed resulting in optimum condensate recovery as well as steam
> * Carried out various engineering calculations to quanitify and identify cost savings and benefits analysis
> * Assisted with 

## Data Sources
Operational reports, meter readings, operator reports

## Software libraries
Excel was utilized for all calculations, Visio for P&ID

## Data Analytics Methods
Statistical and graphical analysis, mass and energy balances
