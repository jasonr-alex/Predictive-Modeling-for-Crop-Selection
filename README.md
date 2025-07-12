# Predictive Modeling for Crop Selection

<img width="530" height="354" alt="image" src="https://github.com/user-attachments/assets/b7bdb1eb-de96-42cf-a8fc-e6293d443868" />

### Summary: 
Soil condition is instrumental for decision-making when selecting the best crops. The elements of the soil that are critical for crop selection are nitrogen (N), phosphorus (P), potassium (K), and pH. However, assessing these levels can be costly and time-consuming, often leading farmers to prioritize only metrics within their budget. In this project, I execute a logistic regression classification to decide which crop to plant each season and identify the most critical feature for predictive performance. 

### How to Run the Project: 
The main project is found in the crop_selection.ipynb file: `crop_selection.ipynb`

### Dataset Source:
The dataset source was extracted from UCI or Kaggle. The data is found in the .csv file extension `soil_measures.csv`

### Model Evaluation:
The logistic classification model predictions were evaluated with the following metrics: accuracy, precision, recall, and F1; a confusion matrix was also created for the predictions.

### Dependencies:
All necessary libraries are included within the Jupyter Notebook.

Here is the list of the necessary packages:

```
import pandas as pd
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import train_test_split
from sklearn import metrics
from sklearn.metrics import confusion_matrix, classification_report
import matplotlib.pyplot as plt
from sklearn.preprocessing import StandardScaler
``` 


