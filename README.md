## Project Description

This extra credit project for **STOR 455 (Methods of Data Analysis)** focuses on predicting NFL game outcomes using historical team statistics. The analysis was conducted by applying Elastic Net regression to predict two key metrics: total passing touchdowns (PassTD) and total rushing yards (RushYds) for NFL teams. The results were combined to estimate game-level performance based on team-level seasonal data.

### Procedure

1. **Data Collection**:  
   Historical NFL team data was sourced from [Stathead - NFL Team Season Finder](https://stathead.com/football/team-season-finder.cgi), covering team performance metrics from 1920 to 2024. Each dataset represents a team's season-level performance.

2. **Data Cleaning & Preprocessing**:  
   - Irrelevant columns were removed, and variables were standardized to address scaling differences.
   - Highly correlated variables were excluded to handle multicollinearity, ensuring model robustness.
   - Seasonal data was adjusted to generate per-game metrics for predictions.

3. **Model Development**:  
   - **Elastic Net Regression**: A combination of Lasso and Ridge regression was used to handle multicollinearity and select the most relevant features. Separate models were trained for predicting PassTD and RushYds.
   - Log-transformation was applied where necessary to improve model fit.

4. **Prediction**:  
   - Models were evaluated using R² and RMSE metrics to validate performance.
   - Predictions were scaled back to per-game and seasonal levels, enabling comparisons across teams.

5. **Outcome Calculation**:  
   - For specific NFL games, predicted RushYds and PassTD values were multiplied to estimate the overall game score metric:  
     **(Total Rushing Yards) × (Total Passing Touchdowns)**  
   - Results were aggregated for teams playing on Thanksgiving Day 2024.

### Results

Our team’s models ranked in the top 5 for prediction accuracy, demonstrating the effectiveness of Elastic Net regression in analyzing NFL data. The project highlights how team-level seasonal data can effectively approximate game-level outcomes, even without direct interaction data between teams.

## Dataset Sources

- **[Stathead - NFL Team Season Finder](https://stathead.com/football/team-season-finder.cgi)**  
  Historical NFL statistics from 1920 to 2024, including passing touchdowns, rushing yards, and other metrics.

## Acknowledgments

We thank Stathead for providing the dataset and acknowledge the use of the R programming language, with libraries such as caret and glmnet, in model development.
