# The-prediction-of-Breast-Cancer


## 1. Database description
The databases was obtained from the University of Wisconsin Hospitals, Madison from Dr. William H. Wolberg. Samples arrived periodically as Dr. Wolberg reports his clinical cases. The database therefore reflects this chronological grouping of the data. The database contains missing values denoted by "?". 
### This grouping information :
     Group 1: 367 instances (January 1989)
     Group 2:  70 instances (October 1989)
     Group 3:  31 instances (February 1990)
     Group 4:  17 instances (April 1990)
     Group 5:  48 instances (August 1990)
     Group 6:  49 instances (Updated January 1991)
     Group 7:  31 instances (June 1991)
     Group 8:  86 instances (November 1991)
     -----------------------------------------
     Total:   699 points (as of the donated datbase on 15 July 1992) 
     Class distribution : 458 (65.5%) Benign , 241 (34.5%) Malignant.
Access to the dataset(https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(original)).

## 2. Attributes
Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. A few of the images can be found at http://www.cs.wisc.edu/~street/images/. Number of Attributes is 10 plus the class attribute
|  | Attribute| Domain| Desciption|
|:-----------:|:-----------|:-----------:|:-----------|
| 1 | Sample code number|  |id number|
| 2 | Clump Thickness               |1 - 10|Benign cells tend to be grouped in monolayers, while cancerous cells often in multilayers|
| 3 | Uniformity of Cell Size       |1 - 10|Cancer cells tend to vary in size and shape|
| 4 | Uniformity of Cell Shape      |1 - 10|Cancer cells tend to vary in shape and size|
| 5 | Marginal Adhesion             |1 - 10|Normal cells tend to stick together while cancer cells tend to lose|
| 6 | Single Epithelial Cell Size   |1 - 10|Related to the uniformity mentioned above. Epithelial cells that significantly enlarged may be a malignant cell|
| 7 | Bare Nuclei                   |1 - 10|Nuclei not surrounded by cytoplasm (the rest of the cell). Those are typically seen in benign tumors|
| 8 | Bland Chromatin               |1 - 10|Malignant cells are coarse while the benign cells display a very fine nucleus|
| 9 | Normal Nucleoli               |1 - 10|Malignant cells have prominent nucleolus and in certain cases have more than one nucleolus|
| 10 | Mitoses                      |1 - 10|Malignant cells tend to have higher mitotic activities|
| 11 | Class                        |2,4|2 for benign, 4 for malignant|


## 2. Prerequisites
### We use python to code this project. Below are the packages/libraries needed:
     import numpy as np
     import pandas as pd
     from pandas import DataFrame
     import matplotlib.pyplot as plt
     import seaborn as sns
     from sklearn.impute import SimpleImputer
     from sklearn.model_selection import train_test_split
     from sklearn.preprocessing import StandardScaler
     from sklearn.ensemble import RandomForestClassifier
     from sklearn.inspection import permutation_importance
     from sklearn.decomposition import PCA
     from tensorflow.keras import Sequential
     import tensorflow.keras.layers as L
     import tensorflow as tf
     from sklearn.metrics import confusion_matrix, accuracy_score,classification_report
     import seaborn as sns

## 3. Tasks
* The most important cytology feature
* The best predictive model

## 4. Methods
The models we used show as below.


## License:
This dataset is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.

## Citation:
1. O. L. Mangasarian and W. H. Wolberg: "Cancer diagnosis via linear programming", SIAM News, Volume 23, Number 5, September 1990, pp 1 & 18.
2. William H. Wolberg and O.L. Mangasarian: "Multisurface method of pattern separation for medical diagnosis applied to breast cytology", Proceedings of the National Academy of Sciences, U.S.A., Volume 87, December 1990, pp 9193-9196.
3. O. L. Mangasarian, R. Setiono, and W.H. Wolberg: "Pattern recognition via linear programming: Theory and application to medical diagnosis", in: "Large-scale numerical optimization", Thomas F. Coleman and Yuying Li, editors, SIAM Publications, Philadelphia 1990, pp 22-30.
4. K. P. Bennett & O. L. Mangasarian: "Robust linear programming discrimination of two linearly inseparable sets", Optimization Methods and Software 1, 1992, 23-34 (Gordon & Breach Science Publishers).
5. Ashidi, N., Isa, M., Subramaniam, E., Mashor, M.Y., & Othman, N.H. (2007). Fine Needle Aspiration Cytology Evaluation for Classifying Breast Cancer Using Artificial Neural Network. American Journal of Applied Sciences, 4, 999-1008.
6. https://www.neuraldesigner.com/learning/examples/breast-cancer-diagnosis
7. Zhang, J. (1992). Selecting typical instances in instance-based learning. In Proceedings of the Ninth International Machine Learning Conference (pp. 470--479). Aberdeen, Scotland: Morgan Kaufmann.
