# HEALTH-INSURANCE-CROSS-SELL-PREDICTION
<h2></h2>

# Problem Statement
Problem Statement: An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer. Just like medicalinsurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer. So we tried our best to build a model to predict whether a customer would be interested in Vehicle Insurance or not.

# Summary
1. From the exploratory data analysis where we tried to dig insights from the
data in hand. Those are
* Customers of age between 30 to 60 are more likely to buy insurance.
* Customers with Driving License have a higher chance of buying Insurance.
* Customers with Vehicle_Damage are likely to buy insurance.
* We come to know which features are affecting the target variable and
which are not.
* The target variable (Response column) is highly imbalance.
2. Use level encoding on vehicle_damge, vehicle_age and gender columns.
3. For feature selection we use ExtraTreesClassifier Driving_License , Gender is contributing very less that's why I'm removing those columns.
4. For handling the imbalance dataset I used RandomOverSampler to resample the dataset.
5. For model building I used Logistic Regression, RandomForest Classifier, XGBClassifier and RandomForest Classifier with GridSearchCV (Hyperparameter Tuning)
6. The RandomForest Classifier with GriedSearchCV is the best model.
