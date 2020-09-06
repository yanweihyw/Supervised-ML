# Supervised-ML-Module 17 Challenge
The result of the resampling module is as follows:
Naive Random Oversampling
balanced_accuracy_score: 0.6504
confusion_matrix:
array([[   70,    31],
       [ 6711, 10393]], dtype=int64)
classification_report_imbalanced:
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.69      0.61      0.02      0.65      0.42       101
   low_risk       1.00      0.61      0.69      0.76      0.65      0.42     17104

avg / total       0.99      0.61      0.69      0.75      0.65      0.42     17205

SMOTE Oversampling:
balanced_accuracy_score: 0.6622
confusion_matrix:
ray([[   64,    37],
       [ 5291, 11813]], dtype=int64)
classification_report_imbalanced:

                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.63      0.69      0.02      0.66      0.44       101
   low_risk       1.00      0.69      0.63      0.82      0.66      0.44     17104

avg / total       0.99      0.69      0.63      0.81      0.66      0.44     17205
Undersampling
balanced_accuracy_score: 0.5442
confusion_matrix:
array([[   68,    33],
       [10002,  7102]], dtype=int64)
classification_report_imbalanced:
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.67      0.42      0.01      0.53      0.29       101
   low_risk       1.00      0.42      0.67      0.59      0.53      0.27     17104

avg / total       0.99      0.42      0.67      0.58      0.53      0.27     17205
Combination (Over and Under) Sampling
balanced_accuracy_score: 0.6447
confusion_matrix:
array([[  73,   28],
       [7412, 9692]], dtype=int64)
classification_report_imbalanced:
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.72      0.57      0.02      0.64      0.42       101
   low_risk       1.00      0.57      0.72      0.72      0.64      0.40     17104

avg / total       0.99      0.57      0.72      0.72      0.64      0.40     17205
Conclusion:
Based on the final result, SMOTE oversampling has higher balanced accuracy score which is 0.6622. The average recall score is also better: 0.69. The average f1 is also better: 0.81. It has better accuracy and better balance for accuracy and sensitivity and should be chosen as sampling method in this case.
