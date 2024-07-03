# Introduction
###
Climate change is a global challenge that has become increasingly urgent to address. Greenhouse gas emissions, primarily carbon dioxide (CO2), are the main contributors to global warming and climate change (Shi, 2018). According to the Intergovernmental Panel on Climate Change (IPCC), the global average temperature has increased by 1.1oC since pre-industrial times, and it is projected to continue to increase in the coming decades if emissions continue to rise at the current rate (IPCC, 2021).
One way to address this challenge is to reduce greenhouse gas emissions. To achieve this, it is important to understand the sources and drivers of emissions, as well as the factors that influence them.
## Statement of the Promblem 
###
The most recent past decade, which includes year 2011 through year 2020 was observed to be the hottest decade. With current trends, global temperatures are expected to rise by another 1.5oC between 2030 and 2052, which would lead to more frequent and severe climate-related disasters (IPCC, 2021). 
Given the significant impacts of climate change, it is essential to monitor its effects in order to understand the scope of the problem and develop effective solutions
## Historical emission prediction approaches
###
The Forecasting of transportation-related energy demand and CO2 emissions in Turkey with different machine learning algorithms by Umit Agbulut, and Machine learning based time series models for effective CO2 emission prediction in India by Surbhi Kumari and Suni Kumar Singh are similar co2 prediction studies. 
Kumari and Singh used three statistical models which were the autoregressive-integrated moving average (ARIMA) model, the seasonal autoregressive-integrated moving average with exogenous factors (SARIMAX) model, and the Holt-Winters model, and two machine learning models, i.e., linear regression and random forest model and a deep learning based long short-term memory (LSTM) model. Agbulut used Deep Learning (DL), Support Vector Machine (SVM) and Artificial Neural Networks (ANN). 
An exploration of clustering and classification machine learning algorithms will inform new ideas and aid the creation of predictive models.
## Aims and Objectives
###
The main aim of this project is to identify the causes of the country-level emission patterns and build solutions that can better forecast expected emission trends. This will aid with policy-making and decision taking. 
Build predictive models to forecast future emissions trends by location.
Analyze the changes in emissions across different countries.  
Present an analysis of emission trends by types (e.g., CO2, CH4, or N2O etc).
Developing an understanding of the detrimental effect of the different types of emissions based on predictions for the next 10 years. 
## Research Questions
###
- How can machine learning models be effectively used to forecast future emissions trends?
- What emission disparity can be observed amongst different countries?
- How do different emission types (e.g., CO2, CH4, or N2O etc) vary across countries, and what factors contribute most to these differences? 
- How can we explain the detrimental effect of the different types of emissions based on predictions for the next 10 years?
## Methodology
###
The model's accuracy was assessed by utilizing it to forecast the final three years of data in the test set and calculating the root mean squared error (RMSE) between the test set and the model's predictions.
The VARMAX model was trained using VAR and VMA order values of 'p' and 'd.' To identify the most optimal model, hyperparameter tuning was conducted by training various VARMAX models with different 'p' and 'd' values, resulting in the model with the lowest RMSE score for all three Elements being predicted. 
It was concluded that if the model's RMSE is less than 10% of the mean emission value for that Element, then the model is deemed acceptable.##
## Performance Evaluation Metrics
###
The model's accuracy was assessed by utilizing it to forecast the final three years of data in the test set and calculating the root mean squared error (RMSE) between the test set and the model's predictions.
The RMSE measures the differences between the predicted values and the real, existing values that are present in the dataset. It is calculated by taking the square root of the average of the squared differences between the predicted values and the actual values (Hodson, 2022). 
![image](https://github.com/inioluwa279/Predict-Emission-using-Machine-Learning-/assets/133115794/771dbfe3-e413-4bb4-8aa6-1799c901fb82)
# Data Analysis, Prediction Model and Results 
## Data Availability 
###
A dataset was identified and downloaded from the site “Kaggle.com”. This dataset tracks emission source, emission type, and total emissions (e.g., CO2, CH4, or N2O etc.) of greenhouse gasses.
. The main source of information relied upon was the website of the Food and Agriculture Organization (FAO) of the United Nations
Given the careful recording of official statistics by this legally established intergovernmental organization, there is no other entity that is better positioned to offer valuable information on emission levels, about over 200 countries from 2000 to 2020, over 7670 days.
## Dataset Description
###
The "Total Emissions Per Country (2000-2020)" dataset on Kaggle is a collection of data on the total amount of greenhouse gas emissions produced by each country between the years 2000 and 2020. The dataset includes information on carbon dioxide (CO2), methane (CH4), and nitrous oxide (N2O) emissions, as well as the total greenhouse gas emissions. It contains 25 attributes and 58765 records.
## Statistical Test 
###
Augmented Dickey-Fuller test was performed on each Element of the dataset to verify that the mean and standard deviation of the data remained constant over time. The results of the test indicated that the data was non-stationary over time
Granger Causality test was conducted on the dataset to investigate whether any causal relationships exist between different emissions. 
## Train-Test Spilt 
###
The data was split into train and test sets with the first 18 years of data for training and the last 3 years for training
# Emission Patterns in Countries 
###
Seven countries were picked based on the World Economic Situation and Prospects report by the United Nations. Three countries were picked from the developed economies, two were picked from the economies in transition and two were picked from developing economies. 
The picked countries were Spain, Japan, United States, Belarus, Ukraine, Nigeria, Colombia
## United States
### 
The COVID-19 pandemic has had a significant impact on the emission levels of greenhouse gases in the United States. CH4 emissions, which had been consistently high since the early 2000s, experienced a marked decline in the 2010s. CO2 emissions, which also started at high levels, showed a general trend of decline, but experienced a significant decrease in 2020 due to the pandemic. Nitrous oxide (N2O) emissions, on the other hand, exhibited a low and fluctuating pattern, but also experienced a reduction in 2020
![image](https://github.com/inioluwa279/Predict-Emission-using-Machine-Learning-/assets/133115794/66d484e1-4b3c-40e8-b13a-ffa177210182)

## Spain
###
CO2 has been found to be the most prevalent greenhouse gas emission across many countries. As illustrated in Figure 4.1, the peak of carbon dioxide emissions occurred in 2007, and there has been a downward trend since then. Similarly, CH4 emissions have also been decreasing over time, but since 2012, there has been an observed increase. N2O emissions have also followed a comparable pattern with that of CH4, but at a relatively lower magnitude.
![image](https://github.com/inioluwa279/Predict-Emission-using-Machine-Learning-/assets/133115794/903e7093-e275-461b-adaf-59061ea8c5f7)
## Japan
###
There has been a declining trend in the emissions of methane (CH4) and nitrous oxide (N2O) in Japan. However, the emission of carbon dioxide (CO2) decreased in 2009, followed by an increase up to its peak in 2013, and has since been gradually decreasing.
![image](https://github.com/inioluwa279/Predict-Emission-using-Machine-Learning-/assets/133115794/5953d848-0afc-46a5-a498-8deaeaa731fa)
## Conclusion
###
The empirical findings indicate that developed countries exhibit higher overall emissions when compared to developing countries or economies in transition. This disparity in emissions levels highlights the unequal distribution of environmental impact between different regions and economies. 
Emissions in developing countries are projected to exhibit a modest increase or maintain relative stability, whereas other countries are anticipated to undergo substantial shifts in their emission levels. However, it is noteworthy that Nigeria, in contrast to these global trends, is predicted to experience a relatively stable trajectory in terms of emissions.
The United States which was recorded to have the highest emission rates across all three emissions was still predicted to maintain the lead, via a huge margin in 2030. Although some work is being put in to mitigate the effects of climate change in the United States such as broad-based climate policies, policies on transportation systems, and policies on the use of electricity which affects climate change





