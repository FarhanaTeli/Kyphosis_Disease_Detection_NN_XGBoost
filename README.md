# Kyphosis_Disease_Prediction using simple Neural Network model and XGBoost model
**Project Summary:**
In the "Kyphosis disease prediction and Imbalanced Data Handling" project, the objective was to develop a predictive model to identify the presence or absence of kyphosis, a medical condition. The dataset used in the project, named "Kyphosis.csv," contained imbalanced data, making it challenging to build an accurate model. The project's workflow can be summarized as follows:

**1. Data Preprocessing:**

--> The "Kyphosis.csv" dataset was loaded, which initially contained imbalanced data.

--> To address the class imbalance, the Synthetic Minority Over-sampling Technique (SMOTE) was applied to oversample the minority class, creating a balanced dataset.

**2. Label Encoding:**

--> As the target class was originally in string format ("sample"), label encoding was used to convert it into a numeric form.

**3. Feature Scaling:**

--> StandardScaler from scikit-learn was applied to scale the features, ensuring they had a mean of 0 and a standard deviation of 1.

**4. Training-Testing Split:**

--> The dataset was split into training and testing sets, enabling model evaluation.

**5. Model Selection:**

--> Two different models were considered for classification:

----> A Simple Neural Network (NN) model built using PyTorch.

----> An XGBoost model with hyperparameter tuning using GridSearchCV.

**6. Model Training and Evaluation:**

--> The Simple Neural Network model was trained using the Adam optimizer and binary cross-entropy loss for binary classification. Training continued for 100 iterations.

--> The XGBoost model's hyperparameters were optimized using GridSearchCV to identify the best parameter combinations for the Kyphosis dataset.

--> After training both models, they were evaluated on the testing data.

--> Evaluation metrics, such as accuracy, precision, recall, f1 score, classification report, were used to assess the model's performance.

**7. Model Comparison:**

--> The project concluded with the finding that the XGBoost model outperformed the Simple Neural Network model, achieving an accuracy of **0.96**. In contrast, the NN model achieved an accuracy of **0.85**.

The project aimed to demonstrate the process of handling imbalanced data, performing binary classification using machine learning(XGBoost with GridSearchCV) and deep learning(Simple Neural Network) models, and selecting the best-performing model for predicting kyphosis in a medical context.
