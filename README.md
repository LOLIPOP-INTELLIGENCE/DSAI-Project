# DSAI-Project

## Table of Contents

  - [Summary Of Mini-Project](#summary-of-mini-project)
  - [Dataset Source and Practical Motivation](#dataset-source-and-practical-motivation)
  - [Problem Definition](#problem-definition)
  - [Models Used](#models-used)
  - [Conclusion](#conclusion)
  - [Learning Points From This Project](#learning-points-from-this-project)
  - [Video Presentation](#video-presentation)
  - [Practical Implementation of Model](#practical-implementation-of-model)
  - [Contributors](#contributors)

### Summary Of Mini-Project

- A classification model through supervised learning to predict from 30 features of breast-cancer cells within per patient
whether they have Malignant (M) or Benign (B) tumor.
- 10 features describes the mean of different cell features, another 10 on its standard error, and last 10 on the "worst" or largest (mean
of the three largest values)
- A total of 6 different models were evaluated based on accuracy score and recall (TPR) for ranking purposes
- Dataset used is based only in US, Wisconsin data collected from University of Wisconsin

### Dataset Source and Practical Motivation
- Breast cancer is a complex disease that affects millions of people worldwide. 
- We realize that breast cancer screening and diagnosis can be challenging, and errors can have serious consequences for patients. 
- [Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

### Problem Definition
- How can we identify malignant or benign tumor in a patient having breast cancer?
- What tools and methods can we use to arrive at an accurate diagnosis?
- What are the implications of developing such models and what scope do they have in the future?

### Models Used
1. K-Nearest Neighbours
2. Random Forest
3. Decision Tree
4. Naive Bayes
5. Logistic Regression
6. Support Vector Machine

### Conclusion
- All 6 models did generally well with accuracy of over 93% for each
- Mild imbalance found in dataset did not require resampling/upweighting as models works and generalises well 
without the need to do so
- It was found that feature selection through using only 10 (the means of features) out of 30 features for prediction negatively affects model evaluation
- Logistic Regression model performs the best among others w/ 98.245% accuracy with 95.312% recall
- Other models fall behind by at most 5% in accuracy


### Learning Points From This Project
- "The model is just as good as the data it is trained on". 
Hence, improving the quality and quantity of the data will ultimately lead to better model performance
- Reinforce concepts on accuracy, recall, and other evaluation metrics
- Evaluating feature importance
- Learnt that normalising distributions of features does not necessarily improve model performance
- Understood the maths behind all the models we implemented and also learned how to apply them in a given context

### Video Presentation
- [Our Presentation](https://youtu.be/fBFhuGbEOGQ)

### Practical Implementation of Model
Model Implementation: [Breast Cancer Diagnosis](https://huggingface.co/spaces/bamitsmanas/breast-cancer-detection)
#### Demo:


https://user-images.githubusercontent.com/130828926/232226392-03191188-c2c6-4af8-a6db-36d79dffcca4.mp4



### Contributors
- Data preparation & cleaning (Ayub)
- Exploratory Data Analysis (Nahvin)
- Machine Learning Models & Evaluation (Manas)
- As a whole, the entire project structure and steps was discussed and agreed as a group
- Model implementation through HuggingFace Spaces developed by Manas
