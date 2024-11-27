# NFL-Prediction

NFL Outcome Prediction & Analysis
This project focuses on predicting key NFL game metrics, specifically Total Rushing Yards and Total Passing Touchdowns, using season-level data from NFL teams spanning 1920 to 2024. Employing elastic net regression, the model was trained on a dataset of team statistics, such as wins, games played, rushing attempts, passing attempts, and yards, while accounting for multicollinearity and scaling issues inherent to sports data.

Key goals included:

Predicting per-game rushing yards and passing touchdowns for NFL teams.
Aggregating predictions to forecast combined totals for specific matchups and events, such as Thanksgiving Day games.
Delivering accurate and explainable results to inform analyses of team performance.
Through systematic preprocessing, feature selection, and model evaluation, our approach achieved strong results. The model's accuracy was validated by achieving a top 5 rank in a competitive evaluation of NFL prediction models. This project demonstrates the value of elastic net regression in balancing model complexity with interpretability, making it suitable for sports analytics and predictive modeling in large datasets.

The repository includes code for:

Cleaning and preparing NFL datasets.
Predicting Rushing Yards and Passing Touchdowns using elastic net regression.
Aggregating and analyzing game-level outcomes based on season-level predictions.
This project highlights the potential for data-driven insights in sports, bridging historical data with predictive analytics.

Dataset Sources
The data used in this project was sourced from publicly available NFL statistics:

Stathead - NFL Team Season Finder
Website: Stathead
Description: Historical NFL team statistics from 1920 to 2024, including passing touchdowns, rushing yards, and other team-level metrics.
Acknowledgments
We acknowledge the contribution of the original dataset providers for making the data available for analysis. Elastic Net regression models and statistical insights were implemented using the following libraries:

R: caret, glmnet, and related packages.
Python (if applicable): scikit-learn, pandas, etc.
