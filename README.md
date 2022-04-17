
# Files:

- 1_PreProcessing_RegExp_Balanced.ipynb
- 2_TfIdfCountvectorizerPipeline.ipynb
- 3_Ensemble_LrKnnCartSvmBayes.ipynb
- 4_Keras_Unoptimized.ipynb
- 5_Keras_Tuner.ipynb
- 6_AutoKeras.ipynb
- 7_Keras_Optimized.ipynb

# Files Objectives

- 1_PreProcessing_RegExp_Balanced.ipynb : Clean Files, Balance Number of Males and Females to prevent Skewness

- 2_TfIdfCountvectorizerPipeline.ipynb : Test MultinomialNB; using TfidfTransformer and CountVectorizer to convert inputs

- 3_Ensemble_LrKnnCartSvmBayes.ipynb : Test Ensemble and Individual Models: LogisticRegression, KNeighborsClassifier, DecisionTreeClassifier, SVM, GaussianNB 

- 4_Keras_Unoptimized.ipynb : Unoptimized Keras Model (LSTM)

- 5_Keras_Tuner.ipynb : Keras Tuner to identify "Optimal Params" 

- 6 AutoKeras.ipynb : Auto Keras to identify "Optimal Params" 

- 7_Keras_Optimized.ipynb : Optimized Keras Model (LSTM)

# Accuracy Comparison
- 2_TfIdfCountvectorizerPipeline.ipynb : 0.5900

- 3_Ensemble_LrKnnCartSvmBayes.ipynb : 
  - lr 0.749
  - knn 0.801
  - cart 0.812
  - svm 0.820
  - bayes 0.683
  - stacking 0.841

- 4_Keras_Unoptimized.ipynb : 
  - Training accuracy: 0.8357 
  - Valid acc : 0.8390

- 5_Keras_Tuner.ipynb : 
  - Training Accuracy: 0.8847
  - Valid Accuracy: 0.8818

- 6_AutKeras : 
  - Training accuracy: 0.8333

- 7_Keras_Optimized.ipynb : 
  - Training accuracy: 0.9754
  - Valid acc 0.9246
  - Test acc 0.9081
# Docker
### Pulling Docker Image and running containers: 
#### Pulling use:
- docker pull jjjj636/rea:0.0.1
#### To ensure pulling is done correctly use:
- docker container run jjjj636/rea:0.0.1
#### Run Notebooks to ensure it is working:
- docker container run jjjj636/rea:0.0.1 ipython 1_PreProcessing_RegExp_Balanced.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 2_TfIdfCountvectorizerPipeline.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 3_Ensemble_LrKnnCartSvmBayes.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 4_Keras_Unoptimized.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 5_Keras_Tuner.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 6_AutoKeras.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 7_Keras_Optimized.ipynb
- docker container run jjjj636/rea:0.0.1 ipython 8_Tuned_Fine_Tuned_BERT.ipynb
