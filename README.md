# Shinkansen-Customer-Experience

# Shinkansen Travel Experience Prediction

## Problem Statement
This project focuses on analyzing passengers' experiences while traveling on the Shinkansen Bullet Train in Japan. The goal is to develop a machine learning model that predicts whether a passenger was satisfied with their overall travel experience based on various parameters.

## Dataset Overview
The dataset consists of two separate files:
1. **Traveldata_train.csv** - Contains passenger details and attributes related to their journey on the Shinkansen.
2. **Surveydata_train.csv** - Aggregated survey responses capturing post-service experiences, including overall satisfaction.

Both datasets are provided in the `Dataset` folder, with separate train and test splits:
- **Train_Data**: Used to train the model.
- **Test_Data**: Used to evaluate model performance on unseen data.

## Target Variable
The variable **Overall_Experience** represents passenger satisfaction:
- `1` = Satisfied
- `0` = Not Satisfied

## Objective
The aim is to determine which parameters most influence passenger satisfaction and use this understanding to predict the overall travel experience of new passengers.

## Approach
1. **Data Preprocessing**
   - Cleaning and handling missing values.
   - Merging travel and survey datasets.
   - Feature engineering and selection.
2. **Model Development**
   - Testing multiple classification models (Logistic Regression, Random Forest, etc.).
   - Hyperparameter tuning for optimal performance.
3. **Evaluation**
   - The model will be evaluated based on **accuracy**, calculated as:
     \[ Accuracy = \frac{(True Positives + True Negatives)}{Total Observations} \]

## Submission Format
The output should be a CSV file with **35,602** entries and two columns:
| ID  | Overall_Experience |
|-----|--------------------|
| 1   | 1                |
| 2   | 0                |

## Repository Structure
```
├── Dataset
│   ├── Train_Data
│   ├── Test_Data
├── notebooks
│   ├── data_preprocessing.ipynb
│   ├── model_training.ipynb
├── models
├── submission.csv
├── README.md
```

## Evaluation Criteria
The model's performance is determined by its **accuracy score**, with the highest possible score being **100%**.

## Next Steps
- Fine-tuning models to improve accuracy.
- Feature importance analysis to gain insights into key travel experience factors.
- Deploying the model for real-time predictions.

