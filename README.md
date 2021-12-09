# KDD_Group8
# US-Accidents Data Analysis
# Team Members:
* Ivy Pham
* Joseph Antony Bala Vineesh Reddy Pentareddy
* Poornima Pulakandam
* Srujana Patil

# Team Name: Group 8

# Introduction to Problem: 
The US-Accidents dataset can be used for various applications such as real-time car accident prediction, to determine car accidents prone locations, accident analysis and deriving cause and effect rules to predict car accidents, and studying the impact of weather or other environmental stimuli on accident occurrence. we are working on a dataset of countrywide car accidents, covers 49 states of the USA. The dataset represents data of accidents from February 2016 to Dec 2020, using multiple APIs that provide streaming traffic incident (or event) data. We can analyze the The most recent release of the dataset can also be useful to study the impact of COVID-19 on traffic behavior and accidents.

US Accident Dataset has a few variables which are categorical  mention about the road condition or any object that was present on the accident scene or where exactly the accident occurred and the time of day. The  other variables are quantitative which mention about how the weather is impacting the accident occurence, such as wind or precipitation. Severity, as a response variable which describes the severity of the accident. Severity assigns a value from 1 to 4 to on how much impact the accident had on traffic with 4 being the most amount of interference and 1 being least amount of interference.

# Domain Data Description:
# Source: https://www.kaggle.com/sobhanmoosavi/us-accidents
* ID - This is a unique identifier of the accident record.
* Severity - Shows the severity of the accident, a number between 1 and 4, where 1 indicates the least impact on traffic (i.e., short delay as a result of the accident) and 4 indicates a significant impact on traffic (i.e., long delay).
* Start_Time - Shows start time of the accident in local time zone.
* End_Time - Shows end time of the accident in local time zone.
* Distance(mi) - The length of the road extent affected by the accident.
* City - Shows the city in address field.
* County -Shows the county in address field.
* State - Shows the state in address field.
* Zipcode - Shows the zipcode in address field.
* Country - Shows the country in address field.
* Timezone - Shows timezone based on the location of the accident (eastern, central, etc.).
* Weather_Timestamp - Shows the time-stamp of weather observation record (in local time).
* Temperature(F) - Shows the temperature (in Fahrenheit).
* Wind_Chill(F) - Shows the wind chill (in Fahrenheit).
* Humidity(%) - Shows the humidity (in percentage).
* Pressure(in) - Shows the air pressure (in inches).
* Wind_Direction - Shows wind direction.
* Wind_Speed(mph) - Shows wind speed (in miles per hour).
* Precipitation(in) - Shows precipitation amount in inches, if there is any.
* Weather_Condition - Shows the weather condition (rain, snow, thunderstorm, fog, etc.).

# Data Pre-Processing:
In the Data Preprocessing step, data cleaning is done by handling missing data in rows and columns. we handled the missing data by dropping it.
The feature Country has only one entry i.e USA, it is obvious since we are dealing with the USA’s dataset. so we will be deleting the feature Country.
The feature Turning_Loop has only one value — False. the feature actually means that no accidents were occured in the turning loops

# Data Understanding and Exploratory Data Analysis:
## Data Understanding from above Graphs
* Most of the US Accidents i.e 0.8 have the severity 2 and followed by severity 4.
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/Severity%20Plot.PNG"/>
* Major percentage of  the US Accidents  are occured at traffic signals, Crossing, Station, Stop and Amenity. The least percentage of  accidents are occured at Bump,           Roundabout, Railway, No-Exit, Junction
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/Accidents.png"/>
* Most percentage of accidents are occured in California followed by florida.
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/statewise%20accidents.png"/>
* Accidents are occurred in clear weather conditions(52.9%) and followed by cloudy weather 18.7% which means that weather conditions effects very less.
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/effect%20of%20Weather%20conditions.png"/>
* Weekday Accidents are higher in number compared to weekends.
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/Weekdays%20vs%20Weekends.png"/>
* Top 20 Accidents Duration in USA in minutes.
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/Top%2020%20Accidents.png"/>
* California is the place where highest number of accidents.
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/Accident%20Analysis%20in%20California.png"/>
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/California%20Aciidents.png"/>
* Accident Prone states in USA 
  <img src="https://github.com/Poornima764/KDD_Group8/blob/main/Images%20Folder/newplot.png"/>
  
# Data Preparation for Modelling:
We have splitted the data based on the Severity feature of the dataset. we have trained and tested the data after splitting the dataset.

# Data Modelling:
The models are implemented on the preprocessed dataset include the following:
  * K-Nearest Neighbour
  * Logistic Regression
  * Decision Tree
 
#  Evaluation Methods:
  * Accuracy Score
  * Precision Recall
  * Cross Validation Score
# Conclusion:
1) What was unique about the data?  Did you have to deal with imbalance? What data cleaning did you do? Outlier treatment?  Imputation?
2) Did you create any new additional features / variables?
3) What was the process you used for evaluation? What was the best result?
    Process used for evaluation includes modeling using logistic regression K- nearest neighbours classification and decision tree classification.  Best results belong to decision tree classification 
4) What were the problems you faced? How did you solve them?
    Problems faced included some data not being in a good form for modeling and we needed to delete some of the data in order to create the models properly
5) What future work would you like to do? 
    * Analyze year-on-year trends of accidents.
    * Explore per-capita accident figures by adding a state and city-wise population data set.
    * The question of missing data in certain months could be analyzed if there is some data available on the source/s of this one.
6) Instructions for individuals that may want to use your work?
    
# Research Questions:
1. Research on how weather condition  impacts on the accident occurence and time affect visibility which results in the number of accidents?
2. Is the accident rates in different states higher due to different Weather Condition?
3. How wind speed and wind direction contribute to accidents?
4. What are the most accident prone states in USA?
5. Number of accidents of a state as compared to its adjacent states?
6. Factors that effect accident severity.
# Future Work:
* Analyze year-on-year trends of accidents.
* Explore per-capita accident figures by adding a state and city-wise population data set.
* The question of missing data in certain months could be analyzed if there is some data available on the source/s of this one.
