# Predicts the next Cricket ODI match result between current top 5 teams based on ICC Rankings
### Reason Adhikari

## Work FlowChart
##### Data: The data being collected are based on recent and updated rankings, NOT based on all-time rankings. They are likely to update after each One Day International match.


1. Find the current top 5 teams. <br>
2. Scrap Nationality and Score of top 100 Batsmen and store them in individual lists if they are from country in top five. <br>
    -> Average the bating score for each teams <br>
3. Scrap Nationality and Score of top 100 Bowler and store them in individual lists if they are from country in top five. <br>
    -> Average the  bowling score for each teams <br>
4. Scrap Nationality and Score of top 20 All_rounders and store them in individual lists if they are from country in top five. <br>
    -> Average the allrounder score for each teams <br>

- Average Players ranking gives the ranking of teams based on players current trend in performance. <br>
- Team with most players in right form/shape is likely to win. <br>
- Outcome of future matches are predicted based on the scores above. <br>

#### Data Source: ICC official websites
#### Webpages used:
- [team_ranking](https://www.icc-cricket.com/rankings/mens/team-rankings/odi") <br>
- [batting_ranking](https://www.icc-cricket.com/rankings/mens/player-rankings/odi/batting") <br>
- [bowling_ranking](https://www.icc-cricket.com/rankings/mens/player-rankings/odi/bowling ) <br>
- [all_rounder_ranking](https://www.icc-cricket.com/rankings/mens/player-rankings/odi/all-rounder") <br>

#### Tools and Packages Used:
* requests
* pickle
* bs4 (beautifulsoup)
* matplotlib (matplotlib.pyplot)
* matplotlib (matplotlib.style)
