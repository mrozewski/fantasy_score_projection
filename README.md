# fantasy_score_projection
Running random forest model to predict fantasy points based on pervious years' stats.

I used nfl-data-py for a previous project, which allowed easy access to in-depth player stats.
Considering ideas for my next project, I figured I could use these stats with sci-kit-learn to predict fantasy points.

It is a simple random forest model, using a number of features ('receiving_air_yards', 'receiving_yards_after_catch', 'targets', 'receiving_yards', 'receiving_tds',
            'pacr', 'receptions', 'receiving_first_downs', 'receiving_epa',
            'racr', 'target_share', 'air_yards_share', 'wopr').

Using data from the past 15 seasons, we got ok results:

Mean Absolute Error: 35.162439301255574
Mean Squared Error: 2121.6375427446565
Root Mean Squared Error: 46.06123687814578
R^2 Score: 0.4695763231194695

MAE is a high when receivers are scoring ususally in the mid 100s of points.
R squared is almost right down the middle, which is better than nothing I suppose. 
Did not have high hopes for the accuracy of the model, but it was fun to practice with ML.
