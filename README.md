
# California Housing Price Predictor 
This repository is designed to examine California housing data and forecast housing prices through the application of linear regression as a machine learning technique. The implementation leverages the widely-used scikit-learn library to handle linear regression and manage the machine learning components of the analysis.


## DataSet Details

This dataset was obtained from the StatLib repository. https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html

This dataset was derived from the 1990 U.S. census, using one row per census block group. A block group is the smallest geographical unit for which the U.S. Census Bureau publishes sample data (a block group typically has a population of 600 to 3,000 people).


It can be downloaded/loaded using the sklearn.datasets.fetch_california_housing function.
- [California Housing Dataset in Sklearn Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)
- 20640 samples
- 8 Input Features: 
    - MedInc median income in block group
    - HouseAge median house age in block group
    - AveRooms average number of rooms per household
    - AveBedrms average number of bedrooms per household
    - Population block group population
    - AveOccup average number of household members
    - Latitude block group latitude
    - Longitude block group longitude
- Target: Median house value for California districts, expressed in hundreds of thousands of dollars ($100,000




## Language / Libraries 

**Language:** Python

**Packages:** Sklearn, Matplotlib
## Usage

The code is built on Google Colab on an iPython Notebook.


```bash
Download the repository, upload the notebook and dataset on colab, and execute!

```
    
## Lessons Learned

### Linear Regression 
    1. Its statistical method through which we can model the relationship between a dependent variable and one or more independent variables by fitting a linear equation to the observed data. 
    
    2. Linear equation : Y = a + bX
      Y : dependent variable : Housing price in this project : plotted along Y axis
      X : independent variable : any of feature available in the dataset : plotted along X axis
      b : slope of line 
      a : intercept (value of y when x = 0) 

    3. The goal is to find the best-fitting line (or hyperplane in higher dimensions) that minimizes the sum of the squared differences between the observed and predicted values.


### Modal evaluation based on R2square and Mean squared error

    MSE :
        1. The squared term in MSE penalizes large errors more than small errors.
        2. This means that the model is more sensitive to outliers or large deviations 
        from the true values.
        3. By squaring the errors, the MSE gives more weight to larger errors, making it suitable when large errors are considered more critical or when you want the model to pay more attention to extreme values.

    R2 Score :
        1.  It's used to evaluate the goodness of fit of the model to the data.
        2. Also known as coefficient of determination. ranges from 0 to 1
        3. A higher R2 score indicates a better fit of the linear regression model to the test  data. 
        4. It can be interpreted as the proportion of the variance in the dependent variable (y) that is captured by the linear model.


## Observation 

Below are the modal evaluation values observed by implementing linear regression on the dataset.

| Metric        | Value         |
| ------------- | ------------- |
| R2 Score      | 0.60          |
| MSE           | 0.53        |

## Contact

If you have any feedback/are interested in collaborating, please reach out to me at srijandangwal1@gmail.com


## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

