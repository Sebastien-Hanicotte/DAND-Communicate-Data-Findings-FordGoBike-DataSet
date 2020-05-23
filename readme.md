# eXploration of the Ford GoBike DataSet
## by Sebastien Hanicotte



## Technical Stack

This project use some libraries which are not by default installed

You'll certainly have to install those librairies first before trying to launch this project

conda install basemap basemap-data-hires

Don't forget to relaunch your Jupyter instance before running this notebook

You'll also find below all the libraries I used for this project : 
- requests
- os
- io import BytesIO
- zipfile import ZipFile
- pandas
- numpy
- matplotlib
- seaborn
- datetime
- math
- calendar
- warnings
- glob
- mpl_toolkits.basemap
- IPython.display


## Dataset

For this last project, I chose to go with the Ford GoBike dataset.

FordGoBike (aka Bay Wheels) is a regional public bicycle sharing system in the San Francisco Bay Area, California. They gracefully share a lot of their use data through a specific Data License Agreement (https://baywheels-assets.s3.amazonaws.com/data-license-agreement.html).

Ford GoBike dataset changed a little during those years, but here you'll find data available through all the datasets :
- duration_sec
- start_time
- end_time
- start_station_id
- start_station_name
- start_station_latitude
- start_station_longitude
- end_station_id
- end_station_name
- end_station_latitude
- end_station_longitude
- bike_id
- user_type
- member_birth_year
- member_gender
- bike_share_for_all_trip
- rental_access_method

All those datas were stored into CSV file, so while doing some preparation of data, I had to update column types

Some of those datas were incomplete or needed to be exploded in more specific form (like datetime exploded in years, months, days, day of week, ...) to accelerate the rendering of the graphs

## Summary of Findings

I did a lot of analysis but here are all discover I made during this process : 
- Users of the service are between 18 and 58 (with the most of them between 28 and 40)
- Subscribers are doing the most of the rides versus Customers which are doing longest trips (in seconds)
- Men are doing the most of the rides versus Women and Others which are doing longest trips (in seconds)
- During warm days (between Spring and Automn) are done the most of the rides with peaks during March and October for 2018
- This service seems to be used by subscribers to go forth and back to work, therefore service is mainly used between Monday and Friday. No particular day is noticeable for customers.
- At 8AM and 5PM is recorded the most rides of the day
- Most trips are during between 2 to 12 minute
- Finaly, there seems not to have real difference of number of trips when grouped by age during through time (months period)


## Key Insights for Presentation

- Either Women and Other seems to have longest trip duration, this difference is not huge comparing of trip done by men (I was expecting the difference to be inverse and more strong)
- Youngest people are not the one who does the longest trips, those are more the people in 30-39 age group. (Service is available since 18 years old)
- No difference through time between groups of age and number of trips

