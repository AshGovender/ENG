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

# [Project 3: Customer Complaints Clustering Model ](https://github.com/TheProcessBoy/Stock-Health-Improvement)

![](/assets/img/Main.PNG)

## Problem Statement
Company X had several customer complaints issues and wanted to develop a clustering model to cluster their different customer complaints group to get an indication of how to handle each group.

## Task/Action
My task was to develop a clustering algorithm that looked at customer returns data and develop a clustering alogorithm to group the data accordingly to gain further insight into the customer complaints experienced. Since it was numerical data, A K-modes algorithm was utilized to develop the clusters. The algorithm starts by picking some random points which will be considered the first cluster centers (centroids). In other words, the clusters will be defined based on the number of matching categories between data points that means using the highest frequency to form the clusters. As in more categories two points overlap, the higher their probability to belong to the same cluster. Below indicates the process:

![](/assets/img/Picture1.png)

Drawback of K-Modes is that we need to input the final number of clusters by which to split the data points
To find the optimum number of splits, the Elbow method with the cost function is used. A cost function to determine how scattered the points are from the cluster needs to be established. The lower the cost, the nearer the points in the cluster. With K-Means the Euclidean distance is used whereas in K-Modes, it is replaced by the Hamming distance  
∑_(𝑖=1)^𝑛▒∑_(𝑖=1)^𝑘▒𝑑_𝑥𝑐 

By plotting the cost function against the number of clusters, an elbow should be found. During the clusters number growth, there is a point where the drop starts to change smoothly, and the increase of k does not give significant improvements. The number where the cost begins to slightly decrease is the number that best fits data-set sub-grouping 

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
Dimensional reduction(feature addition), data imputation and cleaning(removing null values), feature selection,


