---
title: "Marginal Likelihood Estimation in Semiblind Image Deconvolution: A Stochastic Approximation Approach"
collection: publications
permalink: /publication/2023/07/2023-07-01-semi-blindTV
excerpt: 'This paper presents a novel stochastic optimisation methodology to perform empirical Bayesian inference in semi-blind image deconvolution problems. Given a blurred image and a parametric class of possible operators, the proposed optimisation approach automatically calibrates the parameters of the blur model by maximum marginal likelihood estimation, followed by (non-blind) image deconvolution by maximum-a-posteriori estimation conditionally to the estimated model parameters. In addition to the blur model, the proposed approach also automatically calibrates the noise variance as well as any regularisation parameters. The marginal likelihood of the blur, noise variance, and regularisation parameters is generally computationally intractable, as it requires calculating several integrals over the entire solution space. Our approach addresses this difficulty by using a stochastic approximation proximal gradient optimisation scheme, which iteratively solves such integrals by using a Moreau-Yosida regularised unadjusted Langevin Markov chain Monte Carlo algorithm. This optimisation strategy can be easily and efficiently applied to any model that is log-concave, and by using the same gradient and proximal operators that are required to compute the maximum-a-posteriori solution by convex optimisation. We provide convergence guarantees for the proposed optimisation scheme under realistic and easily verifiable conditions and subsequently demonstrate the effectiveness of the approach with a series of deconvolution experiments and comparisons with alternative strategies from the state of the art.'
date: 2023-07-01
venue: 'SIAM'
paperurl: 'https://epubs.siam.org/doi/abs/10.1137/23M1584496'
citation: 'Kemajou Mbakam, Charlesquin and Pereyra, Marcelo and Giovannelli, Jean-François (2023). &quot;Marginal Likelihood Estimation in Semiblind Image Deconvolution: A Stochastic Approximation Approach.&quot; <i>SIAM</i>.'
index: 20230701
code_link: "https://github.com/charles-kmc"
tags:
  - paper
---
