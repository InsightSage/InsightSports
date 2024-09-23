# InsightSports

## Project Overview

**InsightSports** is an open-source initiative by Insight Sage aimed at developing a standardized data model for analyzing sports statistics across multiple sports. Our goal is to create a comprehensive and adaptable data framework that captures all measurable elements of the game, including player performance, team dynamics, and referee decision-making. Starting with basketball, we will expand this model to other major team sports like soccer, baseball, football, hockey, lacrosse, and beyond.

## Project Goals

1. **Create a Unified Sports Data Model**: Develop a common data schema that can be adapted across different sports. The model will capture core elements like player statistics, team performance, play-by-play data, and referee metrics.
   
2. **Focus on Referee Analysis**: A unique aspect of this project is the focus on referee performance, which is often underrepresented in traditional sports analytics. InsightSports aims to provide deeper insights into how referee decisions impact the flow and outcome of games.

3. **Open Source and Community-Driven**: This project is open source, hosted on GitHub to encourage collaboration, feedback, and contributions from the global community of data analysts, sports enthusiasts, and developers.

4. **Expandable Framework**: Start with basketball and expand to other sports, ensuring the model remains adaptable and scalable. We aim to support the analysis of large team sports that require high-level skill from referees to monitor multiple athletes simultaneously.

## Current Progress

### Basketball Use Case

The initial focus is on basketball, using data from the 2023 CCAA Men's Basketball Championship. We have manually downloaded scorecards from this tournament, which are stored in the folder `raw_data_manual_download`. These files serve as the primary data source for building and testing our initial model.

Tournament data source: [2022-23 CCAA Men's Basketball Championship Schedule](https://www.ccaa.ca/sports/mbkb/2022-23c/schedule)

### Data Model Overview

The InsightSports data model will include the following core components:

1. **Player Stats Table**: Records individual player performance metrics, such as:
   - Player ID, Name, Team
   - Field Goals Made/Attempted (FGM-A)
   - Three-Point Shots Made/Attempted (3PM-A)
   - Free Throws Made/Attempted (FTM-A)
   - Offensive and Defensive Rebounds (OREB, DREB)
   - Assists (AST), Turnovers (TO), Blocks (BLK), Steals (STL)
   - Fouls Committed (PF), Total Points Scored (TP)
   
2. **Team Stats Table**: Aggregated statistics for each team, including:
   - Team ID, Team Name
   - Total Field Goals, Three-Pointers, and Free Throws
   - Rebounds, Assists, Turnovers, and Fouls
   - Points in the Paint, Second-Chance Points, Points off Turnovers

3. **Play-by-Play Table**: Detailed event logs capturing every moment of the game:
   - Game Time, Event Type (shot, foul, turnover, etc.)
   - Players Involved, Points Scored
   - Referee Calls and Outcomes

4. **Referee Metrics Table**: Data focusing on the referees' actions and their impact:
   - Referee ID, Name, Calls Made
   - Foul Distribution, Calls by Period
   - Controversial Decisions and Reviews

## Roadmap

1. **Phase 1: Basketball Data Model** (Current)
   - Develop the data model and ETL processes for basketball.
   - Build Python scripts to extract, parse, and load data from manually downloaded scorecards.

2. **Phase 2: Expand to Other Sports**
   - **Soccer**: Adapt the model to incorporate unique aspects such as offside decisions, corner kicks, and goalie performance.
   - **Baseball**: Include pitch-by-pitch analysis, batting metrics, and umpire decision tracking.
   - **Football**: Focus on down-by-down analysis, player positioning, and referee penalties.
   - **Hockey**: Incorporate data on shots on goal, power plays, and penalty analysis.
   - **Lacrosse**: Track player movements, shot efficiency, and referee foul calls.

3. **Phase 3: Advanced Analytics and Visualization**
   - Develop dashboards and visualization tools for deeper insights.
   - Explore machine learning models to predict referee performance and game outcomes.

4. **Phase 4: Community Engagement and Feedback**
   - Open the project to contributions from the sports and data analytics communities.
   - Host webinars, workshops, and hackathons to encourage the use and expansion of the model.


## Contact

For questions or suggestions, please open an issue on GitHub or contact us at [insightsports@insightsage.co](mailto:insightsports@insightsage.co).
