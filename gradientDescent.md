# Gradient Descent For logistic regression
The hypothesis function $h_{\theta}(x)$ for logistic regression function is written as  
$$h_{\theta}(x) = g(\theta^{T}x) = \frac{1}{1+e^{\theta^Tx}} $$

The cost function for logistic regression function is written as  
$$
   J(\theta) = \frac{1}{m} \sum_{i=1}^{m} 
   [
       -y^{(i)} \log( h_{\theta}(x^{(i)}) ) 
       -(1-y^{(i)}) \log( 1 - h_{\theta}(x^{(i)}) ) 
   ]
$$

The derivatives for this function is written as
$$
   \frac{\partial }{\partial \theta_j} J(\theta)
   = \frac{1}{m} \sum_{i=1}^{m} 
   \Big[
       -y^{(i)} \log( h_{\theta}(x^{(i)}) ) 
       -(1-y^{(i)}) \log( 1 - h_{\theta}(x^{(i)}) ) 
   \Big]
   = \frac{1}{m} \sum_{i=1}^{m} 
   \Big[
      \frac{\partial h_{\theta}(x^{(i)})}{\partial \theta_j}
      (
      - \frac{y^{(i)}}{h_{\theta}(x^{(i)})} + \frac{1-y^{(i)}}{1-h_{\theta}(x^{(j)})}
      )
   \Big] 
$$

