# DTI-CDF
Drug-target interactions play a crucial role in target-based drug discovery and exploitation. Computational prediction of DTIs has become a popular alternative strategy to the experimental methods for identification of DTIs of which are both time and resource consuming. However, the performances of the current DTIs prediction approaches suffer from a problem of low precision and high false positive rate. In this study, we aimed to develop a novel DTIs prediction method, named DTI-CDF, for improving the prediction precision based on a cascade deep forest model which integrates hybrid features, including multiple similarity-based features extracted from the heterogeneous graph, fingerprints of drugs, and evolution information of target protein sequences. In the experiments, we built five replicates of 10 fold cross-validations under three different experimental settings of data sets, namely, corresponding DTIs values of certain drugs (S_D), targets (S_T), or drug-target pairs (S_P) in the training set are missed but existed in the test set. The experimental results show that our proposed approach DTI-CDF achieves significantly higher performance than the state-of-the-art methods.

#-----------------------------------------------------------------------------------------------------------------------------

Note-1: When installing gcforest, use the code provided by this page, dir：DTI-CDF/gcforest, because the source code has been modified. Also, note that the first line {#y_pred = np.argmax(y_pred_proba, axis=1)} in the xgb_eval_accuracy(y_pred_proba, y_true) function in the DTI-CDF/gcforest/exp_utils.py file is used for tunable parameters, you need to add or remove comments. 

#-----------------------------------------------------------------------------------------------------------------------------

Note-2: Python2.7 environment configuration: pip install -r DTI-CDF_requirements.txt

#-----------------------------------------------------------------------------------------------------------------------------

Note-3: In the code folder, all the code of the NR data set is provided. Please run the code in order, first generate PsePSSM and data set, and then train. You can get the correlation between the three types of features by running the number 4 code.
Note: Modify the path in the code. To run other datasets, simply change the path to the original file.
