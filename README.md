
# Project Name: Capstone824
### Course: MGMT 59000 AI Assisted Big Data in the Cloud
### Purdue University Summer II 2024
### Team Name: Ninja_1

# Executive Summary: 

##Requirements:
### The intention is to combine at least one (in this case 2) Archived (herein referred to as static) data sets with one live API to analyze energy consumption patterns.

## Business case:
### Very little of the existing energy infrastruture is built to store energy, meaning there is cost to both the over and under production of energy. To facilitate the building of a future optimation model, we've built a proof-of-concecpt prediction model for energy consumption requirements for Trenton Falls, NY.

## Our Solution:
### By Analyzing historical weather data and historical energy consumption on a monthly basis, we attempt to use live weather data for zip codes in Trenton Falls, NY to estimate the likely energy consumption in the current month. We believe that this will allow energy producers to more accurately project required production and adjust production volumes accordingly. While temperature is not the only factor in determining usage, many other prediction models, such as predictions based on cell phone usage, are not able to be adjusted by seasonal factors, causing them to become unreliable certain weather conditions. We believe our model could be used to augment other models in the future, addresssing the limitations of both models.

## Limitations of our model: 
### Not all states track energy consumption at the local level and not all weather stations record temperature data in publicly available data sets. While our model can be used to predict energy consumption for localities that track both data points, the correlation will likely differ depending on location. New York, being a northern climate requires more energy in winter for heat, but has relatively mild summers, requiring much less energy to cool. This produces a strong, negative correlation between temperature and energy consumption. Warmer climates, such as Florida, or Nevada, may find the opposite correlation due to the need to cool in summer while having minimal needs to heat in their relativly mild winters. 

## Reccomendations: 
### In order to improve prediction of consumption, local weather and energy consumption data should be tracked more closely and incorporated in data models. In places where the data is already available, it should be applied to existing models for maximum accuracy in prediction and optimation of production. 

## Sources
### Static Data:
### https://statics.teams.cdn.office.net/evergreen-assets/safelinks/1/atp-safelinks.html](https://catalog.data.gov/dataset/utility-energy-registry-monthly-zip-code-energy-use-beginning-2016
### https://www.climate.gov/maps-data/dataset/past-weather-zip-code-data-table

### Live Data
### Weather API: [https://api.weatherapi.com/v1/current.json?key=7c8218f18550417496b43123242902&q={area}](https://api.weatherapi.com/v1/current.json?key=7c8218f18550417496b43123242902&q=13354)

### Competing Models (Cell phone data)
### https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-016-0075-3#:~:text=An%20accurate%20prediction%20of%20energy,allowing%20an%20efficient%20energy%20storage.
