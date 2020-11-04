# Machine-Learning

## Finding Risky Business

### Sampling

Resampling the data using different techniques and analysing the probability of business being risky:

The data has originally 68,470 low risk business and 347 high risk business entries. And the features of data are scaled using standard scaler before resampling.

#### Over Sampling

1. Random Over-Sampling

Using random over sampler, the number of samples are adjusted to 51,352 samples sfor low risk and high risk loan types.

The balanced accuracy store is 0.63

The model f1 for low risk is 0.81 and high risk is 0.02
Recall for low risk is 0.68 and high risk is 0.59
Precison for low risk is 1 and high risk is 0.01
Geometric mean is 0.63

2. SMOTE Over-Sampling

Using SMOTE over sampler, the number of samples are adjusted to 51,352 samples for low risk and high risk loan types.

The balanced accuracy store is 0.65

The model f1 for low risk is 0.77 and high risk is 0.02
Recall for low risk is 0.63 and high risk is 0.67
Precison for low risk is 1 and high risk is 0.01
Geometric mean is 0.65

** From above specifics, for the data, random over sampling gave better predictions compared to SMOTE over sampling**

#### Under Sampling

1. Cluster Centroids

Using Cluster Centroids under sampler, the number of samples are adjusted to 260 samples for low risk and high risk loan types.

The balanced accuracy store is 0.52

The model f1 for low risk is 0.57 and high risk is 0.01
Recall for low risk is 0.40 and high risk is 0.63
Precison for low risk is 1 and high risk is 0.01
Geometric mean is 0.51

#### Combination Sampling

1. SMOTEENN Sampling

Using SMOTEENN Sampling sampler, the number of samples are adjusted to 51,344 samples for high risk and 46,388 samples for high risk loan types.

The balanced accuracy store is 0.66

The model f1 for low risk is 0.73 and high risk is 0.02
Recall for low risk is 0.58 and high risk is 0.75
Precison for low risk is 1 and high risk is 0.01
Geometric mean is 0.66

Weighing accuracy and f1 values for all the sampling methods, as recall might not be a best metric for comparison with the type of data. From above assumption the best sampling model can be determined as SMOTE or SMOTEENN.


### Ensemble Learners

Finding the best algorithm for predictions

#### Balanced Random Forest Sampler

Balanced accuracy score for the model is 0.82

The model f1 for low risk is 0.96 and high risk is 0.01
Recall for low risk is 0.93 and high risk is 0.71
Precison for low risk is 1 and high risk is 0.05
Geometric mean is 0.81

#### Easy Ensemble Classifier

Balanced accuracy score for the model is 0.93

The model f1 for low risk is 0.97 and high risk is 0.14
Recall for low risk is 0.95 and high risk is 0.91
Precison for low risk is 1 and high risk is 0.08
Geometric mean is 0.93

Comparing the metrics for both the models, Easy Ensemble Classifier is more accurate to presict the data.