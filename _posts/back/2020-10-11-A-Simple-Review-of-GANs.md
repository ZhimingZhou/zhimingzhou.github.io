---
layout: post
author: Zhiming Zhou
date: 2020-08-28
title: A Simple Review of GANs
permalink: /Posts/A-Simple-Review-of-GANs/
comments: false
hide: true
---

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

<!--  -->
- I personally do not follow the optimization path, because I don't think the key problem lies in optimization (and I'm also not sure whether it is valid to regard GANs as a Game). Until Adam is shown to not guarantee its convergence, we then have a work AdaShfit to solve the non-convergence issue of Adam. But after that, I still don't think the key problem lies in optimization.

- I believe GANs are not equally created. In the objective function line, GANs is getting mature and mature. In the network architecture line, it is also getting mature and mature (though maybe network architecture is not the key, so I would not put much effort in this line). Application tools with GANs are also interesting, which I also follow.

- This summary is not aimed to be inclusive, but as a guide on the road-map / development history of GANs, and at the same time, provides one taxonomy. If necessary, the authors can email me or use pull requests.

- By the way, I use "google related articles" & [google scholar](https://scholar.google.com/) & [google](https://www.google.com/) & [arXiv](https://arxiv.org/) to efficiently finish this paper search, tracing, and summary.
