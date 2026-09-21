# Machine-Learning---Movies---Hit-or-Flop

# Movie Success Prediction: Hit or Flop

## Why Should We Predict the Success of Movies?

- When a movie is produced, it takes resources, and it can become expensive/ risky 
- Production businesses want to be able to reduce the losses they may have and maximize Return on investment
- Predictive models help 
  - make budget decisions 
  - perform better release strategy 
  - streaming platforms to identify which genres attract the biggest audience
  - predict churn-reducing titles

## Objective 

Build a machine learning model that predicts whether a movie will be a hit or flop based on key features

## About the Dataset 

- Derived from Kaggle
- 10,178 rows of movies
- 12 features
- the features have categorical, numerical, and text types

## Cleaning the Dataset 

### Issues encountered with Dataset

- Total of 85 missing values in ‘genre’
- Total of 56 missing values in ‘crew’

### Cleaning Dataset

- Categorical feautures such as genre, director, and country were converted into numerical values
- made sure there were no nulls
- created a variable hit or flop
- after labeling, revenue was dropped

## How We Built Our Decision Tree

### dependent variable

We had to manually code our target variable, these are the parameters we used.

- **HIT** → revenue > budget
- **FLOP** → revenue ≤ budget

### features used in Decision Tree

- budget_x
- score
- genre
- actor_count
- orig_land
- country
- director

## Confusion Matrix + Rresults

- **Train accuracy:** 85%
- **Test accuracy:** 82%

## Feature Importance 

Budget and score are the strongest predictors in movie success aka making it a ‘Hit’

## Visualization

The first split is : Budget 

High budgets tend to have ‘Hit’

Low budget varies; it depends on 

- Score
- Genre
- Director 
- Country

## Limitations

- Dataset has amix of data types, so we had to limit our features a lot. In the real world, a movie success is based on more features.
- The “Score” variable does not exist for a lot of new movies. We had to input a medium score for new movies but this introduces human-bias.
- Dataset may not reflect current trends. Movies in different time periods have different trends.

## Recommendations 

- Increase budgets for movies that have promising success
- Focus on movies that have an early high score
- Avoid investing in films that fall in the low-budget and low score category, these tend to flop
