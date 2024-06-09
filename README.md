# Shinkansen Bullet Train Passenger Satisfaction Prediction

Welcome to the winning solution for the Shinkansen Bullet Train Passenger Satisfaction Prediction hackathon. This project aimed to understand the factors contributing to passenger satisfaction and predict whether a passenger was satisfied with their overall travel experience.

## Project Overview

The project analyzed travel and survey data of passengers on the Shinkansen Bullet Train in Japan. Using machine learning techniques, we predicted passenger satisfaction based on various parameters collected during their journey.

## Data Description

The dataset consists of two main components:

- **Travel Data**: Details about passengers and attributes of the Shinkansen train they used.
- **Survey Data**: Aggregated survey responses indicating passengers' post-service experience.

### Files

- `Traveldata_train.csv`: Training data related to travel.
- `Surveydata_train.csv`: Training data from passenger surveys.
- `Traveldata_test.csv`: Test data related to travel.
- `Surveydata_test.csv`: Test data from passenger surveys.
- `Data_Dictionary.xlsx`: Detailed information about dataset variables and survey levels.

### Target Variable

- `Overall_Experience`: Binary indicator (1 for satisfied, 0 for not satisfied) based on passenger feedback.

## Solution Approach

1. **Data Preprocessing**:
   - Cleaned and validated raw data.
   - Merged travel and survey data using a common identifier.
   - Handled missing values and encoded categorical variables.

2. **Feature Engineering**:
   - Extracted significant features influencing passenger satisfaction.
   - Engineered new features to enhance model performance.

3. **Model Training**:
   - Implemented various classification algorithms including Neural Networks, Random Forest, and XGBoost.
   - Optimized model hyperparameters using GridSearchCV.
   - Ensured model robustness through cross-validation techniques.

4. **Model Evaluation**:
   - Selected the best-performing model based on accuracy and other relevant metrics.
   - Validated model performance on unseen test data.

5. **Prediction**:
   - Predicted `Overall_Experience` for the test data.
   - Generated a submission file adhering to competition requirements.

## Results

The model achieved an impressive accuracy of 95.688% in predicting passenger satisfaction.

## Repository Structure

```
├── data
│   ├── Train_Data
│   │   ├── Traveldata_train.csv
│   │   └── Surveydata_train.csv
│   ├── Test_Data
│   │   ├── Traveldata_test.csv
│   │   └── Surveydata_test.csv
│   └── Data_Dictionary.xlsx
├── notebooks
│   ├── Brakenhoff_Hack1.ipynb
└── README.md
```

## Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/mbrakenhoff/Passenger-Satisfaction-Prediction-Hackathon.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd Passenger-Satisfaction-Prediction-Hackathon
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Explore the notebooks**:
   - Review the data preprocessing steps in `notebooks/Brakenhoff_Hack1.ipynb`.

5. **Note**: The true overall experience ratings for the test set were not disclosed, only the accuracy score. 

## Conclusion

This project successfully identifies critical factors influencing passenger satisfaction on the Shinkansen Bullet Train and provides a reliable model for predicting satisfaction levels.
