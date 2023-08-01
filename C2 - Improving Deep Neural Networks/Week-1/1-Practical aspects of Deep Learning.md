## Week 1 Quiz - Practical aspects of Deep Learning

1. If you have 20,000,000 examples, how would you split the train/dev/test set? Choose the best option.

    - 99% train, 0.5% dev, 0.5% test

2. In a personal experiment, an M.L. student decides to not use a test set, only train-dev sets. In this case which of the following is true?

    - He might be overfitting to the dev set

    Note: Information for the bias and variance can be obtained from the training error and the dev error.

3. If your Neural Network model seems to have high bias, what of the following would be promising things to try? (Check all that apply.)

    - [X] Make the neural network deeper
    - [x] Increase the number of units in each hidden layer
    - [ ] Add regularization
    - [ ] Get more training data

4. Working on a model to classify bananas and oranges your classifier gets a training set error of 0.1% and a dev set error of 11%. Which of the following two are true?

    - [ ] The model has a very high bias
    - [ ] The model is overfitting the train set
    - [X] The model has a very high variance
    - [ ] The model is overfitting the dev set

5. What is weight decay?

    - A regularization technique (such as L2 regularization) that results in gradient descent shrinking the weights on every iteration.

6. What happens when you increase the regularization hyperparameter lambda?

    - Weights are pushed toward becoming smaller (closer to 0)

7. Which of the following are true about dropout?

    - [x] It helps to reduce the variance of a model
    - [ ] It helps to reduce the bias of a model
    - [ ] In practice, it eliminates units of each layer with a probability of keep_prob
    - [x] In practice, it eliminates units of each layer with a probability of 1-keep_prob
    - [x] It helps to reduce overfitting


8. Decreasing the parameter keep_prob from (say) 0.6 to 0.4 will likely cause the following:

    - Increasing the regularization effect

9. Which of the following actions increase the regularization of a model? (Check all that apply)

    - [X] Normalizing the data
    - [ ] Decrease the value of the hyperparameter lambda
    - [X] Make use of data augmentation
    - [ ] Increase the value of keep_prob in dropout
    - [X] Decrease the value of keep_prob in dropout
    - [X] Increase the value of hyperparameter lambda

10. Suppose that a model uses, as one feature, the total number of kilometers walked by a person during a year, and another feature is the height of the person in meters. What is the most likely effect of normalization of the input data?

    - It will make the training faster

11. You are working on an automated check-out kiosk for a supermarket and are building a classifier for apples, bananas, and oranges. Suppose your classifier obtains a training set error of 19% and a dev set error of 21%. Which of the following are promising things to try to improve your classifier? (Check all that apply, suppose the human error is approximately 0%)

    - Use a bigger network

    Note:  First, the high bias problem must be addressed.

12. To reduce high variance, the regularization hyperparameter lambda must be increased. True/False?

    - [x] True
    - [ ] False

13. Increasing the parameter keep_prob from (say) 0.5 to 0.6 will likely cause the following: (Check the two that apply)

    - [ ] Increasing the regularization effect
    - [X] Reducing the regularization effect
    - [ ] Causing the neural network to end up with a higher training set error
    - [X] Causing the neural network to end up with a lower training set error

14. When designing a neural network to detect if a house cat is present in the picture, 500,000 pictures of cats were taken by their owners. These are used to make the training, dev and test sets. It is decided that to increase the size of the test set, 10,000 new images of cats taken from security cameras are going to be used in the test set. Which of the following is true?

    - This will be harmful to the project since now dev and test sets have different distributions

    Note: This won't have a real effect on the bias of the model but will hinder the way we are measuring the performance.

