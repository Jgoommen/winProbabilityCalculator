# winProbabilityCalculator
## Matchup calculator using cloudscraped KenPom data

<img width="310" height="163" alt="image" src="https://github.com/user-attachments/assets/b791212f-0298-4bd1-b73a-b6fc64305db7" />

## Overview
The goal of this project is to predict the outcomes of an NCAA college basketball game using reliable, continuously updated data.

Since the official KenPom website is subscription-blocked, I had to use a cloudscraper instead of a normal webpage parser to read in the data. Most websites that are subscription blocked will block requests, and the cloudscraper bypasses such blocks. KenPom in particular uses a software called Cloudflare, which monitors internet traffic and web requests among other things. 

I used adjusted offensive/defensive efficiency, adjusted tempo alongside league averages of tempo and efficiency to calculate scores. I used offensive/defensive efficiency to approximate the scoring capability of both teams, and then calculated the approximate tempo to find the possessions in a game. Combining the two is how I was able to estimate the final score.

I calculated the win probability by finding the difference in scores and using a normal CDF function from scipy



