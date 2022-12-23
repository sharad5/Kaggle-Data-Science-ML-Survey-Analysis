# Kaggle Data Science & Machine Learning Survey Analysis
This is a capstone project for Introduction to Data Science (DS-GA 1001) at [NYU Center for Data Science](https://cds.nyu.edu/). 

## Project Intro/Objective
The purpose of this project is to understand the state of Data Science and Machine Learning across industries and technologies.

### Methods Used
* Inferential Statistics
* Data Visualization
* Predictive Modeling
* Clustering
* Supervised Classification

### Technologies
* Python
* Pandas, jupyter
* Sklearn

## Project Description
We are using Kaggle annual data science and machine learning survey responses data from 2022 and previous years. 
Data Sources: 
* [2022 Kaggle Machine Learning & Data Science Survey](https://www.kaggle.com/competitions/kaggle-survey-2022/data)
* [2021 Kaggle Machine Learning & Data Science Survey](https://www.kaggle.com/competitions/kaggle-survey-2021/data)
* [2020 Kaggle Machine Learning & Data Science Survey](https://www.kaggle.com/competitions/kaggle-survey-2020/data)

Inferential Statistics:
* [Hypothesis](https://github.com/sharad5/Kaggle-Data-Science-ML-Survey-Analysis/blob/main/Hypothesis%20Testing%20(Sargun).ipynb): What Data Science jobs have the highest salaries?
* [Hypothesis](https://github.com/sharad5/Kaggle-Data-Science-ML-Survey-Analysis/blob/main/Hypothesis%20Testing%20(Sharad).ipynb): Is the representation of Advanced degrees (Masters & above) among Data Professionals increasing over years?

[Salary prediction](https://github.com/sharad5/Kaggle-Data-Science-ML-Survey-Analysis/blob/main/Salary%20Prediction%20-%20Sargun.ipynb): Predict data science job salaries of individuals in the United States based on covariates such as their job title, industry, skill sets and experience.
Results:
|   |     Model     | Train R² | Test R² | Adj Train R² | Adj Test R² |
|:-:|:-------------:|:--------:|:-------:|:------------:|:-----------:|
| 1 |      OLS      |   0.159  |   0.18  |     0.389    |    0.393    |
| 2 |     Ridge     |   0.151  |  0.186  |     0.388    |    0.393    |
| 3 |     Lasso     |   0.157  |  0.184  |     0.386    |    0.392    |
| 4 |   Linear SVR  |   0.092  |  0.113  |     0.306    |    0.298    |
| 5 | Random Forest |   0.863  |  0.165  |     0.674    |    0.399    |
| 6 |    XGBoost    |   0.433  |  0.178  |     0.516    |    0.404    |
| 7 |  Poisson GLM  |   0.182  |  0.223  |     0.396    |    0.401    |


[Clustering](https://github.com/sharad5/Kaggle-Data-Science-ML-Survey-Analysis/blob/main/Clustering%20-%20v2%20-%20Harsha.ipynb): Clustering the survey respondents into clusters based on their skills and expeiriences
Approach:
* Traditional KMeans clustering using only numerical data.
* KPrototypes clustering, which is compatible with categorical information as described by [Huang (1998)](https://link.springer.com/article/10.1023/A:1009769707641)

[Classification](https://github.com/sharad5/Kaggle-Data-Science-ML-Survey-Analysis/blob/main/Classification.ipynb):  Identify the most suitable jobs for a user based on the user’s responses about their skills, exposure and experience.
Results:
|                     Model | Accuracy | F1-Score | Top 2 accuracy |
|--------------------------:|:--------:|:--------:|:--------------:|
| Dummy Classifier          |    35%   |   0.10   |       65%      |
| Decision Tree             |    41%   |   0.41   |      51.9%     |
| KNN Classifier            |    42%   |   0.33   |      62.6%     |
| Random Forest             |    48%   |   0.44   |      69.0%     |
| SVM                       |    47%   |   0.45   |      78.6%     |
| Multinomial Logisitic Reg |    48%   |   0.45   |      71.8%     |
| Multi-Layer Perceptron    |    54%   |   0.43   |      78.8%     |
| XGBoost                   |    54%   |   0.45   |      79.1%     |
| LightGBM                  |    55%   |   0.45   |     79.62%     |


Findings and analysis: [Report](https://github.com/sharad5/Kaggle-Data-Science-ML-Survey-Analysis/blob/main/Project%20Report.pdf)

### Team Members

|Name     |  Github   | 
|---------|-----------------|
|[Sargun Nagpal](https://www.linkedin.com/in/sargun-nagpal/)|  [sargun-nagpal](https://github.com/sargun-nagpal)       |
|[Harsha Koneru](https://www.linkedin.com/in/harshakoneru/) |  [harshakoneru](https://github.com/harshakoneru)    |
|[Sharad Dargan](https://www.linkedin.com/in/sharaddargan/) |  [sharaddargan](https://github.com/sharad5)    |
