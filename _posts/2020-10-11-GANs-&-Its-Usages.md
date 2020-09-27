---
layout: post
title: GANs & Its Usages
permalink: /Posts/GANs-&-Its-Usages/
date: 2020-08-26
---

- GANs is just a tool that maps one distribution to another. GANs can be useful, when and only when, it can be properly used. 

- Given the generalization issue (cannot generalize when trained to optimum, memorizing the training distribution), theoretically sound usages are very limited. Two typical that I know are optimal transport (where the target distribution sometimes can just be the data provided and does not need generalization) and data modeling (where the data provided can just be the data to be modeled and somehow does not need generalization). 

- Other typical usages include: image (or any other data) synthesis, forcing the output distribution to a given distribution (like GANs for super-resolution and transferring). GANs can also be used for conditional diverse outputs, which is just like image synthesis, but being conditional, and the diversity comes from the freedom of the unconditioned parts. 

- I think any GANs should has a 's' at the tail, because the *networks* in *adversarial neural networks* means G and D. Hence need the 's'. I believe this is also why Ian Goodfellow adds the 's'. I was also confused for a long time whether I should add the 's'. But now, I believe there should be a 's', always.

- GANs has both a PLURAL sense and a SINGULAR sense, and they share the SAME form, i.e., "GANs".

  - When terming as a concept, we should use SINGULAR sense;
  - When referring to a specific GANs, like WGANs, we should also use the SINGULAR sense;
  - But when referring to a class / set / type of GANs, we should use the PLURAL sense.

<!-- -->
- For the possessive, we can use "the xxx of GANs" or "GANs' xxx", e.g., the convergence of GANs, GANs' training.