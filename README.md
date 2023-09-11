# Cookie-Cat-A-B-Testing
## Background
Cookie Cats is a hugely popular mobile puzzle game developed by Tactile Entertainment. It's a classic "connect three" style puzzle game where the player must connect tiles of the same color in order to clear the board. As players progress through the game they will encounter gates that force them to wait some time before they can progress or make an in-app purchase. But where should the gates be placed? Initially the first gate was placed at level 30. In this project, we're going to analyze an AB-test where we moved the first gate in Cookie Cats from level 30 to level 40. Description from [DataCamp](https://www.datacamp.com/projects/184)  
## Problem
Should we move the gate from level 30 to level 40 based on player's retention rate?
## Dataset  
### Variables
**userid** - A unique number that represents each player  
**version** - Gate is placed at level 30(control group) or level 40(treatment group)  
**sum_gamerounds** - The player's first-week game rounds  
**retention_1** - did the player come back and play 1 day after see the gate?  
**retention_7** - did the player come back and play 7 days after see the gate?  
## Create Metrics
+ 1-day Retention: The percentage of players that return to play the game within 1 day of installation
+ 7-day Retention: The percentage of players that return to play the game within 7 days of installation
## Results
### 1-day Retention 
+ There was a subtle decrease in 1-day retention when the gate was moved to level 40 (44.2%) compared to level 30 (44.8%)
+ Utilized bootstrapping method, the most likely percentage difference is around 1%-2%
+ 96% of the distribution is above 0, in favor of a gate at level 30
### 7-day Retention 
+ There was a decrease in 7-day retention when the gate was moved to level 40 (19.0%) compared to level 30 (18.2%)
+ The overall 7-day retention is lower than 1-day retention
+ 99.8% of the distribution is above 0, in favor of a gate at level 30
## Conclusion
Both 7-day and 1-day retention is higher when the gate is at level 30. If we want to keep the retention high, we should not move tthe gate.  
Reason behind result:
+ The tendency for people to get less enjoyment out of a fun activity over time
+ When the gate is moved to level 40, fewer players make it far enough, and they are more likely to quit the game due to boredom
