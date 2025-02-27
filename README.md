
# Ultimate Inc. take home Challenge
________
## Description and Problem statement


**Part 1 ‐ Exploratory data analysis**

The attached  _logins.json_  file contains (simulated) timestamps of user logins in a particular geographic location. Aggregate these login counts based on 15-minute time intervals, and visualize and describe the resulting time series of login counts in ways that best characterize the underlying patterns of the demand. Please report/illustrate important features of the demand, such as daily cycles. If there are data quality issues, please report them.

**Part 2 ‐ Experiment and metrics design**

The neighboring cities of Gotham and Metropolis have complementary circadian rhythms: on weekdays, Ultimate Gotham is most active at night, and Ultimate Metropolis is most active during the day. On weekends, there is reasonable activity in both cities.

However, a toll bridge, with a two-way toll, between the two cities causes driver partners to tend to be exclusive to each city. The Ultimate managers of city operations for the two cities have proposed an experiment to encourage driver partners to be available in both cities, by reimbursing all toll costs.

1.  What would you choose as the key measure of success of this experiment in encouraging driver partners to serve both cities, and why would you choose this metric?
2.  Describe a practical experiment you would design to compare the effectiveness of the proposed change in relation to the key measure of success. Please provide details on:  
    a. how you will implement the experiment  
    b. what statistical test(s) you will conduct to verify the significance of the observation  
    c. how you would interpret the results and provide recommendations to the city operations team along with any caveats.

**Part 3 ‐ Predictive modeling**

Ultimate is interested in predicting rider retention. To help explore this question, we have provided a sample dataset of a cohort of users who signed up for an Ultimate account in January 2014. The data was pulled several months later; we consider a user retained if they were “active” (i.e. took a trip) in the preceding 30 days.

We would like you to use this data set to help understand what factors are the best predictors for retention, and offer suggestions to operationalize those insights to help Ultimate.

The data is in the attached file  _ultimate_data_challenge.json_. See below for a detailed description of the dataset. Please include any code you wrote for the analysis and delete the dataset when you have finished with the challenge.

1.  Perform any cleaning, exploratory analysis, and/or visualizations to use the provided data for this analysis (a few sentences/plots describing your approach will suffice). What fraction of the observed users were retained?
2.  Build a predictive model to help Ultimate determine whether or not a user will be active in their 6th month on the system. Discuss why you chose your approach, what alternatives you considered, and any concerns you have. How valid is your model? Include any key indicators of model performance.
3.  Briefly discuss how Ultimate might leverage the insights gained from the model to improve its long-term rider retention (again, a few sentences will suffice).

Data description

●  **city**: city this user signed up in  
●  **phone**: primary device for this user  
●  **signup_date**: date of account registration; in the form ‘YYYY MM DD’  
●  **last_trip_date**: the last time this user completed a trip; in the form ‘YYYY MM DD’  
●  **avg_dist**: the average distance in miles per trip taken in the first 30 days after signup  
●  **avg_rating_by_driver**: the rider’s average rating over all of their trips  
●  **avg_rating_of_driver**: the rider’s average rating of their drivers over all of their trips  
●  **surge_pct**: the percent of trips taken with surge multiplier > 1  
●  **avg_surge**: the average surge multiplier over all of this user’s trips  
●  **trips_in_first_30_days**: the number of trips this user took in the first 30 days after signing up  
●  **ultimate_black_user**: TRUE if the user took an Ultimate Black in their first 30 days; FALSE otherwise  
●  **weekday_pct**: the percent of the user’s trips occurring during a weekday
_________



_______
# RELAX CHALLENGE
_______________________________

## Description and Problem statement

The data is available as two attached CSV files:
*takehome_user_engagement. csv*
*takehome_users . csv*<br/>
The data has the following two tables:
1. A user table ( "takehome_users" ) with data on 12,000 users who signed up for the
product in the last two years. This table includes:
● name: the user's name<br/>
● object_id: the user's id<br/>
● email: email address<br/>
● creation_source: how their account was created. This takes on one
of 5 values:<br/>
○ PERSONAL_PROJECTS: invited to join another user's
personal workspace<br/>
○ GUEST_INVITE: invited to an organization as a guest
(limited permissions)<br/>
○ ORG_INVITE: invited to an organization (as a full member)
○ SIGNUP: signed up via the website<br/>
○ SIGNUP_GOOGLE_AUTH: signed up using Google
Authentication (using a Google email account for their login
id)<br/>

● *creation_time:* when they created their account<br/>
● *last_session_creation_time*: unix timestamp of last login<br/>
● *opted_in_to_mailing_list:* whether they have opted into receiving
marketing emails<br/>
● *enabled_for_marketing_drip:* whether they are on the regular
marketing email drip<br/>
● *org_id:* the organization (group of users) they belong to<br/>
● *invited_by_user_id:* which user invited them to join (if applicable).<br/>

2.  A usage summary table ( "takehome_user_engagement" ) that has a row for each day
that a user logged into the product.<br/>

Defining an "adopted user" as a user who has logged into the product on three separate days in at least one seven ­day period , identify which factors predict future user adoption .<br/>

Please send us a brief writeup of your findings (the more concise, the better ­­ no more than one page), along with any summary tables, graphs, code, or queries that can help us understand your approach. Please note any factors you considered or investigation you did, even if they did not pan out. Feel free to identify any further research or data you think would be valuable