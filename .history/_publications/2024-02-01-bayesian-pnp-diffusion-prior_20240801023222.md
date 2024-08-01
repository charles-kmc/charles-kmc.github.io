---
title: "Empirical Bayesian image restoration by Langevin sampling with a denoising diffusion implicit prior"
collection: publications
permalink: /publication/2024/02/2024-02-01-bayesian-pnp-diffusion-prior
excerpt: "Score-based diffusion methods provide a powerful strategy to solve image restoration tasks by flexibly combining a pre-trained foundational prior model with a likelihood function specified during test time. Such methods are predominantly derived from two stochastic processes: reversing Ornstein-Uhlenbeck, which underpins the celebrated denoising diffusion probabilistic models (DDPM) and denoising diffusion implicit models (DDIM), and the Langevin diffusion process. The solutions delivered by DDPM and DDIM are often remarkably realistic, but they are not always consistent with measurements because of likelihood intractability issues and the associated required approximations. Alternatively, using a Langevin process circumvents the intractable likelihood issue, but usually leads to restoration results of inferior quality and longer computing times. This paper presents a novel and highly computationally efficient image restoration method that carefully embeds a foundational DDIM denoiser within an empirical Bayesian Langevin algorithm, which jointly calibrates key model hyper-parameters as it estimates the model's posterior mean. Extensive experimental results on three canonical tasks (image deblurring, super-resolution, and inpainting) demonstrate that the proposed approach improves on state-of-the-art strategies both in image estimation accuracy and computing time."
date: 2024-02-01
venue: 'In preparation'
paperurl: '#'
citation: 'Kemajou Mbakam, Charlesquin and Pereyra, Marcelo and Giovannelli, Jean-François. &quot;Empirical Bayesian image restoration by Langevin sampling with a denoising diffusion implicit prior.&quot; <i>In preparation</i>. 2024'
index: 20240201
code_link: "https://github.com/charles-kmc"
tags:
  - paper
---