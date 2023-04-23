# SC1015-Credit-Card-Fraud  
Dataset: https://www.kaggle.com/datasets/mishra5001/credit-card?resource=download  
Using the dataset, this project aims to gather insights on credit card defaultees and create a model suitable for detecting if a credit card applicant will default.  
We aim the examine the risk of customers defaulting on loans and the variables which are indicators of defaultees.  

## Usage
Juptyer Notebook / Google Colab

1. Download through the link provided above or use the Kaggle API.
2. Run the code in juptyer notebook or google colab.

## Insights
| model    | train_acc | test_acc | precision | recall | f1_score |
|----------|-----------|----------|-----------|--------|----------|
| dec_tree | 0.919     | 0.919    | 0.0       | 0.0    | 0.0      |
| rfc      | 0.984     | 0.918    | 0.229     | 0.004  | 0.007    |
| knn      | 0.927     | 0.902    | 0.130     | 0.036  | 0.057    |
| gnb      | 0.913     | 0.914    | 0.068     | 0.005  | 0.010    |
  
After Smote:
| model    | train_acc | test_acc | precision | recall | f1_score |
|----------|-----------|----------|-----------|--------|----------|
| dec_tree | 0.725     | 0.692    | 0.089     | 0.309  | 0.139    |
| rfc      | 0.993     | 0.897    | 0.128     | 0.048  | 0.070    |
| knn      | 0.926     | 0.724    | 0.097     | 0.293  | 0.146    |
| gnb      | 0.497     | 0.893    | 0.063     | 0.023  | 0.034    |

Accuracy is not everything. Recall and F1_score are better parameters at evaluating if the model will detect if customer defaults.

## Credits
Jerald  
Bryan  
Jonathan  

References:  
https://www.kaggle.com/code/nareshbhat/fraud-detection-feature-selection-over-sampling  
https://www.kaggle.com/code/vamsichennakesava/credit-card-fraud-detection  
