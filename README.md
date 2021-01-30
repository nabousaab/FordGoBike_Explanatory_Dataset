# Explanatory_Dataset
## I have chosen to work on the FordGoBike dataset. 
## And for this reason I will need to upload the data into Jupytor notebook to start exploration and explanation process.

## Oridiginal dataset [fordgobike](http://localhost:8891/edit/201902-fordgobike-tripdata.csv)

# Gathering Dataset
## Software to import and use.

```

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sb

```

# Cleaning the Dataset:
## Quality and tidiness issues
 - We have a lot of empty rows that I do recommend to drop them
 - We should also drop the columns that have no value to our exploratory and explanatory plotting.
 
 
## How does the Dataset Structure ?
- The data we are evaluating is for FordGoBike 2019, 
- We have cleaned the data and saved it under a new folder called bikes_clean.
- bikes_clean dataset constitue of 174952 rows , and 10 columns.


## What are the main features we will investigate in our exploratory plotting?
- Duration of each trip, customer type, gender, birthday, days of the week


## What type of features will be used to create univariate and multivariate plots for both exploratory and explanatory purposes?

- Category data related to days, gender, top 15 station names
- Numerical data that is mainly the colum related with duration of each trip


# Summary:

### The 2019 fordgobike-tripdata requires some cleanning process to make sure that we receive the quality and tidiness contorl for the data before going into the exploratory visualization.
 - The dataset contained 183412 rows, and 16 columns 
 - The only numeric continuous data was for the duration per sec 
 - Rest of the data are more of nominal or categorical data
 - The data also included some empty rows information from 
 
 ### The cleanning process:
  - We have removed all empty raws
  - We've removed some columns to create more tidy information for our analysis, the dropped columns were 'start_station_latitude', 'start_station_longitude', 'end_station_latitude', 'end_station_longitude', 'start_station_id','end_station_id', 'bike_id'.
  - We have added one columns representing the days of the week

### _the cleaned dataset was called bikes_sub_
  



# Conclusion:

- Most of the bike service usage are for preiods less than half an hour.
- The Majorty of deuration, after processing a log type transformation, proves to fall between 8 and 10 min of use.

- Males dominates 70% of all users
- And sunscribers represent 89% from all users

- Weekends seams to be stagnant across the category of member type and and gender with duration_sec relationsship
- Women tends to use more sec comapred to men, this have not changes when measuring different categorical relationship with time and gender.

- The most intersting visual discuover, was the trend covering Subscribers when using the mean average for the line relatiosnhip with time accross days of the week. 
    - This trend shows a complete straight line across all days and at same value for each connecting point
    - There was minor change, cannot be witnessed, over the weekend through.



# Additional suggestions:
 - To improve future predictions, we can do an indepth analysis by age of users. This will help improve AI predection and understand more the other valriance impact on usage and duration of use. 
 - Include more information on the distance covered, We can measure this later on by user type and gender
 - Do more analysis on the time of usage and check if their is any variance through other categories relations with each other
  
