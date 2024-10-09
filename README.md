# Titanic - Machine Learning from Disaster

This repository contains a solution to the Titanic survival prediction problem, which is part of a Kaggle competition. The objective is to create a machine learning model that predicts whether a passenger survived the Titanic disaster based on certain features such as age, gender, and passenger class.

## Dataset Overview

The dataset contains the following files:

- `train.csv`: The training set containing data about the Titanic passengers, along with the survival outcome (`0 = No`, `1 = Yes`).
- `test.csv`: The test set for which we need to predict the survival of passengers. The survival outcome is not provided.
- `gender_submission.csv`: A sample submission file that assumes all female passengers survived and all male passengers did not. This file is provided as an example of the format required for Kaggle submissions.
  
## Project Files

- `Titanic_Model.ipynb`: Jupyter notebook where the machine learning model is built and trained. This notebook includes data analysis, feature engineering, and model creation using various algorithms. The final predictions are exported from this notebook.
  
- `train.csv`: This is the training dataset used to train the model. It contains the following columns:
  - `PassengerId`: Unique identifier for each passenger.
  - `Survived`: Survival indicator (0 = No, 1 = Yes).
  - `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd).
  - `Sex`: Gender of the passenger.
  - `Age`: Age of the passenger.
  - `SibSp`: Number of siblings/spouses aboard the Titanic.
  - `Parch`: Number of parents/children aboard the Titanic.
  - `Ticket`: Ticket number.
  - `Fare`: Passenger fare.
  - `Cabin`: Cabin number.
  - `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

- `test.csv`: This is the test dataset on which the model is evaluated. It contains the same columns as `train.csv`, except for the `Survived` column, which is the target we are predicting.

- `gender_submission.csv`: This file is a sample submission provided by Kaggle. It assumes all female passengers survived and all male passengers did not survive. It is used as a reference for creating our submission file.

- `submission.csv`: This file contains the final predictions from the model. It is structured in the format required by Kaggle for submission:
  - `PassengerId`: Unique ID of the passenger.
  - `Survived`: Predicted survival (0 = No, 1 = Yes).

## Steps to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Ayirhs1/Titanic-ML-Project.git
   cd Titanic-ML-Project
2. Open the Jupyter notebook/google colab
3. Install the required libraries:
  - pip install -r requirements.txt
    
4. Run all cells in the notebook to preprocess the data, train the model, and generate predictions.
5. Save the predictions in a file named submission.csv for Kaggle submission.
