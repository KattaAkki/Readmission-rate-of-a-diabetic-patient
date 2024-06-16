**Business Context**:  To check if a patient will be re-admitted to the hospital after getting admitted once. 

This Jupyter Notebook serves as a comprehensive guide to building and fine-tuning machine learning models for various classifiers. This notebook will explore the process of model selection, training, and hyperparameter optimization for four different classifiers: Random Forest, XGBoost, Decision Tree, and Support Vector Machine (SVM).

1.**Model Selection**: We introduce the five machine learning classifiers (Random Forest, XGBoost, MLP Classifier, Decision Tree, and SVM) and discuss their strengths and weaknesses in the context of the problem we are solving.

2. **Model Training and Evaluation**: For each classifier, we fit the model to the preprocessed data and evaluate its performance using appropriate metrics. This section includes model training and initial performance assessment.

3. **Hyperparameter Tuning**: To optimize the models, we conduct hyperparameter tuning using techniques like RandomizedSearchCV and GridSearchCV. This step aims to find the best set of hyperparameters.

4. **Results and Comparative Analysis**: We compare the performance of each tuned model, highlighting their strengths and weaknesses. This section provides insights into which classifier performs best for the given problem.

**Process**:

1- Data Preprocessing  

![image](https://github.com/KattaAkki/Readmission-rate-of-a-diabetic-patient/assets/71118330/78b15ed8-3f58-4e86-a20a-9b8f06d47919)


2- Identifying the desired metric for our model 

3- Fitting on various Machine Learning Models  

4- Testing on Validation data 

5- Hyperparameter Tuning to identify the best parameters 

6- Selecting the best model based on the desired metric 

**Inference**:

While AUC provides an overview of the models' ability to separate classes, the focus on recall is crucial in this scenario. The problem statement highlights the importance of minimizing False Negatives (missing at-risk patients) as a primary concern. Therefore, the models should prioritize recall over precision.

Random Forest, XGBoost, and SVM exhibit similar AUC scores, but Random Forest and XGBoost outperform SVM and the Decision Tree in recall. This suggests that Random Forest and XGBoost are better at identifying patients at risk of early readmission.

The performance of the Decision Tree is notably lower, with both lower AUC and recall scores. This may indicate that the Decision Tree struggles to capture the complexities of the dataset and requires further refinement.


![image](https://github.com/KattaAkki/Readmission-rate-of-a-diabetic-patient/assets/71118330/66936dda-af3f-4d12-8401-3ac07a85edac)
