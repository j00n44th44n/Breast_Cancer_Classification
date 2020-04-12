# Udemy - Machine Learning Practical 6 Real-World Applications
### SVM Breast Cancer Classification
###### https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)
> `Steps`
1. Importing Data and Libreries
2. Data Visualization
3. Model Training
4. Model Evaluation
4.1 Confusion Matrix
    CM | +       | -
    ---|---------|--------
     + | True +  | False +
     - | False - | True -
 


5. Improving the Model
5.1 Data Normalization
    `X' = (X - Xmin) / (Xmax - Xmin)`
5.2 Parameters Optimization
    `C parameter` : trade-off between classifying training points to get a smooth decision boundry 
    + small C (penalty of misclassification)    C => underfiting
    + large C (cost of misclassification high)  C => overfiting
    
    `Gamma Parameter` : controls how far the influence of a single training set reaches
    + small gamma: far reach (more generalized solution)
    + large gamma: close reach (closer data points have high weight) overfiting
5.3 Sklearn had a function to optimize those parameters values