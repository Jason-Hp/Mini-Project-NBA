# SC1015-Mini-Project-NBA 🏀
A mini project for SC1015 Introduction to Data Science and Artificial Intelligence. We wanted to see if the regular season information can predict NBA champion.
Hence, we decided to analyse the past few season regular season data below.

## Problem Definition 📝
- Which variables from the regular season have a relationship with whether the team becomes/is a NBA Champion?
- Is there a change in a team's playstyle over the seasons?
- Can we use Machine Learning techniques to predict NBA Champion using regular season data?
## Dataset used 📊
The dataset used can be downloaded [here](https://github.com/Jason-Hp/SC1015-Mini-Project-NBA/blob/a30e139d5a7003d36726b341eb7636852126e224/Dataset/NBAdata.csv)
## Presentation 📹
The presentation video can be viewed [here](https://drive.google.com/file/d/1x4riJ3yn1-l3OWNkRCz0mhO2cC4el9vz/view?usp=sharing)
## Brief Details Of Notebook 📚
1. Data preperation & cleaning 🧹
   - Fill in all NULL values
   - One-hot encode a few categorical variables
   - Feature Engineering
   - Remove insignificant columns (variables)
   - Standardize decimal places & team names
2. Visualization & Exploratory Data Analysis 📈
   - Box-plots, Swarm-plots & Violin-plots
   - Point-Biserial Correlation Coefficient & P-value
   - Paired vertical column plots
   - Confusion Matrix (Heat Map)
   - Time-series plot
   - Cramer's V, phi coefficient & P-value
3. Machine Learning
   - Multi-variate Classification Tree 🌲
     - Best 10 variables (Predictors)
     - Average Classification Accuracy: 0.91
     - True Postivie Rate: 0.40
     - True Negative Rate: 0.94
    - Random Forrest 🌳🌳🌳
      - All variables (Except Champion)
      - Average Classification Accuracy: 0.85
      - True Postivie Rate: 0.67
      - True Negative Rate: 0.33
    - Cost-Sensitive Support Vector Machine 🔍
      - Best 10 variables (Predictors)
      - Average Classification Accuracy: 0.98
      - F1-score: 0.98
      - Recall: 0.98 & 1.00
## Conclusion, Data-driven insights & Recommendations 🏁
- Data Driven Insights
  - The higher these variables, the better odds of being Champion:
    - FG%,WIN%,3P%,2P%,AST,BLK,STL,DRB
  - Having the MVP and having high ranking also does positively impact being Champion
  - From our models, we seen that the most important variable is WIN%
  - From all 3 models, our Cost-Sensitive Support Vector Machine performed the best while Multivariate Classification Tree performed the worst
- Recommendations
  - We would obviously recommend using our SVM model when prediciting NBA Champion
  - Teams should seek out players who are:
    - More likely to be MVP
    - Shoot efficiently
    - Able to attack the rim
    - Taller side
    - Longer Wingspan
    - High WIN%
  - For players who have high WIN%, another parameter to look into would be the looking into their WIN Shares, which can tell us more about a player's ability to contribute to winning
## New Learning points 🧠
- Point-Biserial Correlation
- Cramer's V, phi's coefficient
- P-value
- Time-series
- Deal with imbalance data (Resampling)
- Random Forest Model
- Cost-Sensitive Support Vector Machine

## Group Members (FCSA, Group 4)
- Ho Shang Ji Jason - Data Preperation & Cleaning, Exploratory Data Analysis, Multivariate Classification Tree, Presentation Slides, Presenter
- Zou XueHao - Data Preperation & Cleaning, Random Forest, Presentation Slides, Presenter
- Gupta Mannan Mithun - Cost-Sensitive Support Vector Machine, Presentation Slides, Presenter

## References
- https://www.statology.org/phi-coefficient/
- https://www.statology.org/point-biserial-correlation-python/
- https://www.geeksforgeeks.org/how-to-calculate-cramers-v-in-python/
- https://pandas.pydata.org/docs/getting_started/intro_tutorials/09_timeseries.html
- https://scikit-learn.org/stable/auto_examples/model_selection/plot_precision_recall.html
- https://scikit-learn.org/stable/modules/svm.html
- https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html

 
