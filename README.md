#COVID-19 

Context

A new coronavirus designated 2019-nCoV was first identified in Wuhan, the capital of China's Hubei province
People developed pneumonia without a clear cause and for which existing vaccines or treatments were not effective.
The virus has shown evidence of human-to-human transmission.
Transmission rate (rate of infection) appeared to escalate in mid-January 2020.
As of 30 January 2020, approximately 8,243 cases have been confirmed.

I will train a model using only a single feature (cases), and use it to make predictions for that value in the future.

Content

Each row contains report from each region/location for each day

Each column represents the number of cases reported from each country/region

Time series forecasting using Recurrent Neural Networks (RNNs).

A Recurrent Neural Network (RNN) is a type of neural network well-suited to time series data. 
RNNs process a time series step-by-step, maintaining an internal state summarizing the information they've seen so far.

I collected the link from a public GitHub link by the NYT. It is opened to the public. According to the authors, "The data is the product of dozens of journalists working across several time zones to monitor news conferences, analyze data releases and seek clarification from public officials on how they categorize cases". Located at:https://raw.githubusercontent.com/nytimes/covid-19-data/master/us-counties.csv
This dataset contains 6 different features such as date, county, state, fips, cases,deaths. These were collected every single day.

I wanted to calculate root mean squared error and error distribution.

The error metrics measure the predictive performance of a regression model in terms of the mean deviation of its predictions from the true values.
Lower error values mean the model is more accurate in making predictions. An overall error metric of zero means that the model fits the data perfectly.
The term "error" here represents the difference between the predicted value and the true value. 
The absolute value or the square of this difference is usually computed to capture the total magnitude of error across all instances, as the difference between the predicted and true value could be negative in some cases. 


