---
title: "Do Bayesian imaging methods report trustworthy probabilities?"
collection: publications
permalink: /publication/2024/05/2024-05-13-do-Bayesian-imaging-methods-report-trustworthy-probabilities
excerpt: "Bayesian statistics is a cornerstone of imaging sciences, underpinning many and varied approaches from Markov random fields to score-based denoising diffusion models. In addition to powerful image estimation methods, the Bayesian paradigm also provides a framework for uncertainty quantification and for using image data as quantitative evidence. These probabilistic capabilities are important for the rigorous interpretation of experimental results and for robust interfacing of quantitative imaging pipelines with scientific and decision-making processes. However, are the probabilities delivered by existing Bayesian imaging methods meaningful under replication of an experiment, or are they only meaningful as subjective measures of belief? This paper presents a Monte Carlo method to explore this question. We then leverage the proposed Monte Carlo method and run a large experiment requiring 1,000 GPU-hours to probe the accuracy of five canonical Bayesian imaging methods that are representative of some of the main Bayesian imaging strategies from the past decades (a score-based denoising diffusion technique, a plug-and-play Langevin algorithm utilising a Lipschitz-regularised DnCNN denoiser, a Bayesian method with a dictionary-based prior trained subject to a log-concavity constraint, an empirical Bayesian method with a total-variation prior, and a hierarchical Bayesian Gibbs sampler based on a Gaussian Markov random field model). We find that, a few cases, the probabilities reported by modern Bayesian imaging techniques are in broad agreement with long-term averages as observed over a large number of replication of an experiment, but existing Bayesian imaging methods are generally not able to deliver reliable uncertainty quantification results."
date: 2024-13-015
venue: 'SIAM - Under reveiw'
paperurl: '#'
citation: 'Thong Y. W., David and Kemajou Mbakam, Charlesquin and Pereyra, Marcelo and Giovannelli, Jean-François. &quot;Do Bayesian imaging methods report trustworthy probabilities?.&quot; <i>ECCV</i>. 2024'
index: 20240201
code_link: "https://github.com/charles-kmc"
tags:
  - paper
---