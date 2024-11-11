# MIST-4610-Project
Group 9- Manchester City

Team Members JT Warren Charlie Mixson Cassandra Albright Divya Matthew

Scenario Description We are building our model for Manchester City to scout future potential opponents in the Champions League. We included real teams, players, and coaches from the Premier League, Bundesliga, La Liga, and the MLS. Our tables give Man City insight on the performance of other teams. Our model can track goals scored, wins, matches against common opponent, etc. Advanced statistics and data modeling has taken over the professional sports industry, and this a tiny example of what they do on a weekly basis

Data Model 

![image](https://github.com/user-attachments/assets/c5dfa140-4c9f-4dca-b667-f7bf909f1b19)

Entities: players player_id PK f_name l_name position nationality team_id FK from teams playerStats player_id PK, FK from Players goals assists passes tackles minutes_played teams team_id PK team_name city league wins draws losses coaches coach_id PK cf_name cl_name start_date team_id FK from teams assistant_coach_id FK from coaches matches match_id PK match_date match_time match_loc match_team_pairings team_id PK, FK from teams match_id PK, FK from matches matchStats team_id PK, FK from teams match_id PK, FK from matches shots_per_game pass_percentage fouls_per_game goals_scored result Our data model shows the relationships between Coachs, Players, Teams, and their statistics. We also included a relationships between coaches and their proteges. This can help Manchester City determine who to hire next based on which coach produces the best assistants. We can also track our opponents and their star players

Data Dictionary

![image](https://github.com/user-attachments/assets/ab65982f-dacd-4d4a-85f9-42f82c81b118)
![image](https://github.com/user-attachments/assets/da239650-8d67-4514-a9dd-58673e02500d)
![image](https://github.com/user-attachments/assets/8390331d-4d36-4545-96d3-1235145c8219)
![image](https://github.com/user-attachments/assets/4f0d31fa-0106-4d78-9fe3-686737f3e310)
![image](https://github.com/user-attachments/assets/73a23e71-ac92-4dd7-9c99-5829fd92ef89)
![image](https://github.com/user-attachments/assets/abb329c2-d062-46ed-a63c-3ab9e9d9565a)
![image](https://github.com/user-attachments/assets/6278f27e-d290-42e4-a9c1-5fcaa14b5f03)

Ten Queries

1. Identify the top 5 players with the most assists along with the teams they play for
![image](https://github.com/user-attachments/assets/45fb42af-60c5-44a5-a382-904562de16f1)


Identifying the top 5 players with the most assists and their respective teams is valuable for managers as it highlights key playmakers in the league, aiding in recruitment decisions, team strategy, and player valuations. Additionally, this data can be used for marketing purposes and to identify areas for player development, ultimately enhancing overall team performance and profitability.

2. Identify the top scorers from each club
![image](https://github.com/user-attachments/assets/e58271f1-40ea-4fb8-afdd-d93d44fce6d8)


Identifying the top scorers from each club helps managers understand which players are most effective at converting opportunities into goals, guiding decisions on player retention, recruitment, and tactical planning. It also provides insights for marketing and promotional efforts by highlighting standout performers to fans and potential sponsors.

3. Identify matches where a team scored more goals than their average and what were their results, shots pg and passes pg were
![image](https://github.com/user-attachments/assets/b92a241e-2d04-4d24-8182-12416b9c2b89)


Identifying matches where a team scored more goals than their average provides managers with insights into factors contributing to above-average performance, such as tactics, player form, or opponent weaknesses. Analyzing the results, shots per game, and passes per game in these matches can reveal patterns that help optimize strategies, improve training, and make data-driven decisions to replicate such high-scoring outcomes consistently.

4. Provide a detailed breakdown of each player’s performance in different leagues, specifically focusing on their average goals scored per match and average pass percentage.
![image](https://github.com/user-attachments/assets/c3b47f77-066d-4ffe-9a76-a9ca875f2a13)


By grouping the data by league and player, and then sorting by league and average goals scored, this query helps identify top performers in each league, making it valuable for comparing player efficiency and impact across different competitions. This information can assist managers, scouts, and analysts in evaluating player consistency and making data-driven decisions regarding player development, transfers, or strategic planning.

5. Retrieve the players with the highest number of tackles from each team, along with their first name, last name, and team name.
![image](https://github.com/user-attachments/assets/9625f6b3-60e5-4436-9a76-39462f75b9ce)


It allows managers and analysts to identify the best defensive players within each team, which is valuable for understanding defensive strengths, player contributions, and for making decisions about player training, positioning, and strategy. By sorting the results by team name, the query provides an organized view of top tacklers across all teams.

6. Retrieve detailed information about the player Lionel Messi, including his first name, last name, team name, and position.
![image](https://github.com/user-attachments/assets/73e565fa-0d3b-4e5e-aa6c-be134b4817a0)


It helps quickly identify specific details about a well-known player and can be used for player profile generation, reporting, or verifying his current team and position, which can be useful for managers, fans, or analysts looking for up-to-date player information.

7. Calculate the total number of goals scored by Lionel Messi.
![image](https://github.com/user-attachments/assets/484bae40-df4d-4995-b9fb-7e2f6e9967ec)


It aggregates his goal count across all matches in the playerStats table, providing an overview of his scoring performance. This information can be used for player performance analysis, historical records, or comparisons against other players. It's valuable for managers, analysts, and fans who want to quantify Messi’s goal-scoring achievements.

8. Provide an overview of player performance based on nationality, showing the number of players and the total number of goals scored by players from each nationality.
![image](https://github.com/user-attachments/assets/0e1a8ed9-6cd4-4cab-be28-e632f1fef947)


It offers insights into how different nationalities contribute to overall performance. This information can help managers, analysts, and scouts identify strong talent pools by nationality, understand scoring patterns, and inform recruitment or scouting strategies.

9. Compare the performance of mentor-mentee coaching pairs based on the number of team wins

![image](https://github.com/user-attachments/assets/439f9c33-2d91-48aa-b1ef-907b196f4e23)


This analysis can provide insights into the effectiveness of mentorship programs, track mentee development, and highlight successful coaches who have outperformed their mentors.

10. Retrieve the teams and the corresponding match ID for teams that competed against each other at Old Trafford on January 15, 2024, at 3:30 PM.

![image](https://github.com/user-attachments/assets/dc2116ab-5ef4-4546-9ce1-255540bb59e9)


Retrieving this information is useful for managers, analysts, and fans to review specific matches played at a particular venue and time, such as Old Trafford. It helps identify key games, analyze performance metrics, and understand the context of team matchups. This data can also be used for scheduling, historical analysis, and preparing for future encounters between these teams at similar venues or conditions.

Database Information


![image](https://github.com/user-attachments/assets/96370a76-d366-4a95-9c72-0ead3ae9d8aa)


