# Finding Donors Project
Github repository for Udacity Intro to ML Project #1: Finding Donors for CharityML. This project includes the base project with a more in-depth data exploration, as well as more evaluation metrics being added. 

CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than \$50,000 annually. To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity. We will want to create a model that can correctly identify the individuals which should be asked for donations in our to maximize donations and minimize wasted letters.

The dataset for this project originates from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Census+Income). The data we investigate here consists of small changes to the original dataset, such as removing the `'fnlwgt'` feature and records with missing or ill-formatted entries.


### Project Outline:
#### Data Exploration:
- Plot histograms of numeric columns (distribution analysis).
- Explore any stand out findings from the numeric columns in more detail.
- Create a heatmap to see the correlation between label and features.
- Calculate general statistics of the data.

#### Data Preprocessing:
- Transform any highly skewed data that has been found.
- Normalize our numerical features to a scale [0,1].
- Encode our categorical features and labels to numeric format.
- Split our data into training and testing sets (80/20).

#### Initial Modeling:
- Create a Naive model (baseline prediction).
- Train 3 initial models.
- Choose best model to tune based on evaluation metrics (F-score).

#### Hyperparameter Tuning:
- Use Grid Search to find the optimal hyperparamter values based on an F-score with beta = 0.5
- Plot an ROC curve and check AUC to see how our model is performing.

#### Feature Importance:
- Find the 5 most important features used in the model training.
- Use the subset of important features to train a simpler model and see if we see any improvements.
