## Biography

Zhiming obtained his Ph.D. in Computer Science from [Shanghai Jiao Tong University](http://en.sjtu.edu.cn/) in 2020. He received his B.S. degree in Computer Science from the [ACM Class](https://acm.sjtu.edu.cn/home) at Shanghai Jiao Tong University in 2014.

Zhiming’s research is mainly focused on generative adversarial networks (GANs). Leading a group in the [Apex Lab](http://apex.sjtu.edu.cn/members) at Shanghai Jiao Tong University, he also works on first-order optimization, optimal transport, and other related problems. Prior to that, Zhiming worked on computer graphics in the early years of his Ph.D. (2014-2016), focused on surface reflectance acquisition.

Zhiming has a broad interest in machine learning and deep learning, and he prefers fundamental and theoretical research. Currently, he holds a special interest in the optimization and generalization of deep neural networks and GANs.

## Documents & Links

- [CV](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/Zhiming_Zhou_Resume.pdf) 
  
- [Github](https://github.com/ZhimingZhou)

- [Google Scholar](https://scholar.google.com/citations?user=b8YJ1EMAAAAJ&hl=en)

- [DBLP](https://dblp.org/pers/hd/z/Zhou:Zhiming)
  
- [Talk] [On the Key Problems of GANs](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/On%20the%20Key%20Problems%20of%20GANs.pptx)

  - Training issues  
    - Instability (LGANs)    
    - Unreachable optimum (MaxGP, AdaShift, Ongoing)    
  - Sample Quality issues  
    - Complex dataset (AM-GANs)    
    - Latent space (TODO)    
  - Generalization issue (Ongoing)  

- [Talk] [On the Convergence Issues of GANs](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/On%20the%20Convergence%20Issues%20of%20GANs.pptx)

  - Training instability (LGANs)  
  - Unreachable optimum (MaxGP, AdaShift, Ongoing)  
  - Generalization issue (Ongoing)    
  
## Selected Publications 

Lipschitz Regularized Generative Adversarial Nets. (LGANs<sup>+</sup> + MaxGP<sup>+</sup> + MaxAL + Many Related Analyses)
- **Zhiming Zhou**, [Zhihua Zhang](http://www.math.pku.edu.cn/teachers/zhzhang/).
- Submitted to the Journal of Machine Learning Research (JMLR).
- \[[arXiv](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/Lipschitz_Regularized_GANs.pdf)\]
  \[[Code1](https://github.com/ZhimingZhou/AdaShift-LGANs-MaxGP-refactored)\]
  \[[Code2](https://github.com/ZhimingZhou/LGANs-for-reproduce)\]
  \[[Code3](https://github.com/ZhimingZhou/MaxGP-MaxAL-for-reproduce)\]
- <details><summary>Click to expand a brief introduction.</summary>This is a substantially extended version of "Lipschitz Generative Adversarial Nets", aimed at a comprehensive understanding on the training instability issue and convergence of GANs. We provide a thoroughgoing study upon Lipschitz regularization and Lipschitz regularized GANs, both theoretically and empirically. We thereby achieve consistently superior performance over WGANs with theoretical justification. We provide a systematic study on the gradient issues of unregularized GANs (including the gradient uninformativeness) and their practical behaviors, from which we venture a conjecture on the mechanisms of how unregularized GANs work in practice and find a fundamental cause of mode collapse, i.e., the locality of their gradient information. We study the differentiation properties of GANs with the help of the envelope theorem and realize that the current GANs is essentially a sample-based framework and the information interchange between the generator and the discriminator must be passed via the gradients of the discriminative function with respect to generated samples, because the discriminator takes a sample as input.</details>

Lipschitz Generative Adversarial Nets. (LGANs + MaxGP)
- **Zhiming Zhou**, Jiadong Liang, [Y. Song](https://yuxuansong.github.io/files/yuxuan_20Mar.pdf), [L. Yu](http://lantaoyu.com/), [H. Wang](https://cs.stanford.edu/~hongweiw/), [Weinan Zhang](http://wnzhang.net/), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu), [Zhihua Zhang](http://www.math.pku.edu.cn/teachers/zhzhang/).
- The Thirty-sixth International Conference on Machine Learning (ICML, 2019).
- \[[arXiv](https://arxiv.org/abs/1902.05687)\]
  \[[Slide](https://icml.cc/media/Slides/icml/2019/halla(11-14-00)-11-15-10-4628-lipschitz_gener.pdf)\]
  \[[Poster](https://s3.amazonaws.com/postersession.ai/ee90cc20-a261-4aee-b28f-899891a90be3.pdf)\]
  \[[Code1](https://github.com/ZhimingZhou/AdaShift-LGANs-MaxGP-refactored)\]
  \[[Code2](https://github.com/ZhimingZhou/LGANs-for-reproduce)\]
  \[[Code3](https://github.com/ZhimingZhou/MaxGP-MaxAL-for-reproduce)\]
- <details><summary>Click to expand a brief introduction.</summary>We study the cause of training instability of GANs from the perspective of optimal discriminative function and demonstrate its superiority against the divergence perspective. Under a generalized formulation of GANs, we show that: (1) GANs with unrestricted discriminative function space generally does not guarantee its convergence, suffering from a *gradient uninformativeness issue*; (2) Lipschitz regularization on the discriminative function can generally resolve this issue and guarantee the convergence of GANs, leading to a new family of GANs named Lipschitz GANs. All tested instances of this family consistently outperform WGANs in experiments.</details>

AdaShift: Decorrelation and Convergence of Adaptive Learning Rate Methods. (AdaShift)
- **Zhiming Zhou**\*, Qingru Zhang\*, Guansong Lu, [Hongwei Wang](https://cs.stanford.edu/~hongweiw/), [Weinan Zhang](http://wnzhang.net/), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu).
- The Seventh International Conference on Learning Representations (ICLR, 2019).
- \[[arXiv](https://arxiv.org/abs/1810.00143)\]
  \[[OpenReview](https://openreview.net/forum?id=HkgTkhRcKQ)\]
  \[[Poster](https://s3.amazonaws.com/postersession.ai/bd0f7f0b-ecaa-4164-aeb6-d0cf181cc27b.jpg)\]
  \[[Code](https://github.com/ZhimingZhou/AdaShift-LGANs-MaxGP-refactored)\]
- <details><summary>Click to expand a brief introduction.</summary>We study the convergence issue of Adam optimizer. With the proposed concept *net update factor*, we showed that the key issue in Adam lies in its biased adaptive learning rate caused by the correlation between the adaptive term v_t and the current gradient g_t, and a temporal shift operation is proposed to solve such an issue. Our new understanding of the role of v_t also free v_t from its traditional update rule, leading to more interesting variants. Particularly, with dimension reduction operation in v_t, we achieve the so-called adaptive learning rate SGD, which removes the global gradient scale but keeps the relative scales.</details>

Activation Maximization Generative Adversarial Nets. (AM-GANs)
- **Zhiming Zhou**, [Han Cai](https://han-cai.github.io/files/cv.pdf), Shu Rong, [Yuxuan Song](https://yuxuansong.github.io/files/yuxuan_20Mar.pdf), [Kan Ren](http://www.saying.ren/), [Weinan Zhang](http://wnzhang.net/), [Jun Wang](http://www0.cs.ucl.ac.uk/staff/Jun.Wang/), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu).
- The Sixth International Conference on Learning Representations (ICLR, 2018).
- \[[arXiv](https://arxiv.org/abs/1703.02000)\]
  \[[OpenReview](https://openreview.net/forum?id=HyyP33gAZ&noteId=HyyP33gAZ)\]
  \[[Code1](https://github.com/ZhimingZhou/AM-GANs-refactored)\]
  \[[Code2](https://github.com/ZhimingZhou/AM-GANs-for-reproduce)\]
- <details><summary>Click to expand a brief introduction.</summary>We study how class labels interact with GANs training when introduced and how it improves the sample quality of GANs. Based on the analysis, an improved method for leveraging class labels in GANs had been proposed. An interesting relationship among popular variants of GANs that leverage class labels, including the proposed AM-GANs, are unraveled.</details>

Sparse-as-Possible SVBRDF Acquisition. (SparseSVBRDF)
- **Zhiming Zhou**, Guojun Chen, [Yue Dong](http://yuedong.shading.me/), [David Wipf](\href{http://www.davidwipf.com/home.html), [Yong Yu](http://apex.sjtu.edu.cn/members/yyu), [John Snyder](https://www.microsoft.com/en-us/research/people/johnsny/), [Xin Tong](http://www.xtong.info/).
- ACM Transactions on Graphics (TOG) - Proceedings of ACM SIGGRAPH Asia, 2016. 
- \[[PDF](http://yuedong.shading.me/project/sparsesvbrdf/sparsesvbrdf.pdf)\] 
  \[[ACM](https://dl.acm.org/doi/10.1145/2980179.2980247)\]
  \[[Slide](https://drive.google.com/file/d/16gUKZoQH4HiQ61gEQ-YFs6v9WTEOSixf/view?usp=sharing)\]
- <details><summary>Click to expand a brief introduction.</summary>We significantly reduce the number of images required for spatially-varying surface reflectance (SVBRDF) acquisition, by solving an exact low-rank representation and chasing an extreme sparsity. The number of images required dropped from thousands to tens, and high-quality SVBRDF acquisition from a single image became possible for the first time.</details>

## Photos

![Me](https://github.com/ZhimingZhou/zhimingzhou.github.io/raw/master/1.png)

## MISC

- About GANs:

  - GANs & its usages:

    - GANs is just a tool that maps one distribution to another. GANs can be useful, when and only when, it can be properly used. 

    - Given the generalization issue (cannot generalize when trained to optimum, memorizing the training distribution), theoretically sound usages are very limited. Two typical that I know are optimal transport (where the target distribution sometimes can just be the data provided and does not need generalization) and data modeling (where the data provided can just be the data to be modeled and somehow does not need generalization). 

    - Other typical usages include: image (or any other data) synthesis, forcing the output distribution to a given distribution (like GANs for super-resolution and transferring). GANs can also be used for conditional diverse outputs, which is just like image synthesis, but being conditional, and the diversity comes from the freedom of the unconditioned parts. 

    - I think any GANs should has a 's' at the tail, because the *networks* in *adversarial neural networks* means G and D. Hence need the 's'. I believe this is also why Ian Goodfellow adds the 's'. I was also confused for a long time whether I should add the 's'. But now, I believe there should be a 's', always.
    
    - GANs has both a PLURAL sense and a SINGULAR sense, and they share the SAME form, i.e., "GANs". 

      - When terming as a concept, we should use SINGULAR sense;
      - When referring to a specific GANs, like WGANs, we should also use the SINGULAR sense;
      - But when referring to a class / set / type of GANs, we should use the PLURAL sense.

    - For the possessive, we can use "the xxx of GANs" or "GANs' xxx", e.g., the convergence of GANs, GANs' training.

      - Sometimes, it might be more natural to directly use "GANs xxx", e.g., GANs objective. 

  - GANs summary / review:

    - Popular research topics in GANs include:
      - Objective function: 
        - [2014.06 original gans](https://arxiv.org/abs/1406.2661) 
        - [2014.11 conditional gans / cgans](https://arxiv.org/abs/1411.1784)
        - [2016.11 least square gans](https://arxiv.org/abs/1611.04076) 
          - [2016.09 energy based gans](https://arxiv.org/abs/1609.03126)
          - [2016.10 density ratio](https://arxiv.org/abs/1610.02920)
          - [2017.07 f-gans](https://arxiv.org/abs/1707.04385)      
        - [2017.01 towards principled methods](https://arxiv.org/abs/1701.04862)
        - [2017.01 wgans](https://arxiv.org/abs/1701.07875)
        - [2017.04 wgans-gp](https://arxiv.org/abs/1704.00028)
        - [**2019.02 lgans**](https://arxiv.org/abs/1902.05687)
      - Lipschitz implementation: 
        - [2017.01 weight clipping in wgans](https://arxiv.org/abs/1701.07875)
        - [2017.04 gp in wgans-gp](https://arxiv.org/abs/1704.00028)
        - [2017.09 lp in wgans-lp](https://arxiv.org/abs/1709.08894) 
        - [2018.02 sn in sngan](https://arxiv.org/abs/1802.05957)
        - [**2019.02 maxgp in lgans**](https://arxiv.org/abs/1902.05687)
        - [**2019.04 maxal**](https://arxiv.org/abs/1904.01184)
      - Sample quality:
        - [2016.06 labelgans](https://arxiv.org/abs/1606.03498)
        - [2016.10 acgans](https://arxiv.org/abs/1610.09585)
        - [2015.11 catgans](https://arxiv.org/abs/1511.06390) 
        - [**2017.03 amgans**](https://arxiv.org/abs/1703.02000) 
          - possible extension: am-wgans / am-lgans
        - [2019.11 another catgans](https://arxiv.org/abs/1911.06641)
      - GANs based tools:
        - [**2017.02 diverse colorization**](https://arxiv.org/abs/1702.06674)
        - [2017.03 cycle gans](https://arxiv.org/abs/1703.10593)
        - [**2018.11 ot-cycle gans**](https://arxiv.org/abs/1811.06284) 
        - [**2020.03 large scale ot with cycle consistency**](https://arxiv.org/abs/2003.06635)
      - Generalization issue / sub-optimum analysis: 
        - [2017.03 generalization and equilibrium](https://arxiv.org/abs/1703.00573) 
        - [2017.11 discrimination-generalization tradeoff](https://arxiv.org/abs/1711.02771)
        - [2018-xx convex duality framework](http://papers.nips.cc/paper/7771-a-convex-duality-framework-for-gans)
        - One of my ongoing work, appear soon.
      - Optimization: 
        - [2016.11 unrolled](https://arxiv.org/abs/1611.02163) 
        - [2017.05 the numerics](http://papers.nips.cc/paper/6779-the-numerics-of-gans)
        - [2017.06 two time scale](https://arxiv.org/abs/1706.08500)     
        - [2017.06 optimization is locally stable](https://arxiv.org/abs/1706.04156)     
        - [2017.11 training gans with optimism](https://arxiv.org/abs/1711.00141) 
        - [2018.01 which do actually converge?](https://arxiv.org/abs/1801.04406)
      - Latent space / GANs with AE:
        - [2016.05 bi-gans](https://arxiv.org/abs/1605.09782) 
        - [2016.06 ali](https://arxiv.org/abs/1606.00704)
        - [2016.06 info-gans](https://arxiv.org/abs/1606.03657)           
        - [2016.12 mode regularized gans](https://arxiv.org/abs/1612.02136)
        - [2017.06 deli-gans](https://arxiv.org/abs/1706.02071)    
        - [2018.04 manifold guided training](https://arxiv.org/abs/1804.04391)
        - [2018.05 metric-embeddings / bourgan](https://arxiv.org/abs/1805.07674)
        - [2018.06 disconnected manifold learning](https://arxiv.org/abs/1806.00880)
        - [2019.11 multimodal distributions](https://arxiv.org/abs/1911.06663)    
      - Network architecture: 
        - [2015.06 laplace gans](https://arxiv.org/abs/1506.05751) 
        - [2015.11 dcgans](https://arxiv.org/abs/1511.06434) 
        - [2017.10 progressive growing gans](https://arxiv.org/abs/1710.10196) 
        - [2018.05 self attention gans](https://arxiv.org/abs/1805.08318) 
        - [2018.09 big gans](https://arxiv.org/abs/1809.11096) 
      - Systematic study / test: 
        - [2017.06 do actually learn the distribution?](https://arxiv.org/abs/1706.08224) 
        - [2017.10 many paths to equilibrium](https://arxiv.org/abs/1710.08446) 
        - [2017.11 are gans created equal?](https://arxiv.org/abs/1711.10337)
        - [2018.07 the gans landscape / regularization and normalization](https://arxiv.org/abs/1807.04720)
    
    - I personally do not follow the optimization path, because I don't think the key problem lies in optimization (and I'm also not sure whether it is valid to regard GANs as a Game). Until Adam is shown to not guarantee its convergence, we then have a work AdaShfit to solve the non-convergence issue of Adam. But after that, I still don't think the key problem lies in optimization.
    
    - I believe GANs are not equally created. In the objective function line, GANs is getting mature and mature. In the network architecture line, it is also getting mature and mature (though maybe network architecture is not the key, so I would not put much effort in this line). Application tools with GANs are also interesting which I also follow.
    
    - This summary is not aimed to be inclusive, but as a guide on the road-map / development history of GANs, and at the same time, provide one taxonomy. If necessary, the authors can email me or use pull requests.
    
    - By the way, I use "google related articles" & [google scholar](https://scholar.google.com/) & [google](https://www.google.com/) & [arXiv](https://arxiv.org/) to efficiently finish this paper search, tracing, and summary.

- About first-order optimization and Adam:

  - We will first view Adam from the first-order optimization view, but with v_t playing the rule of gradient scale estimation, it then somehow connects to the traditional second-order view. 

  - Adam is proved to have a convergence issue, and counterexamples can be constructed. In the paper of AdaShift, we show that the non-convergence comes from the positive correlation of the current adaptive term v_t and the current gradient g_t, because the update rule is v_t = \beta2 v_(t-1) + (1-\beta2) g_t, i.e., the correlation factor is 1-\beta2. Such a positive correlation would lead to bias net update factor. 

  - The net update factor of g_t can be understood as its accumulated step-size in the entire optimization, because its influence can be delayed to future updates, due to first moment estimation or otherwise named the moving average windows. The influence of g_t decreases at a rate of \beta1 each step and is initialized with a ratio 1-\beta1, which sums to one. (This is similar to Momentum and SGD, where the net update factor of each gradient is also one.)

  - However, for adaptive learning rate methods (Adam as a representative), the net update factor of each gradient does not have a fixed value (hence, not the same) nor follow a fixed distribution (which we believe have a similar effect as fixed value choices, Momentum and SGD). 

  - And obviously, if v_t is independent of g_t and follows a fixed distribution, then, the net update factor of g_t, i.e., its accumulated step-size, follows a fixed distribution (which then leads to a convergence guarantee that similar to Momentum and SGD). This is the central thought of the AdaShift solution. 

  - To achieve "follow a fixed distribution", we propose to temporally shift the gradient for the calculation of v_t. In such a condition, if "moving average windows" is disabled (i.e., \beta1=0), and if g_t follows a fixed distribution, then v_t also follows a fixed distribution. However, "if moving average windows is disabled" turns out to be the limitation of AdaShfit. Nevertheless, we propose to shift the gradient for multiple steps, then, the "leave-out" gradients that still not get involved to v_t can be moving averaged or simply averaged if you like. A new version of AdaShift is coming and we will fix this issue. Looking forward to the new *free-lunch solution* to the non-convergence issue of Adam! 

  - Given the previous anatomy of adaptive learning rate methods, the key of its convergence is to force v_t to be independent of g_t and to follow a fixed distribution. In this sense, the role of v_t is to *estimate the scale of the gradient* (because we know that the key benefit of adaptive learning rate method is scale invariance, which means, the scale of the gradient is removed, making it easy to use, especially in multi-layer neural networks, where the gradient' scales can change dramatically in different layers. given the gradient's scale invariance, it is much easier to turn a good learning rate). 

  - Because v_t is to somehow estimate the scale of the gradient, it can also estimate the overall gradient scale, or layer-wise / block-wise gradient scale. In doing this, it reduces to adaptive learning rate SGD (with each block sharing the same v_t, the overall gradient scale in each block is removed, but the relative gradient scale is kept in the block), which makes it extremely suitable for optimizing a multi-layer neural network. 

  - The update rule of v_t can even be generalized. Try and find more interesting update rules, as long as it estimates the scale of the gradient!
