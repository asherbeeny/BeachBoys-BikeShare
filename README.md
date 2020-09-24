# BeachBoys BikeShare Exploratory Analysis
 
 BeachBoys BikeShare is a bike share service provider where users can take and return bikes at any of the 70 stations on their network. 
 
 The company wants to leverage their data o better understand and, hopefully, optimize their operations. They are interested in exploring the potential of statistical and/or machine learning models to predict the number of bikes taken and returned to each station. 

If this project is successful they would like to use the output of the predictive model to help the logistics department schedule the redistribution of bikes between stations. This in turn will help ensure there are bikes and return docks available when and where users need them. 

To arrange this schedule, they need an estimation of the net change in the stock of bikes at a station for the time window between two pick-up/drop-off visits so the station may ace the upcoming demand. Naturally, the number of visits for each station and thus these ime windows will depend on the intensity of use of that station, the use of other stations in the network, as well as resources available. 

As a first step towards tackling this challenge, the company has asked you to develop a model capable of outputting the net rate of bike renting for a given station (net rate is defined as trips ended minus trips started at the station for a given hour). That is, at any ime the logistics team of the company should be able to make a statement such as 'In the next hour, the net stock of bikes at station A will change by X. Results should be accompanied by the root-mean-square error (RMSE) metric as a measure of performance of each presented model. You are free to use other metrics to discuss a model's merit. 
Deliverables 

# Modeling Approach
This is a regression use case, we need to use regression models.
We will use RandomForestRegressor and GradientBoostingRegressor algorithms
Prepare the data after analyis
Split the data into train and test splits
Use above mentioned models to predict the outcome
Check the model perforomance


# Potential Imporvements
Here are some of the imrovmeents that can be impemeneted in the future:
- Impute null values
- Join with Weather data to add more value to our model
- Drop highly correlated independent variable
- Handle Trip outliars : Need more investigation , some trips has more than 100 minutes duration
- Extract holiday/business days features and add them to the model
- Use spatial data in the analysis and we can overlay the nalysis on the map to have an eagle eye view of the trips
- Link with city dempgraphics and census data to add more value to the analyis
- Add tourists numbers and predictions to the data to help us in predicting more accurate numbers of the visitors


# Conclusion
- San Francisco City has the largest number of Bike Docks
- The distrubtion is right skewed, most of the trips are between 1 miutes and 10-15 minutes
- Subscriber Type " Subscriber" has the majority of the trips in the platform. Customers are mostly visitors to the city
- Most of the "Subscriber" trips are done in the morning (between 6-9 AM) and (4-8 PM) . the normal commute hours
- the "Customer" trips are steady between 6 AM and 8 PM, usually for visiting the city
- Most of the trips are on the normal weekdays, and very less during weekends
