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
