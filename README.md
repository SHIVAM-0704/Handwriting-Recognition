# Handwriting-Recognition

Let's start by importing TensorFlow.
Our image has values from zero to 255, but neural networks work better with normalized data. So, let's change it to between zero and one simply by dividing every value by 255. In Python, you can actually divide an entire array with one line of code given in the program

So now we design our model. As explained earlier, there's an input layer in the shape of the data and an output layer in the shape of the classes, and one hidden layer that tries to figure out the roles between them. Now we compile the model to finding the loss function and the optimizer, and the goal of these is as before, to make a guess as to what the relationship is between the input data and the output data, measure how well or how badly it did using the loss function, use the optimizer to generate a new gas and repeat
We can then try to fit the training images to the training labels. We'll just do it for nine epochs to be quick. We spend about 25 seconds training it over five epochs and we end up with a loss of about 0.0197 . That means it's pretty accurate in guessing the relationship between the images and their labels. That's not great, but considering it was done in just 17 seconds with a very basic neural network, it's not bad either
