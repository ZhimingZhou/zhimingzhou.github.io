## Biography

Zhiming obtained his Ph.D. in Computer Science from [Shanghai Jiao Tong University](http://en.sjtu.edu.cn/) in 2020. He received his B.S. degree in Computer Science from the [ACM Class](https://acm.sjtu.edu.cn/home) at Shanghai Jiao Tong University in 2014.

Zhiming’s research is mainly focused on generative adversarial networks (GANs). Leading a group in the [Apex Lab](http://apex.sjtu.edu.cn/members) at Shanghai Jiao Tong University, he also works on first-order optimization, optimal transport, and other related problems. Prior to that, Zhiming worked on computer graphics in the early years of his Ph.D. (2014-2016), focused on surface reflectance acquisition.

Zhiming has a broad interest in machine learning and deep learning, and he prefers fundamental and theoretical research. Currently, he holds a special interest in the optimization and generalization of deep neural networks and GANs.

## Documents & Links

- [CV](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/Zhiming_Zhou_Resume.pdf) 
  
- [DBLP](https://dblp.org/pers/hd/z/Zhou:Zhiming)
  
- [Google Scholar](https://scholar.google.com/citations?user=b8YJ1EMAAAAJ&hl=en)
  
- [Github](https://github.com/ZhimingZhou)
  
- [Thesis](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/Thesis.pdf) (Chinese) [PPT](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/Defense%20PPT.pptx) (Chinese)
  
- [On the convergence of GANs](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/On%20the%20Convergence%20of%20GANs.pptx)
  - Training instability (LGANs)
  - Unreachable optimum (MaxGP, AdaShift, Ongoing)
  - Generalization issue (Ongoning)
  
- [On the Key Problems of GANs](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/On%20the%20Key%20Problems%20of%20GANs.pptx)
  - Training issues
    - Instability (LGANs)
    - Unreachable Optimum (MaxGP, AdaShift, Ongoing)
  - Sample Quality issues
    - Complex dataset (AM-GAN)
    - Lantent Space (TODO)
  - Generalization issue (Ongoing)
  
- [我的第一份工作以及各种意想不到的收获](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/%E6%88%91%E7%9A%84%E7%AC%AC%E4%B8%80%E4%BB%BD%E5%B7%A5%E4%BD%9C%E4%BB%A5%E5%8F%8A%E5%90%84%E7%A7%8D%E6%84%8F%E6%83%B3%E4%B8%8D%E5%88%B0%E7%9A%84%E6%94%B6%E8%8E%B7.zip)

## Selected Publications 

Lipschitz Generative Adversarial Nets. (LGANs + MaxGP)
- **Zhiming Zhou**, Jiadong Liang, [Y. Song](https://yuxuansong.github.io/files/yuxuan_20Mar.pdf), [L. Yu](http://lantaoyu.com/), [H. Wang](https://cs.stanford.edu/~hongweiw/), [Weinan Zhang](http://wnzhang.net/), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu), [Zhihua Zhang](http://www.math.pku.edu.cn/teachers/zhzhang/).
- The Thirty-sixth International Conference on Machine Learning (ICML, 2019).
- \[[arXiv](https://arxiv.org/abs/1902.05687)\] 
  \[[Slide](https://icml.cc/media/Slides/icml/2019/halla(11-14-00)-11-15-10-4628-lipschitz_gener.pdf)\] 
  \[[Poster](https://s3.amazonaws.com/postersession.ai/ee90cc20-a261-4aee-b28f-899891a90be3.pdf)\]
  \[[Code](https://github.com/ZhimingZhou/AdaShift-Lipschitz-GANs-MaxGP)\]
- <details><summary>Click to expand a brief introduction.</summary>We study the cause of training instability of GANs from the perspective of optimal discriminative function and demonstrate its superiority against the divergence perspective. Under a generalized formulation of GANs, we show that: (1) GANs with unrestricted discriminative function space generally does not guarantee its convergence, suffing from a *gradient uninformativeness issue*; (2) Lipschitz regularization on the discriminative function can generally resolve this issue and guarantee the convergence of GANs, leading to a new family of GANs named Lipschitz GANs. All tested instances of this family consistently outperform WGAN in experiments.</details>

AdaShift: Decorrelation and Convergence of Adaptive Learning Rate Methods. (AdaShift)
- **Zhiming Zhou**\*, Qingru Zhang\*, Guansong Lu, [Hongwei Wang](https://cs.stanford.edu/~hongweiw/), [Weinan Zhang](http://wnzhang.net/), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu).
- The Seventh International Conference on Learning Representations (ICLR, 2019).
- \[[arXiv](https://arxiv.org/abs/1810.00143)\] 
  \[[OpenReview](https://openreview.net/forum?id=HkgTkhRcKQ)\]
  \[[Poster](https://s3.amazonaws.com/postersession.ai/bd0f7f0b-ecaa-4164-aeb6-d0cf181cc27b.jpg)\]
  \[[Code](https://github.com/ZhimingZhou/AdaShift-Lipschitz-GANs-MaxGP)\]
- <details><summary>Click to expand a brief introduction.</summary>We study the convergence issue of Adam optimizer. With the proposed concept *net update factor*, we showed that the key issue in Adam lies in its biased adaptive learning rate caused by the correlation between the adaptive term v_t and the current gradient g_t, and a temporal shift operation is proposed to solve such an issue. Our new understanding of the role of v_t also free v_t from its traditional update rule, leading to more interesting variants. Particularly, with dimension reduction operation in v_t, we achieve the so-called adaptive learning rate SGD, which removes the global gradient scale but keeps the relative scales.</details>

Activation Maximization Generative Adversarial Nets. (AM-GAN)
- **Zhiming Zhou**, [Han Cai](https://han-cai.github.io/files/cv.pdf), Shu Rong, [Yuxuan Song](https://yuxuansong.github.io/files/yuxuan_20Mar.pdf), [Kan Ren](http://www.saying.ren/), [Weinan Zhang](http://wnzhang.net/), [Jun Wang](http://www0.cs.ucl.ac.uk/staff/Jun.Wang/), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu).
- The Sixth International Conference on Learning Representations (ICLR, 2018).
- \[[arXiv](https://arxiv.org/abs/1703.02000)\]
  \[[OpenReview](https://openreview.net/forum?id=HyyP33gAZ&noteId=HyyP33gAZ)\]
  \[[Code](https://github.com/ZhimingZhou/AM-GAN)\]
- <details><summary>Click to expand a brief introduction.</summary>We study how class labels interact with GANs training when introduced and how it improves the sample quality of GANs. Based on the analysis, an improved method for leveraging class labels in GANs had been proposed. An interesting relationship among popular variants of GANs that leverage class labels, including the proposed AM-GAN, are unraveled.</details>

Sparse-as-Possible SVBRDF Acquisition. (SparseSVBRDF)
- **Zhiming Zhou**, Guojun Chen, [Yue Dong](http://yuedong.shading.me/), [David Wipf](\href{http://www.davidwipf.com/home.html), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu), [John Snyder](https://www.microsoft.com/en-us/research/people/johnsny/), [Xin Tong](http://www.xtong.info/).
- ACM Transactions on Graphics (TOG) - Proceedings of ACM SIGGRAPH Asia, 2016. 
- \[[PDF](http://yuedong.shading.me/project/sparsesvbrdf/sparsesvbrdf.pdf)\] 
  \[[ACM](https://dl.acm.org/doi/10.1145/2980179.2980247)\]
  \[[Slide](https://drive.google.com/file/d/16gUKZoQH4HiQ61gEQ-YFs6v9WTEOSixf/view?usp=sharing)\]
- <details><summary>Click to expand a brief introduction.</summary>We significantly reduce the number of images required for spatially-varying surface reflectance (SVBRDF) acquisition, by solving an exact low-rank representation and chasing an extreme sparsity. The number of images required droped from thousands to tens, and high-quality SVBRDF acquisition from a single image becomes possible for the first time.</details>

## Photos

![Me](https://github.com/ZhimingZhou/zhimingzhou.github.io/blob/master/1.png)

## MISC

About GANs:

- GANs is just a tool that maps one distribution to another. GANs can be useful, when and only when, it can be properly used. 

- Given the convergence issue (cannot generalize when trained to optimum, memorizing the training distribution), the two typical theoretically sound usages that I know are optimal transport (where the target distribution does not need generalization) and data modeling (where the data can be just the data to be modeled and somehow does not need generalization). 

- Other typical usages include: image (or any other data) synthesis, forcing the output distribution to a given distribution (like GANs for super-resolution and transferring). GANs can also be used for conditional diverse outputs, which is just like image synthesis, but it is conditional, and the diversity comes from the freedom of the non-conditionaled parts. 

- The most well-know problem about GANs is its training instability issue. According to *WGAN and its foregoing crop*, the non-convergence of GANs (training instability is somehow equivalent to non-convergence), the fundamental cause stems from the illness of divergence: f-divergence based GANs (including vanilla / original / standard GANs) would fail to effective provided gradient for generator's update, because it will become infinite or constant when the supports of the generation distribution and target / real distribution are not (fullly) overlapped, which typically exists in the begining of the training and even the ending of the training. (not very exact, but I tried my current best to simply it)

- The propose solution is to switch to another type of divergence / distance that can well operate when the supports are not (fullly) overlapped. W-distance is one of the typical instance proposed. (there should be a group of such divergence / distance, like f-divergence; W-distance is somehow a special case of optimal transport)

- I view this above as the traditional understanding of the training instability issue of GANs. Our work LGANs provides a more experienced perspective, that is the optimal discriminative function (f*, see the paper for an accurate definition, here you can simply understand it as D*) view. By inspecting f* and its gradient with respect to samples, the understanding of GANs's training can be much more clear. The reason is that we are now considering the G-D structure of GANs and we are inspecting the samples (instead of the densities) and the gradients that the generator receives from the discriminator (i.e., f*) with respect to the samples to be updated. That is to inspect the connecting point of G-D. G: the samples to be updated and update them accordingly; D or f* or the gradient of f*: how should these samples be updated. 

- According to LGANs, the convergence of GANs heavily depends on the regularization in the discriminative function space (whether there is a regularization in the discrimintor and what regularization it is). We show that if there is no regularization in the discriminative function space, the GANs definitely does not guarantee its convergence, provablely suffering a gradient uninformativeness issue (the gradient that the generator received from the discriminator does not tell any information of the target / real distribution). We also find that this gradient uninformativeness issue is non-trivial, not any single simple regularization in the discriminative function space can resolve the gradient uninformativeness issue. 

- Hoever, interestingly, Lipschitz regularization can generally resolve the gradient uninformativeness issue and guarantee the GANs's convergence. We provide a sufficient condition for these GANs (which we believe is very close to the neccesary condition for GANs where the discriminator has only a single input sample). We provide detailed analysis upon why Lipschitz regularization can generally resolve the gradient uninformativeness issue and show that Lipschitz regularization makes the gradients with respect to generated samples point directly towards real samples (i.e., samples in target distributions). We prove the existence and uniqueness of f* for GANs under Lipschitz regularization. We prove that there is only a single pure nash equilibrium between G and f*/D*, otherwise, the GANs will always moving samples from locations where has too much to localtions where has too less. The above leads to the LGANs, a GANs family. We have constructed several instances of this GANs family, and showed their consistent superior performance over WGAN. (We believe gradient penalty / restriction / regularization based methods all have similar effect, based on our analysis upon how Lipschitz regularization works.)

- We suggest use MaxGP instead of GP (gradient penalty) / LP (Lipschitz penalty) / SN (spectral normalization). All the thought are written in https://arxiv.org/abs/1904.01184, but I still not get a time to improve and perfect the experiments, so I would just keep it as a arXiv report for now. The basic idea is that: Lipschitz constant is equivalent to the maximum norm of the gradients; this is the basic intuition of GP and LP (I beleive the intuition in WGAN-GP for propose GP is not accurate, the relatively correct version should be what I have stated.), but GP is not directly penalizing the Lipschitz constant (which includes superfluous constraints and hence biases the optimum state), and even LP has a drawback (though it penalizing all gradients larger than K, there are also superfluous constraints, for these in the middle of K and the current Lipschitz constant / max gradient norm, and hence still biased the optimum state), in contrast, MaxGP is the correct implementation (with which I finally get the optimal discriminative function, for small / easy task, GP and LP both fail, SN also fail to achieve the optimum in many cases).  SNGAN makes SN popular, but according to my experiments, SN fails much more often, comparing to MaxGP (see the paper for more details; I suspect the cause stems from the over-restriction of SN). MaxGP has a drawback too, it does not achieve Lipschitz constant K. In https://arxiv.org/abs/1904.01184, we also proposed an Augmented Lagrangian (AL) method (MaxAL), which can almost exactly achieve "Lipschitz constant = K". MaxAL can be benefitial sometimes, like when you are estimating the W-distance between two distribution. With MaxGP, you need to devide the result by "the current Lipschitz constant", though it can be easily estimated by max gradient norm, but MaxAL does not need the division. (See the paper for all the details.)

- Actually, all previous descriptions is based on an assumption, i.e., the so-called Lipschitz is with respect to the Euclidean distance / norm. When switch to other norms the properly will get changed. See my arXiv https://arxiv.org/abs/1807.00751 for some basic arguments on this. https://arxiv.org/abs/1806.06621 (Banach WGAN) might also help your understanding. 

- 

About first-order optimization and Adam:

- We will first view Adam from the first-order optimization view, but with v_t playing the rule of gradient scale estimation, it then somehow connects to the traditional second-order view. 

- Adam is proved to have a convergence issue, and counterexamples can be constructed. In the paper of AdaShift, we show that the nonconvergence comes from the positive correlation of the current adaptive term v_t and the current graient g_t, because the update rule is v_t = \beta2 v_(t-1) + (1-\beta2) g_t, i.e., the correlation factor is 1-\beta2. Such a positive correlation would lead to bias net update factor. 

- The net update factor of g_t can be understood as its accumulated step-size in the entire optimization, because its influence can be delayed to future updates, due to first moment estimation or otherwise named the moving average windows. The influence of g_t decreases at a rate of \beta1 each step and is initialized with a ratio 1-\beta1, which sums to one. (This is similar to Momentum and SGD, where the net update factor of each gradient is also one.)

- However, for adapative learning rate methods (Adam as a representative), the net update factor of each gradient does not have a fixed value (hence, not the same) nor follow a fixed distribution (which we believe have a similar effect as fixed value choices, Momentum and SGD). 

- And obviously, if v_t is independent of g_t and follows a fixed distribution, then, the net update factor of g_t, i.e., its accumulated step-size, follows a fixed distribution (which then leads to a convergence guarantee that similar to Momentum and SGD). This is the centre thought of AdaShift solution. 

- To achieve "follow a fixed distribution", we propose to temporally shift the gradient for the calculation of v_t. In such condition, if "moving average windows" is disabled (i.e., \beta1=0), and if g_t follows a fixed distribution, then v_t also follows a fixed distribution. However, "if moving average windows is disabled" turns out to be the limitation of AdaShfit. Nevertheless, we propose to shift the gradient for multiple steps, then, the "leave-out" gradients that still not get involved to v_t can be moving averaged or simply averaged if you like. A new version of AdaShift is coming and we will fix this issue. Looking forward to the new *free-lunch solution* to the non-convergence issue of Adam! 

- Given the previous anatomy of adaptive learning rate methods, the key of its convergence is to force v_t to be independent of g_t and to follow a fixed distribution. In this sense, the role of v_t is to *estimate the scale of the gradient* (because we know that the key benefit of adaptive learning rate method is scale invariance, which means, the scale of the gradient is removed, making it easy to use, especially in multi-layer neural network, where the gradient' scales can change dramatically in different layers. given the gradient's scale invariance, it is much easier to turn a good learning rate). 

- Because v_t is to somehow estimate the scale of the gradient, it can also estimate the overall gradient scale, or layerwise / blockwise graident scale. In doing this, it reduces to adaptive learning rate SGD (with each block share the same v_t, and overall gradient scale in each block is removed, but the relative gradient scale is keep in the block), which makes it extremely suitable for optimizing a multi-layer neural network. 

- The update rule of v_t can even be generalized. Try and find more interesting update rules, as long as it estimates the scale of the gradient!
