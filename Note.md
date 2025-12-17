
# M2: Linear Regression with One Variable.
- Model Representation.
## Cost Function.
- We can measure the accuracy of our hypothesis function by using a cost function. This takes an average difference (actually a fancier of an average) of all the results of the pytothesis with inputs from x's and the actual outputs y's.
$$
J(\theta_0,\theta_1) = \frac{1}{2m}\sum_{i=1}^{m}(\hat{y}_i-y_i)^2=\frac{1}{2m}\sum_{i=1}^{m}(h_\theta(x_i)-y_i)^2
$$
To break it parts, it is $\frac{1}{2}\hat{x}$ where $\hat{x}$ is the mean of the squares of $h_\theta(x_i)-y_i$, or the difference between the predicted value and the actual value.

This function is otherwise called the "Squared error function" or "Mean Squared error". This mean is halved $(\frac{1}{2})$ as a convenience for the computation of the gradient descent, as the derivative term of the square will cancel out the $\frac{1}{2}$ term. The folowing image summarizes what the coust function does:

![Cost Function](./images/cost_function.png)

$$
minimize_{\theta_0,\theta_1}[J(\theta_0,\theta_1)]\\
J(\theta_0,\theta_1)=[\frac{1}{2m}\sum_{i=1}^m(h_\theta(x^{(i)})-y^{i})^2]=cost\ function\\
m=number\ of\ training\ examples\\
h_\theta(x^{(i)})=\theta_0+\theta_1x^{(i)}=predicted\ value\ for\ x^{(i)}\\
$$

