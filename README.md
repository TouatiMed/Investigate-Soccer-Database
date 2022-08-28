# Investigate-Soccer-Database
This project was part of the Professional Data Analyst degree by Udacity.
In this project, [European Soccer Database](https://www.kaggle.com/datasets/hugomathien/soccer) was selected to be investigated
This soccer database comes from Kaggle and is well suited for data analysis and machine learning. It contains data for soccer matches, players, and teams from several European countries from 2008 to 2016. This dataset is quite extensive.

## Question(s) for Analysis
- Which teams are the top performers overall from 2008 to 2016?
- Which league had the most goals scored per season?
- Is there any advantage in playing matches at home?
- which teams are the top performers at home and in away matches?
- Which teams had the most wins in a single season?
- Which teams improved the most over the time period?
- What are the attributes of the top teams?
- what are the attributes of the top players in 2016? and Does age play a factor in that?

## Data Cleaning
In this Section we did the following:
- Merged the df_League and df_Country dataframes so we know which league belongs to which country.
- Deleted unnecessary columns in df_Match
- Created df_Match_sub a sub dataframe with the columns we are interested
- Fixed some datatypes like date and birthday
- Merged df_Match_sub with df_Team so we can see the name of the teams in every row, so we can understand who is playing at home or away, and who is the winner
- Merged it also with df_League so we can see to which league every match belongs to
- Added to 'total_goals' column to df_Match_sub
- Added 'winner' and 'loser' columns to df_Match_sub with the name of the teams to make it easier for exploring later
- Merged df_Team_Attributes with df_Team so we can get the name of the teams in rows, better then dealing with API IDs
- Merged df_Player_Attributes with df_Player in the same manner so we know each row of stats belongs to which player by getting their name in a new column
- Checked for any missing or duplicated data through all dataframes and we dealed with them.

