# Bracketology
Predictions for seeding of March Madness.

Stats obtained through warrennolan.com

Step 1) Perform a logistic regression to assign every team a probability of making the tournament.
Take the top 68 as the teams in the field (regardless of how many have a >50% chance of making it)

Step 2) Perfrm a linear regression to try to predict seeding. This is used to create an ordinal ranking, rather than actual seed values.

Step 3) (Attempt to) build a bracket, trying to maintain teams within their overall seeds. Note I have limited understanding of the proccess of turning overall seeds into the bracket.

field_predictions.csv - Ranking of all teams in order of most likely to least likely to make the field.
overall_seed_predictions.csv - Overall seed ranking of the top 68 teams, 1-68. Note this order need not match the field_predictions order.
bracket.txt - My attempt to build a bracket out of the above file.

Results:  
2025:  
65/68 teams correct.   
37 on correct seed line.  
20 off by 1 seed line.  
6 off by 2 seed lines.  
2 off by 3 seed lines.  
Final score - 326  
