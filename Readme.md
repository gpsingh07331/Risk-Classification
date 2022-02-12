### Risk classification using Supervised classification models.
In this project we have used various classification models on a imbalanced data set for assessing risk for granting loans.
The project has been split in two notebooks.
- *Credit_Risk_Resampling.ipynb*
- *Credit_Risk_Ensemble.ipynb*

**Credit_Risk_Resampling**, in this notebook we have analyzed the lending_data.csv data. We have used simple logistic regression and then considering that the data is imbalanced for the target variable, we have used oversampling, undersampling and combined sampling and then applied logistic regression.
Some of the sampling methods applied are -

- Naive Random Oversampler and SMOTE algorithms
- Cluster Centroids algorithm undersmpling
- Over- and undersample using a combination SMOTEENN algorithm

We use balanced_accuracy_score, confusion_matrix and classification_report to asses the quality of the models and in the end compare and answer few questions.

---

![alt text](https://github.com/RutgersCodingBootcamp/RUT-VIRT-FIN-PT-11-2021-U-C/raw/main/Homework/11-Machine-Learning/Instructions/Images/credit-risk.jpg)

---

We use Pandas, hvplot and pandas_profiler to do exploratory data analysis.

For categorical values and the target value, we did encoding -

<img src="./IMG/sample_encoding.PNG" width="800" height="400">

Output of summary of profile after EDA and transformation

<img src="./IMG/sample_profile1.PNG" width="800" height="400">

**Results**

*Which model had the best balanced accuracy score?*
Too close to call but SMOTEENN is the best.

<img src="./IMG/>sample_ba.PNG" width="800" height="400">
     
*Which model had the best recall score?*
LogisticRegression is the best.
     
<img src="./IMG/>sample_recall.PNG" width="800" height="400">

*Which model had the best geometric score?*
Too close to call but SMOTEENN is the best.

<img src="./IMG/>sample_gm.PNG" width="800" height="400">
