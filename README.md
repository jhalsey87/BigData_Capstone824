# BigData_Capstone824

## This a team capstone submission for Purude University MGMT 59000 AI Assisted Big Data in the Cloud
### The intention is to combine at least one (in this case 2) Archived (herein referred to as static) data sets with one live API to analyze energy consumption patterns.

### We are attempting to analyze historical weather data and energy consumption data in order to correlate consumption with temperature in a given location (Trenton Falls, NY). 

#Business case - very little of the existing energy infrastruture is built to store energy, meaning there is cost to both the over and under production of energy. To facilitate the building of a future optimation model, we've built a proof-of-concecpt prediction model for energy consumption requirements. 

### Using our analysis, we attempt to use live weather data for zip codes in Trenton Falls, NY to estimate the likely energy consumption in the current month. We believe that this will allow energy producers to more accurately project required production and adjust production volumes accordingly. While temperature is not the only factor in determining usage, many other prediction models, such as predictions based on cell phone usage, are not able to be adjusted by seasonal factors, causing them to become unreliable certain weather conditions. We believe our model could be used to augment other models in the future, addresssing the limitations of both models.

##Limitations of our model: Not all states track energy consumption at the local level and not all weather stations record temperature data in publicly available data sets. While our model can be used to predict energy consumption for localities that track both data points, the correlation will likely differ depending on location. New York, being a northern climate requires more energy in winter for heat, but has relatively mild summers, requiring much less energy to cool. This produces a strong, negative correlation between temperature and energy consumption. Warmer climates, such as Florida, or Nevada, may find the opposite correlation due to the need to cool in summer while having minimal needs to heat in their relativly mild winters. 

##Reccomendations: In order to improve prediction of consumption, local weather and energy consumption data should be tracked more closely and incorporated in data models. In places where the data is already available, it should be applied to existing models for maximum accuracy in prediction and optimation of production. 
