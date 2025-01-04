# Machine-Learning-Driven-MBTI-Classification-Project


## Overview

The Myers-Briggs Type Indicator (MBTI) is a psychological tool used to categorize individuals into one of 16 personality types based on their preferences in four dimensions: where they focus their attention, the way they take in information, how they make decisions, and how they deal with the outside world. Understanding these types helps in predicting and analyzing individual behaviors in various settings, including the workplace.

This project explores 'To What Extent Can Social Media Posts Predict One’s MBTI Personality Type?', utilizing a dataset with 8675 instances, each record contains an individual's MBTI type and their 50 most recent social media posts.

### MBTI and Workplace Behavior

Research has explored the relationship between MBTI types and workplace behavior, particularly in areas such as job performance, turnover, and workplace aggression. Notable findings include:

- **Extraversion (E) vs. Introversion (I)**: Extraverts are more likely to engage in 'passive-verbal' aggression while being less likely to consider 'active' behaviors as aggressive.
- **Intuition (N) vs. Sensing (S)**: Individuals with a preference for Intuition are more likely to rate 'passive indirect' behaviors as aggressive compared to those who prefer Sensing.
- **Perceiving (P) vs. Judging (J)**: Those who lean towards Perceiving are more prone to label behaviors as 'passive, indirect, physical' aggression.

These dynamics are critical in understanding how personality traits influence workplace interactions and can inform strategies for management and team composition.

## Project Video
Watch the detailed project overview here: [MBTI Personality Classification Project](https://youtu.be/10CQyKx4lvg).

## Research Question
To what extent can social media posts predict one’s MBTI personality type?

## Data Source
The dataset was sourced from Kaggle and includes the following features:
- **MBTI Type**: A 4-letter MBTI type of the individual.
- **Posts**: The 50 most recent social media posts of the individual, separated by `|||`.
  
Dataset Link: [MBTI Personality Type Dataset](https://www.kaggle.com/datasets/datasnaek/mbti-type)

## Data Preprocessing
1. **Text Cleaning**: Removal of links, punctuations, and conversion to lowercase.
2. **Lemmatization**: Converting words to their base forms.
3. **Stop Words Removal**: Elimination of stop words including single letters and incomplete words.
4. **Vectorization**: Applied before model training for feature extraction.

## Main Models Employed
### Tree-Based Models
- **Random Forest**:
  - Hyperparameter tuning via GridSearchCV.
  - K-Fold cross-validation.
  - Classification metrics and confusion matrix visualization.

### Linear Models
- **Logistic Regression**:
  - Feature selection through L1 regularization.
  - K-Fold cross-validation.
  - Performance comparison with Random Forest models.

## Evaluation and Challenges
- **Overfitting**: Decision Tree models showed tendencies to overfit.
- **Performance**: Random Forest models, while time-consuming, showed improved performance after hyperparameter tuning.
- **Handling Sparse Data**: Logistic Regression was adjusted for the imbalanced dataset using regularization.

## Conclusion
1. The model achieved an accuracy of 52%, indicating that it was able to correctly predict the personality type based on social media posts more than half of the time.
2. The model achieved an accuracy of 52%, indicating that it was able to correctly predict the personality type based on social media posts more than half of the time.
3. The model's ability to predict different personality types varied, suggesting that some personality traits or types may be more easily identifiable from social media posts than others.



## Resources and References
- Dataset: [MBTI Myers-Briggs Personality Type Dataset](https://www.kaggle.com/datasets/datasnaek/mbti-type)
- Related study on personality and workplace behavior: [Personality Factors Linked to Workplace Aggression](https://mds.marshall.edu/etd/1589)

