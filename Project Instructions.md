# Data Engineer Associate Exam - Virtual Reality Fitness

ActiVR provides a virtual reality device designed for exercise and fitness.

ActiVR offers a range of products, including VR devices and subscription-based fitness programs through their apps.

The sales team at ActiVR wants to analyze user data to enhance their marketing strategy and evaluate their products. For this, it is crucial that the data is clean, accurate, and available for reporting.

They need your assistance in preparing the data before launching a new promotional campaign.

Database Schema

The data schema for ActiVR's database is outlined as follows:

-  **events**: Contains records of events registered in different games.
-  **games**: Stores information about various games available on the platform.
-  **devices**: Holds data about the virtual reality devices used by the users.
-  **users**: Contains details about the users utilizing the ActiVR platform.  

![image](https://github.com/user-attachments/assets/ddf4f568-61a7-4928-92c9-e92132f8b423)


## Task 1
ActiVR's sales team wants to use the information it has about users for targeted marketing.

However, they suspect that the data may need to be cleaned before.

The expected data format and types for the users table according to the sales team's requirements is shown in the table below.

Write an SQL query that returns the users table with the specified format, including identifying and cleaning all invalid values.

Your output should be a DataFrame with the name 'clean_data'. Do not modify the users table.
Note that the DataLab environment formats dates as YYYY-MM-DD-hh-ss-SSS.  

![image](https://github.com/user-attachments/assets/982ac30e-df47-44b0-a68f-be665ac934f8)  


## Task 2
It seems like there are missing values in the events table for the column game_id for all events before the year 2021.

However, we know that before 2021 there were only games where the game_type is running. The game_id for these games can be found in the games table.

Write a query so that the events table has a game_id for all events including those before 2021.

Your output should be a DataFrame with the name 'events_with_game_id'. Do not modify the events table.


## Task 3
ActiVR's sales team plans to launch a promotion for upgrades to virtual reality devices.

They aim to target customers who have participated in events related to specific game types.

Write a SQL query to provide the user_id and event_time for users who have participated in events related to biking games. Your output should be a DataFrame with the name 'event_biking'.


## Task 4
After running their promotion, the sales team at ActiVR wants to investigate the results.

To do so, they require insights into the number of users who participated in events for each game_type.

Write a SQL query that returns the count of unique users for each game type game_type and game_id. The user count should be shown in a column user_count. Your output should be a DataFrame with the name 'users_game'.
