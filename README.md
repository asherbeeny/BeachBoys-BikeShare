# BeachBoys BikeShare Exploratory Analysis
 
 BeachBoys BikeShare is a bike share service provider where users can take and return bikes at any of the 70 stations on their network. 
 
 The company wants to leverage their data o better understand and, hopefully, optimize their operations. They are interested in exploring the potential of statistical and/or machine learning models to predict the number of bikes taken and returned to each station. 

If this project is successful they would like to use the output of the predictive model to help the logistics department schedule the redistribution of bikes between stations. This in turn will help ensure there are bikes and return docks available when and where users need them. 

To arrange this schedule, they need an estimation of the net change in the stock of bikes at a station for the time window between two pick-up/drop-off visits so the station may ace the upcoming demand. Naturally, the number of visits for each station and thus these ime windows will depend on the intensity of use of that station, the use of other stations in the network, as well as resources available. 

As a first step towards tackling this challenge, the company has asked you to develop a model capable of outputting the net rate of bike renting for a given station (net rate is defined as trips ended minus trips started at the station for a given hour). That is, at any ime the logistics team of the company should be able to make a statement such as 'In the next hour, the net stock of bikes at station A will change by X. Results should be accompanied by the root-mean-square error (RMSE) metric as a measure of performance of each presented model. You are free to use other metrics to discuss a model's merit. 
Deliverables 

