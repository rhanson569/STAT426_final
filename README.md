# STAT426_final
Final Project for STAT 426

Prediction Question - Can you use raw statistics to predict who will make one of the annual All-NBA teams? A secondary question was whether traditional statistics (points, rebounds, assists,etc.) or advanced statistics (PER, BPM, VORP) would be more reliable in prediction.

After reading and wrangling my data, I selected specific features for traditional and advanced stats. For traditional, I used Field Goal Attempts, Effective Field Goal Percentage, Points, Total Rebounds, Assists, Blocks, and Steals. For Advanced metrics, I used Player Efficiency Rating, Usage Percentage, True Shooting Percentage, Box Plus Minus, Win Shares per 48, and Value over Replacement Player. I initially combined the data together into one table called total and used Multinomial NB, Decision Tree, and Random Forest models. Multinomial NB predicted that no player would make an All-NBA team, so clearly that model was an issue. The best model was the random forest. The random forest model had about a 97% accuracy, while only about 93% of the data was players who didn't make an All-NBA team. It was able to find the pattern and predict 99% of those who didn't make the All-NBA team correctly. It also guessed 70% of those who made an All-NBA team correctly, a high number considering only 6% of players make one of the teams.

I then separated the advanced and tradiitonal statistics back into their datasets and ran them through random forest models. To my surprise, the advanced statisitics were on average about a 1% higher than the traditional stats, despite the lack of usage until only recently. It showed that even back in the 80's, when advanced stats weren't utilized, these stats could reliably predict who would make an All-NBA team.

There could be some bias, however, in the variables I chose. I have a lot of experience with the NBA and so I chose the variables I felt would best predict from each category. 
