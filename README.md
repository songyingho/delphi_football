# Delphi Football Analysis

Executive Summary: Analyzing individual team performances in Bundesliga for the 2011 season and investigate the team performance when matches were played during rain.

Using the dataset given, we accomplished the following:
1. Final dataset consisting of:
*  - Team Name
*  - Total Goals Scored by Team
*  - Total Wins Acquired by Team
*  - Win Percentage by Team during rain days
2. Histogram Visualization dsplaying the number of wins and losses by each team
3. Two classes created for the project (SQL & MongoDB)
4. Integrated weather information into our project via DarkSky API
5. Imported final dataset to MongoDB

Methodology: This project uses Python 3, documented with Jupyter Notebook. We used a combination of SQL and Pandas for data cleaning, filtering and querying. DarkSky API was used to evaluate past weather during matchday. Finally, MongoDB was used for data storage.

High Level Overview: The project started by finding relevant information from the database given, SQL was mainly used to filter the data and summarizing new statistics that were not given from the original table, we obtained the team name, along with the goals and wins associated with the team. Next, we used weather information from the DarkSky API and use the data to evaluate team performance during rainy matchdays. Finally, we imported the final dataset with the required information to our MongoDB database.

Limitations & Improvements:
1. Inaccurate weather data collection: - As we generalized the location of all matches to Berlin, Germany, it provides a poor representation of the presence of rain in the respective matches. A more accurate analysis can be conducted by gathering the exact coordinate of the football stadiums that the matches were played.
2. Limited amount of rain matches analyzed: - With only 146 rain matches in the sample, this is significantly low as we conducted analysis for 36 teams, hence this is just an average of 4 rain matches per team. We should conduct the same analysis for multiple seasons so that we can have a more statistically significant analysis for our rain matches.
3. API requests should be saved into a CSV file to prevent over-requesting from the DarkSky API, as only 1000 requests per day were allowed. This will be an issue when conducting analysis for multiple seasons.
