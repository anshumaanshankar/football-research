### What avenue of player acquisition do you think currently provides teams with the most value per dollar spend and why?

1. I used a player's overall rating on Madden 23 to evaluate them in comparison to others in the same position. This rating, divided by the log of their salary gives each player a value score. Observing the top 3 players per position, it was seen that 60% of these players were signed as free agents and 30% were drafted. That is not hard to believe as hiring free agents means that teams acquire proven NFL talents without sacrificing draft picks or future assets, often at a lower cost than re-signing their own players. Additionally, it provides flexibility in addressing specific team needs and immediate roster improvements than grooming a rookie would.

    Although the answer makes sense, A single Madden rating may not be the best way to determine player value. Instead, we could consider changes in rating and salary over time to see if their value is increasing, plateauing or decreasing. For players with little or no NFL game time, college performance against rookie contract rates could best describe value. Alternative methods for comparing players could involve using overall metrics like Pro Football Focus (PFF) ratings or formulating our own Wins Above Replacement (WAR) metric, similar to baseball. By using these methods or a combination of them, we can overcome the shortcomings of relying on a single Madden ranking.

  
      The working, analysis and visualizations for my chosen approach are available on my GitHub repository: https://github.com/anshumaanshankar/football-research/

### Imagine that you are tasked with evaluating the accuracy of three different college-to-pro player projection systems for wide receivers. You have both the projections and actual pro statistics for the past 10 seasons. Discuss how you would approach the problem and list any potential issues you may encounter.

2. To me, projecting a player's future performance based on the past is similar to predicting stock prices. Just as a stock's value depends on company valuation and competition, a player's performance relies not only on their abilities but also on the surrounding environment. Therefore, in my opinion, models should be compared on the number and kind of captured metrics. Models accounting for metrics such as past injuries and their recurrence risk, the team's style of play & its alignment with the player's strengths as a percentage, expected playing minutes for the rookie based on squad depth are better than one that does not. Specifically for wide receivers, existing chemistry with the quarterback—such as sharing an alma mater like Joe Burrow and Ja'Marr Chase—can positively impact performance and should be included. While the quantification of some metrics may be subjective, integrating them once they are well defined will help these models outperform their stats-only counterparts.

   We can evaluate systems by how well they capture the correlation of key statistics with outcomes or by calculating error metrics such as MAE/RMSE between projections and actual numbers. When comparing algorithms, we can run multiple statistical tests to compare accuracies and determine which system is superior. While this approach can be effective, I lean towards models that also capture less mainstream statistics, in the case of similar performance with more common, stats-only models.

### Choose any active player in the NFL. How do you assess the quality of this player relative to their position group, and why? How would you value this player in terms of dollars, and how does this compare to their current contract?

3. I will be comparing Josh Allen against other QBs. For the 2023 season, I considered QBs who played at least 9 games (> 50% of the reg. season), ranking them on eight metrics: Passing & Rushing Yards, Completion %age, Adjusted Net Yards per Attempt, Sacks, Game-Winning Drives, 4th Quarter Comebacks, TD/INT Ratio - highlighting passing accuracy, efficiency, pressure handling, clutch performance, decision-making, and versatility, for a comprehensive assessment.

    After ranking them on these metrics, I find their average ranking. Allen ranked 1st, consistent with his reputation as a top-tier QB. Despite this, Allen is the 12th highest-paid QB. While 9 of the 11 earning more signed contracts in the last 18 months, indicating that Allen's salary is more about timing than ability, I believe Allen is slightly underpaid. Using a regression model targeting Avg salary, Allen's salary is predicted at $47.14 mil/year. Factoring in NFL experience compared to top earners, I value Allen at $60 million/year.
  
    Improvements to value calculation could include accounting for team dynamics that influence statistics and using weighted average to account for importance of metrics. Comprehensive metrics like QBR or Pro Football Focus (PFF) Grades could be included in conjunction, but I chose not to use them to prevent double-counts of certain stats. Allen ranks #3 on QBR, leading some confidence to our results. To see the working, please refer to my GitHub repository linked in Q1.

### The head coach has a difficult decision to make on 4th down. Discuss how you would evaluate the possible options using data.

4. When a head coach faces a 4th down decision, I evaluate the options using a data-driven approach to maximize win percentage like so:

i. Consider the 3 main choices: Going for it: Analyze yards-to-go, field position, offensive line & QB performance, opponent’s pass rush, secondary performance etc. Field goal: Assess kicker’s likelihood to score based on distance, performance, and weather conditions. Punting: Evaluate punt coverage and the opponent’s return ability.

ii. Incorporate contextual factors: Account for score differential, time left, home/away status and opponent scoring probability based on success/failure of each option. Use advanced metrics like Expected Points Added (EPA) and Win Probability Added (WPA), updated in real time, to quantify each option’s impact.

iii. Use real-time models: Input live data into pre-built models trained on historical data. These models would be updated after each play to reflect the current game situation accurately.

iv. Apply visualization tools: Use aids like heat maps and decision trees for quick data interpretation and real-time dashboards to help coaches and analysts make informed decisions collaboratively.

For example, on 4th and 2 at the opponent’s 40-yard line with 5 minutes left, the model can provide conversion likelihood, field goal success rate, and punt outcomes. This comprehensive approach ensures we make the most informed choice to maximize win probability.

### Why does football matter to you?

5. Football matters to me because, as an international student in the US for my graduate studies, it provided a sense of community and companionship. Coming from a cricket-loving city in India, I grew up an ardent sports fan, finding joy in discussing tactics and numbers. Right from the first NCAA game I watched, I quickly found a similar camaraderie in football, and this passion helped me build a community in Indiana. With each game, my interest deepened, and I grew to appreciate the NFL’s strategic complexity and depth.

   I love the game's structure. The NFL's emphasis on detailed play analysis and player statistics makes it highly analytical, offering ample space for data to influence decisions and outcomes. The strategic complexity involved in draft picks and game-day decisions also makes data crucial in shaping team success. This structure, governed by salary caps and performance-based draft orders, ensures that success comes from strategic excellence and smart decision-making, rather than just financial power.

    Given my passion for sports and my technical skills, the NFL presents an ideal opportunity for a career in sports analytics. The league’s structured, data-rich environment allows for the application of advanced analytics to drive decisions and strategies. This convergence of my interests and skills solidified my desire to pursue a career where I can contribute meaningfully to the sport while leveraging my analytical expertise.
