# NYC Trip Time Prediction Project

The Taxi and Limousine Commission (TLC), established in 1971, is in charge of licencing and regulating New York City's Medallion (Yellow) taxi cabs, for-hire vehicles (community-based liveries, black cars, and luxury limousines), commuter vans, and paratransit vehicles.Every day, approximately 1,000,000 trips are completed by over 200,000 TLC licensees. Drivers who work for hire must first pass a background check, have a clean driving record, and complete 24 hours of driver training. TLC-licensed vehicles are inspected at TLC's Woodside Inspection Facility for safety and emissions.

The dataset is based on data from the 2016 NYC Yellow Cab trip records, which were made available in Big Query on Google Cloud Platform. The NYC Taxi and Limousine Commission first made the data public (TLC). For the purposes of this project, the data was sampled and cleaned. We should predict the duration of each trip in the test set based on individual trip attributes.


## Problem Statement
To build a model that predicts the total ride duration of taxi trips in New York City. Primary dataset is one released by the NYC Taxi and Limousine Commission, which includes pickup time, geo-coordinates, number of passengers, and several other variables.



## Authors

- [@Aman Guleria](https://www.github.com/AMAN-GULERIA)
- [@Saurabh Aradwad](https://www.github.com/SaurabhAradwad)
- [@Ayush Sharma](https://www.github.com/SharmaAyush98)
- [@Rishika Rai](https://www.github.com/Rishika70)


## Referance Project Document

- [Project Report](https://docs.google.com/document/d/1ko1L1wk3wFxsTLKgyzw0zTCCzi_zp46PxTGzwX6Qprw/edit?usp=sharing)
- [Project Summary](https://docs.google.com/document/d/1jomVw-hpvA4csJukC2lO858OZYfMp9SlZEoe35Hwf48/edit?usp=sharing)
- [Colab Notebook ✔](https://colab.research.google.com/drive/1pB-XRubyeVNO7TVMQBkLblyCv0jusZTI?usp=sharing)
- [Presentation PPt](https://docs.google.com/presentation/d/1t2hYKW9KQfNod7BUhn0lgJkMxOIIF21cvwURahLtZ3Q/edit?usp=sharing)

## Data Summary

All columns and type of information stored in the csv file is as follows

- *Id* -unique id in the dataset
- *vendor_id* - a code indicating the provider associated    with  the trip record
- *pickup_datetime* - date and time when the metre was engaged
- *dropoff_datetime* - date and time when the metre was disengaged
- *passenger_count* - the number of passengers in the vehicle (driver entered value)
- *pickup_longitude* - the longitude where the metre was engaged
- *pickup_latitude* - the latitude where the metre was engaged
- *dropoff_longitude* - the longitude where the metre was disengaged
- *dropoff_latitude* - the latitude where the metre was  disengaged
- *store_and_fwd_flag* - This flag indicates whether the trip record was  held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server (Y=store and forward; N=not a store and forward trip)
- *trip_duration* - duration of the trip in seconds



## Conclusions

- LGBM models have the highest accuracy of 93% when compared to other models.
- The least accurate solutions for this problem are linear, lasso, and ridge regulation.
- Gradient Boost took a moderate time of 8 minutes and 7 seconds, while LGBM took the shortest time of
- LGBM's low learning rate increases accuracy while decreasing percentage error.
- If we want to reduce the training time of our model, we can use hyperparameter tuning to select tuned parameters. It will produce similar results in much less time.
- Logarithm treatment of trip duration is important, due to skewed data.
- Speed and distance calculation. We can confirm this with correlation heatmap and skewed.
- This trip duration prediction project is important for many cab service providers such as ola, uber etc. It helps them to improve their customer experience by showing expected trip duration time and arrival time. 
- It will be helpful if you select a certain time from the day and select pickup and dropoff coordinates for your future trips and get a prediction for trip duration. 

