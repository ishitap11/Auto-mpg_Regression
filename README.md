# Auto-mpg_Regression
The repository shows regression models for auto-mpg dataset from UCI Machine Learning Repository

The project is a simple guide to understanding how to build a regression model for data. It also depicts the working of learning curves and how they help in understanding issues of underfitting and overfitting.

## Tasks Accomplished
The project helps in understanding the following two tasks
  1. Building a Regression Model
     The following regression algorithms were used for the project
      a. Polynomial Regression
      b. Decision Tree
      c. Random Forest
  2. Plotting Learning Curve for the model performance.

## Understanding the Dataset
The following plot shows the relationship between the dependant variable x (auto mpg values) with the features of training data instances.
  
  ![Training data](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/trainingdata.PNG)

It is clear that a polynomial model would fit well for the above data.

The following plot shows the training data as a 2-D representation using two features: diplacement(displ) on x-axis and hp on y-axis.
  
  ![Training data](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/trainingdata2d.PNG)
  
## Models Results and consequent Learning Curves

### Polynomial Regression
The plot shows the mapping between true values v/s the predicted values for the testing data.

  ![LR-result](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/lrresult.PNG)

The plot below shows the learning curve for the Polynomial Regression model.

  ![LR-curve](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/lclr.PNG)
  
It is clear from the plot and learning curve above that the regression model built using Polynomial regression is a good fit for the data. The close learning curves for the training and testing data with a fairly low error values suggest the same.

### Decision Tree
The plot shows the mapping between true values v/s the predicted values for the testing data.

  ![DT-result](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/drresult.PNG)

The plot below shows the learning curve for the Decision Tree regression model.

  ![DT-curve](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/lcdr.PNG)

It is clear form the plot and learning curve above that the regression model is underfitted. The errors on both the training and testing set are more quite close and the model does not generalize well for either of the datasets

### Random Forest
The plot shows the mapping between true values v/s the predicted values for the testing data.

  ![RF-result](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/rfresult.PNG)
  
The plot below shows the learning curve for the Random Forest regression model.

  ![RF-curve](https://github.com/ishitap11/Auto-mpg_Regression/blob/master/images/lcrf.PNG)
 
The learning curve and result plot depict that the Random Forest regression tends to overfit the data. The fluctuation in the learning curve shows how poorly the model performs for unseen testing data.

## The Root Mean Squared Error (RMSE) scores

| Model Name            | RMSE Score    |
| -------------         | ------------- |
| Polynomial Regression | 3.89722       |
| Decision Treee        | 4.22591       |
| Random Forest         | 4.44458       |

The error values above confirms with the iniferences made using the Learning Curve. The Polynomial Regression model performs most effectively. 


