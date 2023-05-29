# Evil-Geniuses-x-Genius-League

## Project Overview

This project aims to analyze the performance of Starcraft players using a comprehensive dataset, containing detailed information about their basic demographic and in-game statistics.

## Introduction

Starcraft is a popular real-time strategy game known for its competitive gameplay, and studying player in-game statistics can provide valuable insights into technical strategies, skill levels, and factors influencing ranking.

The analysis of player in-game statistics in Starcraft can have various applications, such as guiding aspiring players to improve their skills, assisting coaches in devising effective training programs, strategic planning, and providing insights to game developers for balancing gameplay mechanics. Furthermore, understanding the dynamics of player performance in a competitive gaming environment like Starcraft can contribute to the broader field of esports analytics and enhance our understanding of the factors that drive success in professional gaming especially in e-sport league.

## Abstract

This project presents an analysis of in-game statistics in Starcraft and the development of predictive models for ranking prediction. Machine learning algorithms, including KNNClassifier, Logistic Regression, Support Vector Machine, and Random Forest Classifier, were employed to accurately predict player rankings based on comprehensive performance data. The models achieved an accuracy of approximately 43% in classifying player rankings and demonstrated a strong NDCG score of 0.988, indicating their effectiveness in ranking players. These findings offer valuable insights into the relationship of in-game statistics and league index, guiding strategic decision-making and contributing to the development of fair and competitive gameplay environments in Starcraft.

## Data Description

The dataset used in this project consists of various features capturing the performance and statistics of Starcraft players. Here are the description of 20 features included in the dataset:

1. GameID: Unique ID number for each game
2. LeagueIndex: Bronze, Silver, Gold, Platinum, Diamond, Master, GrandMaster, and Professional leagues coded 1-8
3. Age: Age of each player
4. HoursPerWeek: Reported hours spent playing per week 
5. TotalHours: Reported total hours spent playing 
6. APM: Action per minute
7. SelectByHotkeys: Number of unit or building selections made using hotkeys per timestamp
8. AssignToHotkeys: Number of units or buildings assigned to hotkeys per timestamp
9. UniqueHotkeys: Number of unique hotkeys used per timestamp 
10. MinimapAttacks: Number of attack actions on minimap per timestamp 
11. MinimapRightClicks: number of right-clicks on minimap per timestamp
12. NumberOfPACs: Number of PACs per timestamp 
13. GapBetweenPACs: Mean duration in milliseconds between PACs
14. ActionLatency: Mean latency from the onset of a PACs to their first action in milliseconds
15. ActionsInPAC: Mean number of actions within each PAC 
16. TotalMapExplored: The number of 24x24 game coordinate grids viewed by the player per timestamp
17. WorkersMade: Number of SCVs, drones, and probes trained per timestamp
18. UniqueUnitsMade: Unique unites made per timestamp
19. ComplexUnitsMade: Number of ghosts, infestors, and high templars trained per timestamp
20. ComplexAbilitiesUsed: Abilities requiring specific targeting instructions used per timestamp

Data preprocessing steps included handling missing values, imputation, and scaling numerical features. Exploratory data analysis (EDA) was performed to gain insights into the distribution of variables and identify any patterns or correlations.  

## References and Citations
1. "StarCraft." StarCraft Official Website, Blizzard Entertainment, 2023, https://starcraft.com/en-us/.
2. "Dutta, Ankita. 'Demystifying NDCG.' Towards Data Science, Medium, 10 Nov. 2020, https://towardsdatascience.com/demystifying-ndcg-bee3be58cfe0."

## Conclusion and Future Work
The models achieved an average accuracy of 43% in predicting the league index and a 98.6% of NDCG Score. The Random Forest algorithm outperformed other models, and it is the best to be used for ranking prediction considering the computational and cost efficiency while also providing valuable insights into the most influential features. 

Future work could involve:
1. Exploring additional feature engineering techniques
- potentially create new variables based on the relevant features (ideally formulate the effectiveness of actions, attacks, and units made based on frequency of the variables)
2. Investigating other features such as:
- historical performance records (Win-Loss Ratio)
- match outcomes (ELO rating)
- tournament results
- expert judgement (referencing from coach or experienced players)
- player profiles (demographics)
- game mode (single player or multi-player, PvP vs PvC)

3. Identifying a clearer outlier boundary as the TotalHours and HoursPerWeek spent in gaming is illogically large.  
 
4. Incorporating external data sources
5. Implementing advanced ensemble methods

for further improving model performance.

Data collection could be collected via training over Artificial Intelligence players from several difficulty and task.  
