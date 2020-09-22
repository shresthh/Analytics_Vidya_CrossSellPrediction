# Analytics_Vidya_CrossSellPrediction

Participated in Analytics_Vidya_CrossSellPrediction Hackathon to predict whether a person will be interested or not to buy insurance based on various features available like id , gender, age, driving lincense, region_code, previously_insured , vehicle_age, vehicle_damage, annual_preimium, policy_sales_channel, and vintage

and target variable as "Response" - 1 :  Customer is interested, 0 : Customer is not interested

## Algorithms Used-

1. XGBOOST (low accuracy)
2. LGBMClassifier with hyperparameter tuning

## Accuracy achieved 

85.76 in public leaderboard
86.22 in private leaderboard

## What led to such accuracy-

-Hyperparameter tuning using grid search and random search cv

## RandomSearch. best params-

{'colsample_bytree': 0.5,
 'gamma': 0.9,
 'learning_rate': 0.03,
 'max_depth': 14,
 'min_child_weight': 0.01,
 'n_estimators': 400,
 'reg_alpha': 1,
 'reg_lambda': 2}
 
 ## Random search best estimators
 
 LGBMClassifier(boosting_type='gbdt', class_weight=None, colsample_bytree=0.3,
               gamma=0.9, importance_type='split', learning_rate=0.01,
               max_depth=14, min_child_samples=20, min_child_weight=0.01,
               min_split_gain=0.0, n_estimators=800, n_jobs=-1,is_unbalance = True, num_leaves=31,
               objective='binary',metric = 'auc', random_state=294, reg_alpha=1, reg_lambda=2,
               silent=True, subsample=1.0,njobs = -1, subsample_for_bin=200000,
               subsample_freq=0)
               
