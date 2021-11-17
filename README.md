# Lab Machine Learning Iris Classification


## Create a model that can classify the different species of the Iris flower

![image](https://user-images.githubusercontent.com/88676121/141144626-55913b7c-1969-4efa-9c79-42751258e928.png)

## Table of contents
- [Project Brief](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions#project-brief)
- [Data](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions#data)
- [Process & Tools](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions#process--tools)
- [Visualization](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions#visualization) 
- [Key Take Aways](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions#visualization)

## Project Brief
**Scenario**: Iris is a genus species of flowering plants. Within the Iris species we can find other different types such as the iris setosa, iris versicolor or the iris virginica.

**Challenge**: We will use the given data set to create the model that can classify the different species of the Iris flower.


## Data

Leveraging on the [data](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions/blob/main/iris_dirty.csv) we were provided with, we used Python to explore the relationships between features.

The data set consists of:

- 150 samples

- 3 labels: species of Iris (Iris setosa, Iris virginica and Iris versicolor)

- 4 features: Sepal length,Sepal width,Petal length,Petal Width in cm

![image](https://user-images.githubusercontent.com/88676121/141148918-4f13829b-3460-43c3-a806-34a4410974d6.png)

For further details on all features, please refer to the [notebook](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions/blob/main/Lab_Iris_Predictions.ipynb)

## Process & Tools

**Process**

Our process included the following steps:

Dataset preparation

EDA: assessment of dataframe to prepare for cleaning

Data cleaning & wrangling in Python: 
    
- Identified 1 null value in 'sepal width' and filled it in with the mean of the 'sepal width' values, standarize units converting 'petal width' to cm to be      aligned with the other physical attributes measured and convert to float. 
    
- Locating outliers and dealing with them. We determined that the main outlier had an error as it was showing an unrealistic value for 'sepal lenght'
    
   _**Before**_
    
<img width="611" alt="Screenshot 2021-11-10 at 17 26 42" src="https://user-images.githubusercontent.com/88676121/141152518-cf1a9677-322c-4802-be58-21fe95bd41d7.png">

   _**After**_
    
<img width="607" alt="Screenshot 2021-11-10 at 17 26 50" src="https://user-images.githubusercontent.com/88676121/141152580-fbfdd1f2-86dd-4216-907f-21b100554fa7.png">


- Finding typos on the categorical values and correcting them

_**Before**_

<img width="569" alt="Screenshot 2021-11-10 at 17 32 23" src="https://user-images.githubusercontent.com/88676121/141153666-035c27ad-3398-49ae-bf14-5d883691234d.png">


 _**After**_
 
 <img width="378" alt="Screenshot 2021-11-10 at 17 32 30" src="https://user-images.githubusercontent.com/88676121/141153778-45083f75-5a5e-4752-9916-9eaecee2635a.png">
    
    
Machine Learning Model: using scikit learn and logistic regression

**Tools**

Database: [CSV file](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions/blob/main/iris_dirty.csv)

Vizualizations: seaborn / matplotlib

Code: [Jupyter Notebook](https://github.com/PolFerrandis/Lab-Readme-Iris-Predictions/blob/main/Lab_Iris_Predictions.ipynb) 


## Visualization


_**Data visualization**_

<img width="675" alt="Screenshot 2021-11-10 at 17 11 45" src="https://user-images.githubusercontent.com/88676121/141150156-19f70c4b-a24e-412d-9d09-f68ce297a14c.png">


**_Correlations found_**

<img width="576" alt="Screenshot 2021-11-10 at 17 11 20" src="https://user-images.githubusercontent.com/88676121/141150124-90994a58-0437-4374-bb02-9d548fefb5a0.png">



## Key Take Aways

Our model can classify the different species with an accuracy of more than a 93%.
