# **Colorado Avalanche Season Prediction:** 

---

This is a project I did for my Data Science course at Regis University. The purpose of this project is to determine the season ending prediction for the Colorado Avalanche hockey team for the 2022-2023 season. 

My goal was to predict their expected statistical totals for certain categories and leverage those to determine if they will return to the playoffs this season and what the probability of that predicted outcome is. 

---

## **Data:** 
The data leveraged was retreived from the NHL. The location of the data is www.nhl.com/stats/

---

## **Project Process:** 

The process for my project started by collecting data for all the teams since the 2010-2011 season. I also collected the individual player statistics up to the same season, if the specific player has played that many season. Many have not played that long and are newer to the league, and therefor have fewer season statistics to leverage. The individual players were picked based on the Colorado Avalanche Roster and Depth Chart as of late September, 2022 (prior to season start). 

I determined the most imporant features that impact a team making or missing the playoffs, and then continue to extrapalate those imporant features to identify what individual, player statistics are the most impactful. 
Leveraging those specific statistic, I developed a representative team prediction for the Avalanche based on the career averages for the players. I did apply a multiplier to specific players that are expected to overachieve their average totals - this was decided by players who play well over half the games each season, and who average Time On Ice/Game Played (how much a player actually plays each game) that is over the average TOI/GP for their respective position. Only 8 players were affected. 

Using these totals, I was able to predict how many Wins the team can be expected to have this season, which in turn, allowed me to predict whether they will make or miss the playoffs and how likely that result is to be true. 

---

***Import note**: Given the time restraint of this course, I purposefully did not take into account any possible roster changes, such as injuries, trades, free agency, etc. These will invitably occur, but for this project, my representative team of players will start and stop the season together, unchanged. 

You will see in the data that for the team statistics, there are 3 seasons that were removed from the data and that these 3 seasons may, or may not have been removed from specific player statistics. These seasons are all shortened seasons due to a lockout in 2012-2013 season, and the two seasons shortened due to COVID. Because I am working heavily with averages, keeping these seasons in the data would significantly skew the results. 
Depending on how many seasons a player has, I either removed or kept those shortened seasons due to a lack of data for specific players. In the future, I likely could implement some adjustments to make predictive totals for those players based on per game averages. 

---

## **Machine Learning Models Used:**

Random Forest Classifier, Random Forest Regressor, Gradient Boosting Regressor, and Extra Trees Regressor

***Note**: I know there is some overfitting in certain models, but I actually was fine with that being the case given the data used. 

---

## **Future:**
I learned AFTER this project that there is a provided, but relatively unknown API maintained and provided by the NHL which allows you to gather team and player data, which includes MANY more statistics than the website provides. In future iterations of this project, I would love to included data from that API, which would allow me to programatically handle predictions for ALL players and teams, rather than just the Avalanche as manually collecting data and combining predicted teams would be too time consuming that it's worth. 

# **Finally:**

This is my first true, start to finish project I have done myself, so keep that in mind with errors you may find or anything missing - I welcome thoughts on how I could better this project. 



