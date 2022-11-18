
# Codecademy NBA Trends Project

In this project,we will analyze data from the NBA (National Basketball Association) and explore possible associations.
This data was originally sourced from 538's Analysis of the Complete History Of The NBA and contains the original, unmodified data from Basketball Reference as well as several 
additional variables 538 added to perform their own analysis.

For this project we've limited the data to just 5 teams and 10 
columns (plus one constructed column, point_diff, the difference 
between pts and opp_pts).


## Task  performed

1. The data has been subset  into two smaller datasets: 
games from 2010 (named nba_2010) and games from 2014 (named nba_2014).
To start, let’s focus on the 2010 data.

 Suppose we want to compare the knicks to the nets with respect to points earned per game. Using the pts column from the nba_2010 DataFrame, create two series named knicks_pts (fran_id = "Knicks") and nets_pts(fran_id = "Nets")
 that represent the points each team has scored in their games.

2. Calculated the difference between the two teams’ average points scored and save the result as diff_means_2010. Based on this value, do you think fran_id and pts are associated?

3. Rather than comparing means, it’s useful look at the full distribution of values to understand whether a difference in means is meaningful.
 we created a set of overlapping histograms that can be used to compare the points scored for the Knicks compared to the Nets. we will use the series you created in the previous step (1) and the code below to create the plot. 

4. Now, let’s compare the 2010 games to 2014. We will Replicate the steps from Tasks 2 and 3 using nba_2014. First, we will calculate the mean difference between the two teams points scored.We will Save and print the value as diff_means_2014. 

5. For the remainder of this project, we’ll focus on data from 2010. Let’s now include all teams in the dataset and investigate the relationship between franchise and points scored per game.

Using nba_2010, generated  side-by-side boxplots with points scored (pts) on the y-axis and team (fran_id) on the x-axis.

6. We'd like to know if teams tend to win more games at home compared to away.

The variable, game_result, indicates whether a team won a particular game ('W' stands for “win” and 'L' stands for “loss”). The variable, game_location, indicates whether a team was playing at home or away ('H' stands for “home” and 'A' stands for “away”).
Data scientists will often calculate a contingency table of frequencies to help them determine if categorical variables are associated. We will Calculate a table of frequencies that shows the counts of game_result and game_location.
Save our result as location_result_freq and print our result.

7. We will Convert this table of frequencies to a table of proportions and save the result as location_result_proportions.

8. Using the contingency table created in the previous task (7),we will calculate the expected contingency table (if there were no association) and the Chi-Square statistic.

9. For each game, 538 has calculated the probability that each team will win the game. We want to know if teams with a higher probability of winning (according to 538) also tend to win games by more points.

In the data, 538's prediction is saved as forecast. The point_diff column gives the margin of victory/defeat for each team (positive values mean that the team won; negative values mean that they lost).

Using nba_2010, we will calculate the covariance between forecast (538's projected win probability) and point_diff (the margin of victory/defeat) in the dataset. Save and print your result.

10. Because 538’s forecast variable is reported as a probability (not a binary), we can calculate the strength of the correlation.

Using nba_2010, calculated the correlation between forecast and point_diff. Call this point_diff_forecast_corr. We will Save and print your result. 

11. Generate a scatter plot of forecast (on the x-axis) and point_diff (on the y-axis).

