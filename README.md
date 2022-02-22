# Neural_Network_Charity_Analysis

## Overview of the analysis
An analysis project that used neural network modelling to predict whether applicants would be successful if funded by the organization, Alphabet Soup Co.

![image](https://user-images.githubusercontent.com/81877387/155226010-90c92216-e76b-4c35-80de-75af109eea23.png)## Resources

Software: Python 3.8.5 (mlenv environment), Jupyter Notebook 6.1.4, TensorFlow 2.0

## Results 
## Data Preprocessing:
* The IS_SUCCESSFUL column is the target for my model
* The IS_SUCCESSFUL, EIN, NAMES columns were dropped from the data set. All other columns were features for my model

## Compiling, Training, and Evaluating the Model:
* Due to the large amount of data points, I selected 2 hidden layers in the model - the first layer having 120 neurons, second layer with 50 neurons and both using the ReLU function. The third outer layer used a sigmoid function. The Relu function was selected as it is considered best for nonlinear datasets and the Sigmoid activation function is considered best for binary classications. By having 2 hidden layers and a larger amount of neurons the aim was to try and catch more variability within the data. 
* The results of the model showed 70% accuracy, so it did not achieve the target performance of 75%. 

<img width="618" alt="Screen Shot 2021-09-04 at 4 04 50 PM" src="https://user-images.githubusercontent.com/81877387/132106735-4de311e5-35a1-460d-9a48-4ae358c98862.png">

## Optimization steps to increase model performance:
To try and increase the model's performance, the below 3 attempts were taken:
* 1st attempt: Adding a 3rd hidden layer with 30 neurons. Accuracy of this model = 53%

<img width="642" alt="1st op attempt" src="https://user-images.githubusercontent.com/81877387/132106771-844c7922-e993-4c15-baee-0f2678ad062e.png">

* 2nd attempt: Kept the 3rd hidden layer and increased epochs to 300. Accuracy of this model = 49%

<img width="638" alt="2nd attempt" src="https://user-images.githubusercontent.com/81877387/132106789-e927155a-b967-4c00-b193-d76c6c471c79.png">

* 3rd attempt: Kept original model layers but changed 2nd hidden layer activation function to sigmoid. Accuracy of this model = 53%.

<img width="626" alt="3rd attempt" src="https://user-images.githubusercontent.com/81877387/132106839-4ee2cafa-ce3c-4566-8e9b-bf762656aa36.png">


## Summary 
In summary, the original model had the best accuracy of all the attempts. However, this failed to reach the target of 75% accuracy. In reviewing the models, another thing to consider in future is to remove more columns in the data and this would therefore reduce the features in the model. Large numbers of input features can cause poor performance, so by carrying out dimensionality reduction, this could generate a better model for this data. 
