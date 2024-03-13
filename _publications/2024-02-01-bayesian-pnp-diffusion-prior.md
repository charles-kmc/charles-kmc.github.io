---
title: "A stochastic optimisation unadjusted Langevin method for empirical Bayesian estimation in semi-blind image deblurring problems"
collection: publications
permalink: /publication/2024/02/2024-02-01-pnp-score-based
excerpt: 'This paper presents a novel stochastic optimisation methodology to perform empirical Bayesian inference in semi-blind image deconvolution problems. Given a blurred image and a parametric class of possible operators, the proposed optimisation approach automatically calibrates the parameters of the blur model by maximum marginal likelihood estimation, followed by (non-blind) image deconvolution by maximum-a-posteriori estimation conditionally to the estimated model parameters. In addition to the blur model, the proposed approach also automatically calibrates the noise variance as well as any regularisation parameters. The marginal likelihood of the blur, noise variance, and regularisation parameters is generally computationally intractable, as it requires calculating several integrals over the entire solution space. Our approach addresses this difficulty by using a stochastic approximation proximal gradient optimisation scheme, which iteratively solves such integrals by using a Moreau-Yosida regularised unadjusted Langevin Markov chain Monte Carlo algorithm. This optimisation strategy can be easily and efficiently applied to any model that is log-concave, and by using the same gradient and proximal operators that are required to compute the maximum-a-posteriori solution by convex optimisation. We provide convergence guarantees for the proposed optimisation scheme under realistic and easily verifiable conditions and subsequently demonstrate the effectiveness of the approach with a series of deconvolution experiments and comparisons with alternative strategies from the state of the art.'
date: 2024-02-01
venue: 'SIAM'
paperurl: 'https://arxiv.org/pdf/2403.04536'
citation: 'Kemajou Mbakam, Charlesquin and Pereyra, Marcelo and Giovannelli, Jean-François (2023). &quot;A stochastic optimisation unadjusted Langevin method for empirical Bayesian estimation in semi-blind image deblurring problems.&quot; <i>SIAM</i>.'
index: 20240201
code_link: "https://github.com/charles-kmc"
tags:
  - paper
---





<!-- ---
title: "Empirical Bayesian image restoration by Langevin sampling with a denoising diffusion implicit prior"
collection: publications
permalink: /publication/2024/02/2024-02-14-bayesian-pnp-diffusion-prior
excerpt: 'Score-based diffusion methods provide a powerful strategy to solve image restoration tasks by flexibly combining a pre-trained foundational prior model with a likelihood function specified during test time. Such methods are predominantly derived from two stochastic processes: reversing Ornstein-Uhlenbeck, which underpins the celebrated denoising diffusion probabilistic models (DDPM) and denoising diffusion implicit models (DDIM), and the Langevin diffusion process. The solutions delivered by DDPM and DDIM are often remarkably realistic, but they are not always consistent with measurements because of likelihood intractability issues and the associated required approximations. Alternatively, using a Langevin process circumvents the intractable likelihood issue, but usually leads to restoration results of inferior quality and longer computing times. This paper presents a novel and highly computationally efficient image restoration method that carefully embeds a foundational DDIM denoiser within an empirical Bayesian Langevin algorithm, which jointly calibrates key model hyper-parameters as it estimates the model's posterior mean. Extensive experimental results on three canonical tasks (image deblurring, super-resolution, and inpainting) demonstrate that the proposed approach improves on state-of-the-art strategies both in image estimation accuracy and computing time.'
date: 2024-02-14
venue: '(Stay tuned !!)'
paperurl: 'https://arxiv.org/pdf/2403.04536'
citation: 'Kemajou Mbakam, Charlesquin and Pereyra, Marcelo and Giovannelli, Jean-François (2024). &quot;Empirical Bayesian image restoration by Langevin sampling with a denoising diffusion implicit prior.&quot; <i>ECCV</i>.'
index: 20240214
code_link: "https://github.com/charles-kmc"
tags:
  - paper
--- -->