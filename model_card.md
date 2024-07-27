# Model Card

## Model Description

**Input:** Because it a time series regression problem, input is 
    X: time_sec, Fourier terms, Week Day

**Output:** Output 
    y: count(pickups)

**Model Architecture:** 

 I used Fast Fourier Transform Forecasting Modeling. More info in notebooks with plots 

## Performance

 	Because it is a time series regression problem, we select Mean Absolute Percentage Error (MAPE) but other
    metrics were calculated too

## Limitations

  In time series regression problem we can not add more feature such as cost, drop location etc
  Data transformed in a interval time window of 1 hour in order to calculate frequencies. In this hour there
  are many taxi trips with different cost, drop location etc. It is one to many relation.

## Trade-offs

 I don't see any change in perfomance by selecting diferent number of harmonics
 
