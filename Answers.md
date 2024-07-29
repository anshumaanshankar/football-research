### Question 1
For this question, I evaluated a player's ability in comparison to others in the same position using Madden 23 rankings to get an overall rating for each player. Additionally, I normalized player salaries to compress the range of values. I then calculated each player's 'value' as their rating divided by their normalized salary. Grouping players by position, I identified the top three players per position based on this value metric. Due to the difficulties of web scraping, I manually added the type of acquisition for each player.

The analysis revealed an overwhelming majority of free agents, with drafted players being the second most common, followed by trades. To enhance this analysis, we could leverage player stats grouped by position, create a model to identify the most significant metrics, and rank players using a formula based on these metrics.

The findings are documented and available on my GitHub repository.