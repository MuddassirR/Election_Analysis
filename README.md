# Election_Analysis

## Overview of Election Audit
The purpose of this analysis was to determine the total number of votes for each candidate, the percentage of votes for each candidate, the winner of the election based on popular vote, the county with the most amount of votes, the total votes in the largest county, and the percentage of votes that came from the largest county, from a dataset containing voter information related to a Colorado election audit for a US congressional precint in Colorado. The dataset was in CSV formart and analysis was done on Python using import modules and on VS code.

## Election-Audit Results
 As shown in the [election results:](https://github.com/MuddassirR/Election_Analysis/blob/main/election_analysis.txt) 
 - there were 369,711 total votes casted in this precint.
 - there were 3 counties that voters belonged to in this precint: Jefferson, Denver, and Arapahoe
 - Jefferson received 38,655 votes which is 10.5% of total votes
 - Denver received 306,055 votes which is 82.8% of total votes
 - Araphoe received 24,801 votes which is 6.7% of total votes
 - Denver had the most votes as 306,055 of votes came from Denver, which is 82.8%
 - there were 3 candidates that people voted for in this precint: Charles Casper Stockham, Diana DeGette, and Raymon Anthony Doane
 - Charles Casper Stockham received 85,213 votes, which is 23% of total votes
 - Diana DeGette received 272,892 votes, which is 73.8% of total votes
 - Raymon Anthony Doane received 11,606 votes, which is 3.1% of total votes
 - thus, the winner was Dianna Degette with 272,892 votes (73.8% of total votes)

#Election-Audit Summary
The coding in this analysis can be used for other precints in Colorado. This would help determine not only the winners in each precient but the state as a whole, resulting in one being able to quickly determine who the final winner was and with how many votes and percentages of votes. You can also extend this code to beyond Colorado and make it country-wide, as the candidate_name = row[2] line of code helps get each candidate that was given a vote and county_name = row[1] helps get all the counties that were voted. You can add states as well to the election dataset and add a variable that is state_name = row[column to be indexed] to help determine which state had the best voter turnout. You could also add whether voters were female or male to help determine what percentage of voters voted for each candidate by gender, which could help provide polling data to political campaigns. If gender was its own column in the election dataset, you could find the total types of gender voters associated themselves with by coding gender = row[coluimn in election dataset to be index] using a for loop. If the gender does not equal a previous gender option, then add the new gender type to the gender list. Then you can create a new variable such as gender_votes and set it equal to candidate_votes.get(gender), and then candidate_name: {vote_percentage:.1f}% ({gender_votes:,})\n"). After printing, you would get the percentage of each gender that candidates got.
