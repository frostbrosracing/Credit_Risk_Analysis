# Credit Risk Analysis using 6 Different Methods

## Project Overview of the Analysis
#### The goal of this project was to analyze the outcomes of six different methods of evaluating credit risk.
Using a dataset from a peer-to-peer lending services company, each of the methods was used to create training and target variables and then make predictions through the use of the `LogisticRegression` classifier.  The accuracy of each model's performance was then evaluated by the calculation of an accuracy score of those predictions.  Finally, a confusion matrix was generated in which the predictions were assigned based on their accuracy and an imbalanced classification report was printed out.  For the purposes of this analysis, two classes were determined:  `low-risk` and `high-risk`.

#### Resources
- Data Source: <br>
`Resources/LoanStats_2019Q1.csv`

- Software:  Jupyter Notebook
- Languages:  Pandas, Python
- Libraries:  `imbalanced-learn`  `scikit-learn`
- Methods: <br>Oversampling  `RandomOverSampler`  `SMOTE`  
            Undersampling  `ClusterCentroids`  
            (Over and Under) Sampling  `SMOTEENN`  
            Bias Reduction  `BalancedRandomForestClassifier`  `EasyEnsembleClassifier`
  
## Results of the Analysis
* The balanced accuracy score of the Naive Random Oversampling is 65.14%

![NaiveRandomOversampling](https://user-images.githubusercontent.com/77071776/124400906-8747ff80-dceb-11eb-8a03-f371db85f173.PNG)

* The balanced accuracy score of the SMOTE Oversampling is 62.67%

![SmoteOversampling](https://user-images.githubusercontent.com/77071776/124400916-97f87580-dceb-11eb-8188-c168a32650c1.PNG)

* The balanced accuracy score of the Cluster Centroids Undersampling is 51.61%

![ClusterCentroidsUndersampling](https://user-images.githubusercontent.com/77071776/124400921-a8a8eb80-dceb-11eb-8a86-8930bd1de49d.PNG)

* The balanced accuracy score of the SMOTEENN (Over and Under) Sampling is 62.48%

![SMOTEENN](https://user-images.githubusercontent.com/77071776/124400926-b8283480-dceb-11eb-8890-1ff3949c8ccf.PNG)

* The balanced accuracy score of the Balanced Random Forest Classifier is 78.78%

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/77071776/124400947-dc841100-dceb-11eb-83e0-3decd43cd269.PNG)

* The balanced accuracy score of the Easy Ensemble Classifier is 92.54%

![EasyEnsembleClassifier](https://user-images.githubusercontent.com/77071776/124400951-e279f200-dceb-11eb-8ece-d29a3ec4695f.PNG)



## Summary
Because of the significance of the imbalance between the low-risk and high-risk class, the precision in the classification report isn't going to represent the entire story.  IN this case, the recall (or accuracy) score should share more of the story.  
