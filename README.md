# Diabetes-Prediction-using-Machine-Learning-
This Project is on Diabetes Predictio with Machine Learning by using PyCharm IDE and Django 

Diabetes, increasingly prevalent even among younger populations, demands a deep understanding of how it 
manifests. To comprehend its development, one must first grasp the body's normal functioning. Glucose, sourced 
primarily from carbohydrates like bread, pasta, and fruits, fuels our system after digestion. This glucose circulates 
in the bloodstream, powering both brain and body cells. Any surplus gets stored in the liver for future energy needs. 
Insulin, a hormone from the pancreas, acts as a facilitator, allowing glucose into cells for energy production. 
However, if the pancreas fails to produce enough insulin (insulin deficiency) or if cells become resistant to its 
effects, glucose accumulates in the blood, leading to diabetes. 
There are distinct types of diabetes: 
Type 1 diabetes emerges from an immune system malfunction, resulting in insufficient insulin production by 
pancreatic cells. Despite ongoing research, its exact triggers and preventive measures remain elusive. 
Type 2 diabetes occurs when cells produce inadequate insulin or when the body can't use insulin effectively. This 
form is the most common, affecting around 90% of those with diabetes, and is influenced by genetic predisposition 
and lifestyle choices. 

3.1.1 Data Description: 
Fig 1: Proposed system work 
The dataset on diabetes originated from the Kaggle website and comprises more than 2400 cases. Its purpose is to 
utilize various measures to predict whether a patient is diabetic or not. The dataset for "Diabetes Prediction" 
comprises eight distinct features, namely: (i) Pregnancies, (ii) Glucose, (iii) Blood Pressure, (iv) Skin Thickness, 
(v) Insulin, (vi) BMI (Body Mass Index), (vii) Diabetes Pedigree Function, and (viii) Age 
Our aim is to predict the "Outcome" feature, where 0 indicates the absence of diabetes and 1 indicates the presence 
of diabetes. 
3.1.2  Data Preprocessing:  
Data preprocessing is a crucial step, particularly in healthcare-related datasets, where missing values and other 
impurities can undermine data effectiveness. Enhancing the quality and efficacy of the dataset post-mining is vital, 
and data preprocessing serves this purpose. It's essential for employing machine learning techniques effectively, 
ensuring accurate results and successful predictions. One fundamental aspect of preprocessing involves handling 
missing values, such as removing instances where values are zero, as they are implausible in healthcare contexts. 
By eliminating irrelevant features or instances, we create a feature subset, known as feature subset selection, which 
reduces data dimensionality and enhances computational efficiency. 
<class 'pandas.core.frame.DataFrame'> 
RangeIndex: 2460 entries, 0 to 2459 
Data columns (total 9 columns): 
#   Column                    
Non-Null Count  Dtype   ---  ------                    
0   Pregnancies               
1   Glucose                   
2   BloodPressure             
3   SkinThickness             
4   Insulin                   
5   BMI                       --------------  -----   
2460 non-null   int64   
2460 non-null   int64   
2460 non-null   int64   
2460 non-null   int64   
2460 non-null   int64   
2460 non-null   float64 
6   DiabetesPedigreeFunction  2460 non-null   float64 
7   Age                       
2460 non-null   int64   
8   Outcome                   
2460 non-null   int64  

3.1.3  Train And Test Split: 
Following data cleaning, the next step involves normalizing the data before training and testing the model. During 
this process, the dataset is divided into training and testing sets, with the training set utilized to train the algorithm 
while keeping the test set separate for evaluation. Through training, the algorithm develops a model based on the 
2247 
J. Electrical Systems 20-7s (2024): 2244-2257 
logic, algorithms, and feature values present in the training data. Essentially, normalization aims to standardize all 
attributes to a consistent scale, ensuring uniformity across the dataset. 
3.1.4  Fitting The Model: 
Adjusting the parameters of the model to enhance accuracy is known as model fitting. To create a machine learning 
model, an algorithm is applied to data where the target variable is known. The accuracy of the model is evaluated 
by comparing its predictions with the actual values of the target variable. Model fitting refers to the model's capacity 
to generalize data similar to what it was trained on. A well-fitted model accurately predicts outputs when provided 
with unknown inputs.  
3.1.5  Predicting The Model: 
In the context of forecasting a particular outcome, "prediction" signifies the result produced by an algorithm post
training on historical data and application to new data. Utilizing the predict () method to forecast the model involves 
inputting a test feature dataset and receiving an array of predicted values along with a Classification Report as 
output. 
3.1.6  Evaluation:  
This is the final step of prediction model. Here, we evaluate the prediction results using various evaluation metrics 
like classification accuracy, confusion matrix and f1-score. Classification Accuracy- It is the ratio of number of 
correct predictions to the total number of input samples. It is given as. 
Here's a step-by-step guide on how to calculate accuracy. 

• Make Predictions: Use your trained machine learning model to make predictions on a dataset that was 
not used during training (e.g., a test set or validation set). Each prediction will be compared to the actual known 
values. 
• Count Correct Predictions: Count the number of predictions made by the model that match the actual 
values in the dataset. 
• Total Number of Predictions: Determine the total number of predictions made by the model. 
• Calculate Accuracy: Use the formula mentioned above to calculate the accuracy of the model. This will 
give you a percentage that represents the proportion of correct predictions out of all predictions made by the model. 
Here's a more detailed breakdown: 
Accuracy =   Number of Correct Predictions /  
Total number of predictions Made
