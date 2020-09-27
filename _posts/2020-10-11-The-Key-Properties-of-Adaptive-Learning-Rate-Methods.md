---
layout: post
title: The Key Properties of Adaptive Learning Rate Methods
permalink: /Posts/The-Key-Properties-of-Adaptive-Learning-Rate-Methods/
date: 2020-08-28
---

- Gradient's scale invariance: 

  - In adaptive learning rate methods, sqrt(v_t) plays the role of estimating the scale of the gradient, while m_t plays the role of estimating the gradient. When g_t or m_t is divided by sqrt(v_t), the scale of the gradient is removed and hence achieves scale invariance. 

  - Formally, we have:
  
    - {g_i}\_(i=0)^T is equivalent to {k*g_i}\_(i=0)^T for any k>0.
    - The scale of m_t/sqrt(v_t) is approximately 1.  
      - Because v_t^2 is approximately var(g_t) + E(g_t)^2.    
      - The standard deviation is approximately 1, if E[g_t]=0 and \beta_1=0.  
      - If g_t is constant, then m_t/sqrt(v_t) equals 1.

<!--  -->
  - It benefits the tuning of learning rate, and especially benefits settings where gradients have different scales, e.g., multi-layer deep neural networks where gradients at different layers tend to be dramatically different.

<!--  -->
- Fixed parameter update step size, and its scale is basically just equal to the learning rate:

  - This is the direct consequence of scale removing or scale invariance. 
  - g_t or m_t is divided by its estimated scale sqrt(v_t) and hence is normalized. 
  - So its scale becomes 1, hence the scale of (lr * m_t/sqrt(vt)) is basically equal to the learning rate.

<!--  -->
- Parameter's scale hence is very important in Adam etc. and has an equivalent effect as the learning rate:

  - (1) if the weight is of scale 1 and the lr is 0.001, for each update, the model parameter is changed by 0.1%.
  - (2) if the weight is of scale 10 and the lr is 0.01, for each update, the model parameter is changed by 0.1%.
  - (3) if the weight is of scale 10 and the lr is 0.001, for each update, the model parameter is changed by 0.01%.
  - (4) if the weight is of scale 1 and the lr is 0.0001, for each update, the model parameter is changed by 0.01%.
  - One can empirically verify that: (1) and (2) are equivalent; (3) and (4) are equivalent.

  - To test different weight scales while keep the model's equivalency, one may use the reparameterization trick:  

    - y = w * x     <-->     y = w' / k * x
    - where w' = k * w, i.e., the weights are scaled up by k

<!--  -->
- So give the learning rate while do not tell the parameter scale actually tells nothing.
  
  - Though we can assume a commonly used parameter initialization scheme. But it is not necessarily true. 