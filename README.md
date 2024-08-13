# nosql-challenge
Module 12 Challenge
## Overview
Utilizing MongoDB to help a food magazine find highly-rated, clean restaurants around London and this particular new restaurant called Penang Flavours.

### Specific Questions from the magazine
1. Which establishments have a hygiene score equal to 20?
   I set the requirement of having a hygiene score = 20 as the query and just used "establishments.find(query)" to find all of them from our existing data. Then I compiled them into a Pandas Dataframe.
2. Which establishments in London have a RatingValue greater than or equal to 4?
   I used the same method to answer this question. Only for this, I searched for a regular expression of "London" as told by the hint.
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
   First, we found Penang Flavours' location and used its coordinates as the center of our search radius. Then it was about the same method as above.
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
   For this, I was told to make a pipeline that find restaurants that matches the hygiene requirement, groups the results to its local authority, then sort them from highest to lowest, and finally aggregates the results. Lastly I compiled the results to a Dataframe.
