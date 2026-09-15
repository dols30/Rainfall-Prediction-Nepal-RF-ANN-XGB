# Rainfall-Prediction-Nepal-RF-ANN-XGB
RainTomorrow prediction for Nepal using Random Forest, XGBoost and ANN.

A machine learning project that predicts whether it will rain tomorrow in Nepal using historical weather observations from the Open-Meteo Historical Weather Archive.

## Project Overview

This project compares three classification models:

- Random Forest
- XGBoost
- Artificial Neural Network

The data is split chronologically, with earlier dates used for training and later dates used for testing.

## Workflow

1. Load historical Nepal weather data
2. Inspect and prepare the data
3. Explore distributions, outliers and correlations
4. Engineer date features
5. Create the `RainTomorrow` target
6. Perform a chronological train/test split
7. Train Random Forest, XGBoost and ANN models
8. Evaluate confusion matrices and ROC curves
9. Compare model performance
10. Examine XGBoost feature importance
11. Make a final prediction using a historical test row

## Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Random Forest | 0.8599 | 0.8061 | 0.8343 | 0.8200 | 0.9295 |
| XGBoost | 0.8603 | 0.8034 | 0.8404 | 0.8214 | 0.9307 |
| ANN | 0.8448 | 0.7490 | 0.8934 | 0.8149 | 0.9272 |

## Conclusion

XGBoost produced the strongest overall performance, achieving an accuracy of 86.03%, an F1 score of 0.8214 and a ROC-AUC of 0.9307.

The ANN achieved the highest recall, detecting more rainy days, but it also produced more false-positive rain predictions.

## Data Source

Historical weather observations were obtained from the [Open-Meteo Historical Weather Archive](https://open-meteo.com/en/docs/historical-weather-api).

## Technologies

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost and TensorFlow/Keras.

## Run the Project

Install the required packages:

```bash
pip install -r requirements.txt
```

Then open:

```text
Nepal_RainTomorrow_Clean_Final.ipynb
```
