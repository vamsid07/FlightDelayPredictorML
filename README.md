# Two Stage Flight Delay Predictor

The objective of this project is to predict flight delays for 15 airports in the United States using a two-stage machine learning model. This model combines classification and regression techniques to provide comprehensive predictions. Initially, a binary classifier determines if a flight will be delayed by 15 minutes or more, using the target variable `Arrdel15`. Subsequently, for flights classified as delayed, a regression model predicts the exact delay duration in minutes, denoted by `ArrDelminutes`. 

The project involves extensive data acquisition and preprocessing of flight and weather information. The final **classifier** and **regressor** has an accuracy of **0.92** and **0.94** respectively.

The table below lists the airports for which weather data is available:

| ATL | CLT | DEN | DFW | EWR |
|-----|-----|-----|-----|-----|
| IAH | JFK | LAS | LAX | MCO |
| MIA | ORD | PHX | SEA | SFO |

**Table 1**: The airports for which weather data is available.
