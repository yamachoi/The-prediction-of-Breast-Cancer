# The-prediction-of-Breast-Cancer
Breast cancer is the most common malignancy in women worldwide. Fine needle aspiration (FNA) cytology is widely adopted for the pathologic assessment to breast cancer nowadays when there is a breast lump or an abnormal mammogram. A successful of artificial intelligence system could elevated the efficiency and accuracy of the diagnosis in breast cancer and the subsequent clinical management of patients. We are aimed to target the most important features over all cell nuclei characteristics and describe the best performance model in predicting benign or malignant breast cancer.

## 1. Dataset description
The databset was obtained from the University of Wisconsin Hospitals, Madison from Dr. William H. Wolberg. Samples arrived periodically as Dr. Wolberg reports his clinical cases. The database therefore reflects this chronological grouping of the data. The database contains missing values denoted by "?". 
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
### Or use the codes below :
     ! wget --no-check-certificate \
    'https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/breast-cancer-wisconsin.names' \
     -O breast-cancer-wisconsin.names

     ! wget --no-check-certificate \
    'https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/breast-cancer-wisconsin.data' \
    -O breast-cancer-wisconsin.data


## 2. Attributes
Attributes are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. A few of the images can be found at http://www.cs.wisc.edu/~street/images/. Number of Attributes is 10 plus the class attribute. The cytological characteristics of breast FNAs were valued on a scale of 1 to 10 with 1 being the closest to benign and 10 the most anaplastic.
|  | Attribute| Domain| Desciption|
|:-----------:|:-----------|:-----------:|:-----------|
| 1 | Sample code number (id)|  |id number|
| 2 | Clump Thickness (clp_th)|1 - 10|Benign cells tend to be grouped in monolayers, while cancerous cells often in multilayers|
| 3 | Uniformity of Cell Size (c_size)|1 - 10|Cancer cells tend to vary in size and shape|
| 4 | Uniformity of Cell Shape (c_shape)|1 - 10|Cancer cells tend to vary in shape and size|
| 5 | Marginal Adhesion (ma)         |1 - 10|Normal cells tend to stick together while cancer cells tend to lose|
| 6 | Single Epithelial Cell Size (epi_size)|1 - 10|Related to the uniformity mentioned above. Epithelial cells that significantly enlarged may be a malignant cell|
| 7 | Bare Nuclei (BN)                   |1 - 10|Nuclei not surrounded by cytoplasm (the rest of the cell). Those are typically seen in benign tumors|
| 8 | Bland Chromatin (BC)               |1 - 10|Malignant cells are coarse while the benign cells display a very fine nucleus|
| 9 | Normal Nucleoli (NN)               |1 - 10|Malignant cells have prominent nucleolus and in certain cases have more than one nucleolus|
| 10 | Mitoses (Mito)                      |1 - 10|Malignant cells tend to have higher mitotic activities|
| 11 | Class                        |2,4|2 for benign, 4 for malignant|


## 2. Prerequisites
### Use jupyter notebook(python) to open this project. Followings are the packages/libraries needed:
      python                3.7.13
      jupyter               1.0.0
      IPython               5.5.0
      ipykernel             4.10.1
      ipywidgets            7.7.0
      jupyter_client        5.3.5
      jupyter_core          4.10.0
      nbclient              0.6.0
      nbconvert             5.6.1
      nbformat              5.3.0
      notebook              5.3.1
      qtconsole             5.3.0
      traitlets             5.1.1 
      numpy                 1.21.6
      pandas                1.3.5
      matplotlib            3.2.2
      seaborn               0.11.2
      sklearn               0.0
      sklearn-pandas        1.8.0
      tensorflow            2.8.0
      tensorflow-datasets   4.0.1
      scipy                 >= 1.6

## 3. Tasks
* The important cytology feature selection
* The best predictive model

## 4. Methods
We split out works in 3 parts:
1. Data processing : data cleaning (Null, duplicates), data splitting(Training,Validation, Test)
2. Feature engineering : 
* Feature distribution : Histogram
* Feature selection : Logistic regression with Recursive feature elimination
3. Model building: the models we used shown as below.
* Model 1:  Logistic Regression
* Model 2:  Support Vector Machine
* Model 3:  Random Forest Classifier
* Model 4:  Gradient Boosting Classifier
* Model 5:  K-Nearest Neighbor (KNN) classification

## 5. License:
This dataset is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.

## 6. Citation:
1.William H. Wolberg and O.L. Mangasarian: "Multisurface method of pattern separation for medical diagnosis applied to breast cytology", Proceedings of the National Academy of Sciences, U.S.A., Volume 87, December 1990, pp 9193-9196.
2.Ashidi, N., Isa, M., Subramaniam, E., Mashor, M.Y., & Othman, N.H. (2007). Fine Needle Aspiration Cytology Evaluation for Classifying Breast Cancer Using Artificial Neural Network. American Journal of Applied Sciences, 4, 999-1008.
3.Diagnose breast cancer from histopathological images using Neural Designer (https://www.neuraldesigner.com/learning/examples/breast-cancer-diagnosis)
4.Sabzevari, M., Martínez-Muñoz, G., Suárez, A. (2018). Randomization vs Optimization in SVM Ensembles. In: Kůrková, V., Manolopoulos, Y., Hammer, B., Iliadis, L., Maglogiannis, I. (eds) Artificial Neural Networks and Machine Learning – ICANN 2018. ICANN 2018. Lecture Notes in Computer Science(), vol 11140. Springer, Cham. https://doi.org/10.1007/978-3-030-01421-6_40
5.ANNUAL REPORT OF MACAO CANCER REGISTRY (2019). Health Bureau of the Government of Macao Special Administrative Region. 1st edition, Macao, JULY 2021
6.R. Rajbharath, L. Sankari, Dr. G. Tholkappia Arasu, 2017, Predicting Breast Cancer using Novel Approach in Data Analytics, INTERNATIONAL JOURNAL OF ENGINEERING RESEARCH & TECHNOLOGY (IJERT) Volume 06, Issue 05 (May 2017), http://dx.doi.org/10.17577/IJERTV6IS050018
7.Fine Needle Aspiration (FNA) of the Breast. American Cancer Society medical information, January 14, 2022 (https://www.cancer.org/cancer/breast-cancer/screening-tests-and-early-detection/breast-biopsy/fine-needle-aspiration-biopsy-of-the-breast.html)
8.Mendoza, P., Lacambra, M., Tan, P. H., & Tse, G. M. (2011). Fine needle aspiration cytology of the breast: the nonmalignant categories. Pathology research international, 2011, 547580. https://doi.org/10.4061/2011/547580
9.Somani A, Hwang JS, Chaiwun B, Tse GM, Lui PC, Tan PH. Fine needle aspiration cytology in young women with breast cancer: diagnostic difficulties. Pathology. 2008 Jun;40(4):359-64. doi: 10.1080/00313020802035881. PMID: 18446625.
10.Baba AI, Câtoi C. Comparative Oncology. Bucharest (RO): The Publishing House of the Romanian Academy; 2007. Chapter 3, TUMOR CELL MORPHOLOGY. Available from: https://www.ncbi.nlm.nih.gov/books/NBK9553/
11.Cangiarella, J., & Simsir, A. (2013). Advantages and disadvantages of FNA and core biopsies: Diagnostic accuracy and precision for aspiration biopsy in the diagnosis of lesions of the breast. In J. Cangiarella, A. Simsir, & S. Tabbara (Eds.), Breast Cytohistology (Cytohistology of Small Tissue Samples, pp. 19-26). Cambridge: Cambridge University Press. doi:10.1017/CBO9780511979941.002

