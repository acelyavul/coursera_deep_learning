## Week 3 Quiz - Hyperparameter tuning, Batch Normalization, Programming Frameworks

1. If searching among a large number of hyperparameters, you should try values in a grid rather than random values, so that you can carry out the search more systematically and not rely on chance. True or False?

   - [ ] True
   - [x] False

<br>

2. If it is only possible to tune two parameters from the following due to limited computational resources. Which two would you choose?

   - [x] $\alpha$
   - [x] The $\beta$ parameter of the momentum in gradient descent
   - [ ] $\epsilon$ in Adam
   - [ ] $\beta _1$, $\beta _2$ in Adam

<br>

3. Even if enough computational power is available for hyperparameter tuning, it is always better to babysit one model ("Panda" strategy), since this will result in a more custom model. True/False?

   - [ ] True
   - [x] False

<br>

4. Knowing that the hyperparameter α should be in the range of 0.001 and 1.0. Which of the following is the recommended way to sample a value for α?

      $r=-3*np.random.rand() \newline alpha=10**r$

<br>

5. Once good values of hyperparameters have been found, those values should be changed if new data is added or a change in computational power occurs. True/False?

   - [x] True
   - [ ] False

<br>
   <em>The choice of some hyperparameters such as the batch size, depends on conditions such as hardware and quantity of data.</em>

<br>

6. When using batch normalization it is OK to drop the parameter $ b^{[l]}$ from the forward propagation since it will be subtracted out when we compute $\tilde{z}^{[l]}=\gamma z^{[l]}_{normalize} + \beta ^{[l]}$. True/False?

   - [x] True
   - [ ] False

<br>

7. In the normalization formula $z^{(i)}_{norm}=\frac {z^{(i)}-\mu} {\sqrt{\sigma ^2 + \epsilon}}$, why do we use epsilon?

      - To avoid division by zero

<br>

8. Question 9 A neural network is trained with Batch Norm. At test time, to evaluate the neural network we turn off the Batch Norm to avoid random predictions from the network. True/False?

   - [ ] True
   - [x] False

<br>

9. Which of the following are some recommended criteria to choose a deep learning framework?

    - Running speed

<br>

10. With a relatively small set of hyperparameters, it is OK to use a grid search. True/False?

   - [x] True
   - [ ] False

<br>

10. Every hyperparameter, if set poorly, can have a huge negative impact on training, and so all hyperparameters are about equally important to tune well. True or False?

   - [ ] True
   - [x] False

<br>

11. Using the "Panda" strategy, it is possible to create several models. True/False?

   - [x] True
   - [ ] False

<br>

12. Finding new values for the hyperparameters, once we have found good ones for a model, should only be done if new hardware or computational power is acquired. True/False?

   - [ ] True
   - [x] False

   *As the data changes for the model, it might be beneficial to tune some of the hyperparameters again.*

<br>

13. Which of the following are true about batch normalization?

    - One intuition behind why batch normalization works is that it helps reduce the internal covariance.

<br>

14. Which of these statements about deep learning programming frameworks are true? (Check all that apply)

   - [x] A programming framework allows you to code up deep learning algorithms with typically fewer lines of code than a lower-level language such as Python.
   - [x] Even if a project is currently open source, good governance of the project helps ensure that the it remains open even in the long term, rather than become closed or modified to benefit only one company.
   - [ ] Deep learning programming frameworks require cloud-based machines to run.

<br>

15. Knowing that the hyperparameter α should be in the range of 0.00001 and 1.0. Which of the following is the recommended way to sample a value for α?

      $r=-5*np.random.rand() \newline alpha=10**r$

<br>

16. After training a neural network with Batch Norm, at test time, to evaluate the neural network on a new example you should:

      - Perform the needed normalizations, use μ and $σ^2$ estimated using an exponentially weighted average across mini-batches seen during training.

<br>

17. Which of the following statements about $\gamma$ and β in Batch Norm are true?

   - [ ] The optimal values are $\gamma = \sqrt {\sigma ^2 + \epsilon}$, and $\beta = \mu$
   - [x] They set the variance and mean of the linear variable $z^{[l]}$ of a given layer.
   - [x] They can be learned using Adam, Gradient descent with momentum, or RMSprop, not just with gradient descent.
   - [ ] There is one global value of $\gamma ∈ \mathbb{R}$ and one global value of $\beta ∈ \mathbb{R}$ for each layer, and these apply to all the hidden units in that layer
   - [ ] $\beta$ and $\gamma$ are hyperparameters of the algorithm, which we tune via random sampling
