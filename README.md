# Project Breast Cancer Detection
Built a classifier model to detect breast cancer. <br>

Choosing a metric: It is important to set the metric of success before you actually implement the algorithm so you don't cheat. Since I was using an imbalanced dataset, instead of accuracy, I choose sensitivity as the model metric. The sensitivity of a test is its ability to determine the patient cases correctly. To estimate it, we should calculate the proportion of true positive in patient cases. Mathematically, this can be stated as: <br>
Sensitivity = TP / (TP + FN) <br>
TP: True Positive; FN: False Negative <br>

It is also important to know what is the score on the sensitivity metric previously, without using any machine learning algorithms so the metric can tell us whether the machine learning model is indeed better than humans to do the job. <br>

Built multiple models, namely logistic regression classifier, k-Nearest Neigbors (k-NN) classifier, support vector machine (SVM) classifier, kernel SVM classifier, Naive Bayes classifier, Decision Tree classifier, and Random Forest classifier. Code for all these algorithms can be found [here](https://github.com/mehtamishah/Breast-Cancer-Detection). <br>

Best performance was achieved on a k - Nearest neighbors classifier model. On the test set, achieved <br>
Sensitivity = 0.95  #The ability to determine the patient cases (malignant tumors) correctly <br>
Specificity = 0.98  #The ability to determine the healthy cases (benign tumors) correctly <br>
roc_auc_score = 0.97
