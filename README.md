
# Project Name: Capstone824
### Course: MGMT 59000 AI Assisted Big Data in the Cloud
### Purdue University Summer II 2024
### Team Name: Ninja_1

# Executive Summary: 

## Requirements:
### The intention is to combine at least one (in this case 2) Archived (herein referred to as static) data sets with one live API to analyze energy consumption patterns. 
### The project should utilize at least three Google Cloud Components

## Business case/Problem Statement:
### The electrical grid in the United States does not have significant energy storage capacity, and there is a cost to transporting and storing fuel for consumption. This creates a cost burden for energy companies who either produce too little or too much energy in a given time window. 

## Our Solution:
### To facilitate the building of a future optimization model, we've built an ETL pipeline and proof-of-concept prediction model for energy consumption requirements for Trenton Falls, NY. By Analyzing historical weather and energy consumption data, we attempt to use live weather data for zip codes in Trenton Falls, NY to estimate the likely energy needs in the current month. By using a mature prediction model to create an optimization model, energy producers could reduce both storage and transportation costs.

## Key Findings:
### We find a strong, negative correlation (-0.82) between temperature and energy consumption, strongly suggesting that colder months require significantly more energy than cooler months. 

## Strengths of our model: 
### While temperature is not the only factor in determining usage, many other prediction models, such as predictions based on cell phone usage, are not able to be adjusted by seasonal factors, affecting their reliability. We believe our model could be used to augment other models in the future, addressing the limitations of both models.


## Limitations of our model: 
### Few states track energy below the state level, and only limited weather stations keep records of local temperature in public data sets. While our model can be used to predict energy consumption for localities that track both data points, it cannot predict energy needs for areas that do not. Furthermore, the correlation will likely differ depending on location, meaning a fully matured model would need to adjust for location. The current model accounts for New Yorks harsh winters and mild summers, but an opposing correlation might be observed in a warmer climate, like Florida, where cooling in summer is more difficult than heating in winter. More research is necessary to improve the model.

## Reccomendations: 
### To improve prediction of consumption, local weather and energy consumption data should be tracked more closely and incorporated so that the model can be expanded to more locations. In places where the data is already available, the model should be used to augment existing models for maximum accuracy in prediction and optimization of production requirements. The final prediction model should be used to create an optimization model for utility companies to apply to production.

## Sources
### Static Data:
### Historical Energy Data: https://statics.teams.cdn.office.net/evergreen-assets/safelinks/1/atp-safelinks.html](https://catalog.data.gov/dataset/utility-energy-registry-monthly-zip-code-energy-use-beginning-2016
### Historical Weather Data: https://www.climate.gov/maps-data/dataset/past-weather-zip-code-data-table

### Live Data
### Weather API: [https://api.weatherapi.com/v1/current.json?key=7c8218f18550417496b43123242902&q={area}](https://api.weatherapi.com/v1/current.json?key=7c8218f18550417496b43123242902&q=13354)

### Competing Models (Cell phone data)
### https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-016-0075-3#:~:text=An%20accurate%20prediction%20of%20energy,allowing%20an%20efficient%20energy%20storage.

##Project Resources: 
###•	Github Repository Link: https://github.com/jhalsey87/BigData_Capstone824/tree/main 
###•	Lookerstudio Dashboard: https://lookerstudio.google.com/u/0/reporting/00b216a9-b9e3-4ba4-a8a1-739f389aefa4/page/KAd8D 
##Methodologies 
###•	Data Integration: Combined historical weather and energy consumption data with real-time weather information via a live API. 
###•	Correlation Analysis: Assessed the relationship between temperature and energy consumption to identify actionable patterns. 
###•	Predictive Modeling: Developed a proof-of-concept model to project energy consumption based on live weather inputs, serving as a foundation for enhancing future prediction accuracy. 

## GCP Components Used
### Big Query
### Looker (Formerly Data Studio)
### Cloud Pub/Sub
### Cloud Storage
### Cloud Functions
### Gemini

