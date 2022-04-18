
# Files:

- 1_PreProcessing_RegExp_Balanced.ipynb
- 2_TfIdfCountvectorizerPipeline.ipynb
- 3_Ensemble_LrKnnCartSvmBayes.ipynb
- 4_Keras_Unoptimized.ipynb
- 5_Keras_Tuner.ipynb
- 6_AutoKeras.ipynb
- 7_Keras_Optimized.ipynb
- 8_Tuned_Fine_Tuned_BERT.ipynb

# Files Objectives And Rationales

- 1_PreProcessing_RegExp_Balanced.ipynb : Clean Files, Balance Number of Males and Females to prevent Skewness

- 2_TfIdfCountvectorizerPipeline.ipynb : Test MultinomialNB; using TfidfTransformer and CountVectorizer to convert inputs
  - Identify Baseline Accuracy before moving to NeuralNetwork Based Models; it is never wise to move straight to over complicated models.

- 3_Ensemble_LrKnnCartSvmBayes.ipynb : Test Ensemble and Individual Models: LogisticRegression, KNeighborsClassifier, DecisionTreeClassifier, SVM, GaussianNB 
  - Test classic ML Algorithms and subsequently, ensembles. After having a good idea of accuracy of baseline models, we can move on to NN-based Models

- 4_Keras_Unoptimized.ipynb : Unoptimized Keras Model (LSTM)
  - Untuned HyperParameters

- 5_Keras_Tuner.ipynb : Keras Tuner to identify "Optimal Params" 
    - Use Keras Tuner to Tune HyperParameters

- 6 AutoKeras.ipynb : Auto Keras to identify "Optimal Params" 
  - Use AutoKeras to Tune HyperParameters

- 7_Keras_Optimized.ipynb : Optimized Keras Model (LSTM)
  - Tuned HyperParameters

- 8_Tuned_Fine_Tuned_BERT.ipynb
  - Fine tuning Bert for Gender Identification

# Bird Eye View of Accuracy Comparison
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

- 6_AutoKeras : 
  - Training accuracy: 0.8333

- 7_Keras_Optimized.ipynb : 
  - Training accuracy: 0.9754
  - Valid acc 0.9246
  - Test acc 0.9081

- 8_Tuned_Fine_Tuned_BERT.ipynb :
  - Valid acc 0.8798
 
# Docker
### Pulling Docker Image and running containers: 
#### To Pull, use:
- docker pull jjjj636/rea:0.0.2
#### To ensure pulling is done correctly use:
- docker container run jjjj636/rea:0.0.2
#### Run Notebooks to ensure it is working:
- docker container run jjjj636/rea:0.0.2 ipython 1_PreProcessing_RegExp_Balanced.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 2_TfIdfCountvectorizerPipeline.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 3_Ensemble_LrKnnCartSvmBayes.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 4_Keras_Unoptimized.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 5_Keras_Tuner.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 6_AutoKeras.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 7_Keras_Optimized.ipynb
- docker container run jjjj636/rea:0.0.2 ipython 8_Tuned_Fine_Tuned_BERT.ipynb
