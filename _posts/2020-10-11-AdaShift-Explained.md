---
layout: post
author: Zhiming Zhou
date: 2020-08-29
title: AdaShift Explained
permalink: /Posts/AdaShift-Explained/
---

- Adam is proved to have a convergence issue, and counterexamples can be constructed. In the paper of AdaShift, we show that the non-convergence comes from the positive correlation of the current adaptive term v_t and the current gradient g_t, because the update rule is v_t = \beta2 v_(t-1) + (1-\beta2) g_t, i.e., the correlation factor is 1-\beta2. Such a positive correlation would lead to bias net update factor. 

- The net update factor of g_t can be understood as its accumulated step-size in the entire optimization, because its influence can be delayed to future updates, due to first moment estimation or otherwise named the moving average windows. The influence of g_t decreases at a rate of \beta1 each step and is initialized with a ratio 1-\beta1, which sums to one. (This is similar to Momentum and SGD, where the net update factor of each gradient is also one.)

- However, for adaptive learning rate methods (Adam as a representative), the net update factor of each gradient does not have a fixed value (hence, not the same) nor follow a fixed distribution (which we believe have a similar effect as fixed value choices, Momentum and SGD). 

- And obviously, if v_t is independent of g_t and follows a fixed distribution, then, the net update factor of g_t, i.e., its accumulated step-size, follows a fixed distribution (which then leads to a convergence guarantee that similar to Momentum and SGD). This is the central thought of the AdaShift solution. 

- To achieve "follow a fixed distribution", we propose to temporally shift the gradient for the calculation of v_t. In such a condition, if "moving average windows" is disabled (i.e., \beta1=0), and if g_t follows a fixed distribution, then v_t also follows a fixed distribution. However, "if moving average windows is disabled" turns out to be the limitation of AdaShfit. Nevertheless, we propose to shift the gradient for multiple steps, then, the "leave-out" gradients that still not get involved to v_t can be moving averaged or simply averaged if you like. A new version of AdaShift is coming and we will fix this issue. Looking forward to the new *free-lunch solution* to the non-convergence issue of Adam! 

- Given the previous anatomy of adaptive learning rate methods, the key of its convergence is to force v_t to be independent of g_t and to follow a fixed distribution. In this sense, the role of v_t is to *estimate the scale of the gradient* (because we know that the key benefit of adaptive learning rate method is scale invariance, which means, the scale of the gradient is removed, making it easy to use, especially in multi-layer neural networks, where the gradient' scales can change dramatically in different layers. given the gradient's scale invariance, it is much easier to turn a good learning rate). 

- Because v_t is to somehow estimate the scale of the gradient, it can also estimate the overall gradient scale, or layer-wise / block-wise gradient scale. In doing this, it reduces to adaptive learning rate SGD (with each block sharing the same v_t, the overall gradient scale in each block is removed, but the relative gradient scale is kept in the block), which makes it extremely suitable for optimizing a multi-layer neural network. 

- The update rule of v_t can even be generalized. Try and find more interesting update rules, as long as it estimates the scale of the gradient!