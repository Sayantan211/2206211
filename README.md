 **ASSIGNMENT - 1 : SIMPLE LINEAR REGRESSION** 

-----------------------------------------------------------------------------------------------------------------------------------------------------------

**NAME : SAYANTAN CHAUDHURI**

**ROLL NO.: 2206211**

**SECTION : IT01**

-----------------------------------------------------------------------------------------------------------------------------------------------------------
**QUESTION**
- In this assignment, you need to implement a simple linear regression
model using gradient descent algorithm on the following database.
Database

- Independent/Predictor Variable -
xxxxxxxz
- Dependent/Response Variable -
zzzzzzzz

Answer the following questions based on your observations
1. Use linear regression to fit a straight line to the given
database. Set your learning rate to 0.5. What are the cost
function value and learning parameters values after
convergence? Also, mention the convergence criteria you used.

2. The cost function that we are using in this assignment is
different than the one we used in class. Can you think of the
advantage of averaging the cost?

3. Plot cost function v/s iteration graph for the model in
question 1 for first 50 iterations.

4. Plot the given dataset on a graph and also print the straight
line you obtained in question 1 to show how it fits the data.

5. Test your regression model with the learning rates
lr = 0.005, lr = 0.5, lr = 5
For each learning rate, plot a graph showing how the cost
function changes for the first 50 iterations and write your
observation.

6. Choose a suitable learning rate, then implement stochastic and
min-batch gradient descent, plot the cost function against
iteration, and observe how your cost function changes compared
to batch gradient descent.

------------------------------------------------------------------------------------------------------------------------------------------------------------

This repository demonstrates how to implement linear regression using three types of gradient descent methods:
1. **Batch Gradient Descent**
2. **Mini-batch Gradient Descent**
3. **Stochastic Gradient Descent**

The model is applied to a dataset for linear regression, and visualizations of the cost function vs. iterations and the fitted regression line are provided.

## Project Structure

~ `linearX.csv`: Dataset for the independent variable `X` (features).

~ `linearY.csv`: Dataset for the dependent variable `Y` (target).

~ `2206211.py`: Python script implementing linear regression with different gradient descent techniques.

## Process

1. **Data Loading and Preprocessing**:
    - Loaded the datasets (`linearX.csv` and `linearY.csv`) and merged them. 
    - Applied **Min-Max scaling** to normalize the features and target values.

2. **Splitting the Dataset**:
    - Split the data into training and testing sets using `train_test_split` for model training and evaluation.

3. **Implementing Gradient Descent**:
    - **Batch Gradient Descent**: Implemented a basic linear regression model using full dataset updates per iteration.
    - **Mini-batch Gradient Descent**: Modified the GD algorithm to use small batches for parameter updates, improving efficiency.
    - **Stochastic Gradient Descent**: Updated parameters after each data point, offering faster convergence.

4. **Cost Function Visualization**:
    - Plotted cost vs. iterations for each gradient descent method and tested different learning rates (0.005, 0.5, 5) to observe their impact on convergence.

5. **Model Evaluation and Visualization**:
    - Used the test set for predictions and visualized the fitted regression line over the data points to assess the model’s performance.

This process helped compare the effectiveness of different gradient descent techniques for linear regression.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

