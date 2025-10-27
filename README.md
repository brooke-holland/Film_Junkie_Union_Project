The_Film_Junkie_Union_Project : https://github.com/brooke-holland/Film_Junkie_Union_Project

CodeSpace files : https://jubilant-happiness-975xpv5rrgwqhxqq.github.dev/

# Film_Junkie_Union_Project

## Project Statement

The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. You'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. It will need to have an F1 score of at least 0.85

Composed a evaluation routine which can be used for all models in this project

Trained and completed Random Forest, now has 5000 features. 
Random Forest F1 Score: 0.8446706638485095

Random Forest Classifier, max_depth
Max depth: 3, Score: 0.8169109836413851
Max depth: 5, Score: 0.8211599745060548
Max depth: 7, Score: 0.8208625451455279
Max depth: 10, Score: 0.8268111323560654
Max depth: 15, Score: 0.8299978755045677
Max depth: 20, Score: 0.8336944975568302
Max depth: None, Score: 0.8469513490545996

Basic LightGBM model setup

Dummy Classifier (Baseline): 50.15%
This is the baseline - essentially random guessing Any model significantly above this shows real predictive power

Logistic Regression: Best Overall Performer
Train: 91% accuracy, Test: 88% accuracy Excellent generalization (only 3% drop from train to test) High precision across all metrics (F1, APS, ROC AUC all ~95%) This suggests TF-IDF features work very well with linear models

Random Forest: Good but Overfitting
Best depth: None (unlimited) with 84.7% F1 The performance keeps improving as depth increases This suggests the model might benefit from more complex tuning

LightGBM: Solid Performance
85.6% accuracy with balanced precision/recall (0.86 each) Good performance for a gradient boosting method Competitive with Random Forest
