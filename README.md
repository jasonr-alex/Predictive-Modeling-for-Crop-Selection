## Predictive Modeling for Crop Selection

<img width="530" height="354" alt="image" src="https://github.com/user-attachments/assets/b7bdb1eb-de96-42cf-a8fc-e6293d443868" />

### Summary: 
Soil condition is instrumental for decision-making when selecting the best crops. The elements of the soil that are critical for crop selection are nitrogen (N), phosphorus (P), potassium (K), and pH. However, assessing these levels can be costly and time-consuming, often leading farmers to prioritize only metrics within their budget. In this project, I execute a logistic regression classification to decide which crop to plant each season and identify the most critical feature for predictive performance. 

### Hypothesis: 
The most important feature for predictive performance would be the pH. 

### How to Run the Project: 
The main project is found in the crop_selection.ipynb file: `crop_selection.ipynb`

### Dataset Source & Details:
The dataset source was extracted from UCI or Kaggle. The data is found in the .csv file extension `soil_measures.csv`

### Model Evaluation:
The logistic classification model predictions were evaluated with the following metrics: **accuracy**, **precision**, **recall**, and **F1**; a confusion matrix was also created for the predictions.

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

### Methodology

#### Preprocessing
For Logistic Regression and classification models in general, it's essential to scale your data so that the model treats all features fairly. Scaling is also crucial as it assists with convergence. 

The training dataset was also checked to see if there was a balanced distribution of the number of crops; imbalance can affect the prediction outcomes for the model.

Analysis for any missing values was done as well; any missing values would also mean a lack of essential data for the model. No missing values were found in the dataset; no imputation was performed.

  - [x] StandardScaler() to scale the data.
  - [x] Balance trained dataset
  - [x] Handled missing values

### Results & Visualizations: 
The logistic regression model, without performing any feature scaling, scored with an accuracy of 61.3%; with scaling, that prediction performance improved to 65.9%. 

Based on the classification report, we can also see the predictive performance. The model could correctly predict the following crops: banana, chickpea, coffee, cotton, maize, mungbean, orange, and papaya. 

To improve the model's performance, incorporating feature engineering can assist the model in understanding more complex relationships based on foundational knowledge for soil health and crop yield.
<br><br>

### Classification Report with all Features
<img width="441" height="614" alt="Screenshot 2025-07-12 at 3 00 00 PM" src="https://github.com/user-attachments/assets/c3d6f6b2-bd44-4576-93dd-7f014d054f6e" />

<br><br>
Analyzing the importance of features, it was found that the single most crucial feature for predictive performance is potassium (K); this rejects the initial hypothesis. 

Furthermore, classification reports have also been included to show how the model performs in classifying based on a single feature. 
<br><br>

<img width="1148" height="907" alt="image" src="https://github.com/user-attachments/assets/361b4d12-00ad-439f-935e-c8476a59af33" />




  




