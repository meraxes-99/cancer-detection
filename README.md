# Diagnosing Cervical cancer using Machine Learning

![license logo](https://img.shields.io/github/license/adsers/cancer-detection)
![last commit](https://img.shields.io/github/last-commit/adsers/cancer-detection)
![repo size](https://img.shields.io/github/repo-size/adsers/cancer-detection)

Watch project video here:

[![Watch the video](https://drive.google.com/u/0/uc?id=1iOPt05nPLRgNdZHrmxFRdmpINg2sGtZH&export=download)](https://youtu.be/LEvAryBK_ew)

According to the World Health Organisation (WHO), when detected at an early stage, cervical cancer is one of the most curable cancers. Hence, the main motive behind this project is to detect cancer in its early stages so that it can be treated and managed in the patients effectively.

Some facts about Cervical Cancer:
* It is diagnosed most often in women over the age of 30 years.
* The main cause of cervical cancer is long-lasting infection with certain types of human papillomavirus (HPV), which is a common virus that is passed from one person to another during sex.
* At least half of sexually active people will have HPV at some point in their lives, but few women get cervical cancer.
* The only procedure that can confirm cervical cancer is a biopsy. But, conducting a biopsy requires medical expertise and sound infrastructure that may not be available in rural and developing areas. The idea here is to employ machine learning models in these areas which will help screen potential patients.

#

This repository is divided into two parts: 
1) The dataset, a `CSV` file named `risk_factors_cervical_cancer.csv`
2) The jupyter notebook, an `ipynb` file named `Diagnosing Cervical Cancer using Supervised ML.ipynb`

The dataset for tackling the problem is supplied by the UCI repository for Machine Learning. It contains a list of risk factors that lead up to the Biopsy examination.
The aim is to try to predict the 'biopsy' variable from the dataset using four algorithms, namely, <br>

1) Logistic Regression
2) Bagging with Decision Trees
3) Random Forest and,
4) Boosting with XGBoost Classifier.


The results obtained by the four models are summarised below,

|                      Model                      | Accuracy | Precision | Recall | F1 score |  AUC   |
|                       ---                       |   ----   |   -----   |  ----  |   ----   |  ----  |
|               Logistic Regression               |  95.93%  |   66.67%  | 72.73% |  69.57%  | 0.8238 |
|     Bagging with base model as Decision Tree    |  97.09%  |   80.00%  | 72.73% |  76.19%  | 0.8950 |
| Random Forest with Upsampling and class weights |  97.09%  |   80.00%  | 72.73% |  76.19%  | 0.8673 |
|                XGBoost Classifier               |  95.93%  |   66.67%  | 72.73% |  69.57%  | 0.9348 |

#

References: <br>
Link to basic information regarding cervical cancer : https://www.cdc.gov/cancer/cervical/basic_info/index.htm <br>
Link to Dataset : https://archive.ics.uci.edu/ml/datasets/Cervical+cancer+%28Risk+Factors%29
