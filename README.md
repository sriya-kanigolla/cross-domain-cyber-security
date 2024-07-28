# ***Cross-Domain Cybersecurity: Integrated Intrusion Detection Framework***
This repository is a code storage for my Mini Project submission towards department of ***CSE(AI&ML)*** @ ***Vardhaman College of Engineering*** 

## Dataset Used: NSL-KDD Train Dataset
The NSL-KDD dataset is a refined version of the KDD Cup 1999 dataset, which was created for network intrusion detection research. The primary purpose of the NSL-KDD dataset is to evaluate the performance of various intrusion detection systems. It addresses some of the inherent issues in the original KDD dataset, such as the presence of redundant records, by eliminating duplicate records and normalizing the number of records in different classes. The dataset consists of various network traffic features and labels that classify the traffic into normal or different types of attacks, such as DOS, Probe, U2R, and R2L. This makes it a widely used benchmark for evaluating the effectiveness of intrusion detection models.
It has `42` features and `25192` observations

## Proposed Model
The proposed ensembled model integrates a CNN-GRU architecture with a simulated XGBoost layer to enhance predictive performance. The CNN-GRU component extracts complex spatial and temporal features from the input data, with the CNN capturing local patterns and the GRU handling sequential dependencies. The outputs of these layers are concatenated and combined with the original input features to create a comprehensive feature set. This combined feature set is then passed through dense layers, simulating the functionality of an XGBoost model to produce the final prediction. This ensemble approach leverages the strengths of both deep learning and gradient boosting techniques, aiming to improve accuracy and robustness in classification tasks.

## Results
| Classifier	                        |  Accuracy	  | Precision   |	Recall  |	F1-Score | 
| ----------------------------------- | ----------- | ----------- | ------- | -------- | 
| Proposed Ensembled Model	          |  99.77%	    | 99.61%	    | 99.74%	| 99.67%	 |
