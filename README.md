Linear Regression in pure python

Linear regression is the problem that paved the path for us into the vast, beautiful and beneficial world of deep learning. Linear regression follows the basic
idea of neural networks.
Optimization is the underlying function of all neural networks and to understand that linear regression is a good starting point.

Think of linear regression as a function that can find the relation between inputs and outputs.  example: (inputs:area of house,distance from city,height,rating 
output: price)
In linear Regression the relation is defined by a linear polynomial whose output is the output of the model and the inputs of the polynomial is the actual input
of the linear regression model.  The variables of this linear polynomial are called weights which determine the relation between the inputs and outputs

So in the training process we are going to update the weights(variables) such that the output of the linear regression function(polynomial) is as close to the 
actual output we have given the model.

If we go into the linear regression python file, the main part of the code is the function of "model". 
You can see the inputs of the function is X,Y,Learning rate and interation.
X is the set of inputs and the Y is the set of outputs for the corresponding inputs. The learning rate defines the pace of learning that is how fast the 
learning should happen. If the learning rate is low, then the weight updation would be slow and if it is very high then, the model might change too much thus 
leading to inaccuracy.
Iteration states the number of times we should updates the weights. Normally, the higher the iteration the higher the accuracy but slower the model.

Here, theta is the weight, as we have only one input at every row of X in this case, theta is only a single number.
y-pred is the prediction of the model which is dependent on the input value X and the weight value theta.

The for loop represents the training process. cost is the function that calculates the difference between y-pred and the actual output y. 
After that we are going to calculate the derivative of theta with respect to the cost function we have calculated.
And then we are going to update the theta by subtracting the value of the product of learning rate and slope(derivative) we have calculated. 
And again, you can see the function of the learning rate as it controls the rate of change. 

And then after performing the above steps for some iterations, we will finally output the value of theta.

So, we have successfully found the relation between the two sets of numbers X and Y and now we could use this theta to do some predictions.


And in the next section we have performed the same process for two dimensional set of X that is it had two numbers for each row and one output. 
For that we have also made the shape of theta to be two dimensional.
