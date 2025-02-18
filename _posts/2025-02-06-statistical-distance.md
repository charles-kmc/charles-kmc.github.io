---
layout: post
title: Common statistical ways to measure distance between two distributions
date: 2025-02-17 17:39:00
description:
# tags: formatting math
categories: generative-models
# related_posts: false
---

<h3> Introduction </h3>
In this block, we will discuss common distances and metrics between distributions that are essential in statistics.

Let consider a measurable space $$ \mathcal{M}=\left(\Omega, \mathcal{F}\right) $$ and two probability measures $$P$$ and $$ Q $$ defined of $$\mathcal{M}$$. We say $$ Q $$ dominate $$ P  $$ when the following statement is true. If $$ Q(A)=0 $$ for some set $$ A $$ then it has to be the case that $$ P(A) $$ is also $$ 0 $$.

<h3> Total variation (TV) distance </h3>
Total variation distance is a statistical distance between two probability distributions. Mathematically, it is defined as follows

\begin{equation}
    \text{TV}(P,Q) = \sup_{A\in\mathcal{F}}|P(A) - Q(A)|,
\end{equation}

where $$ A $$ is a measurable set. Precisely, total variation distance is the largest absolute distance between probabilities that the two probability distributions assign to the same event. In other word, it measures the maximum difference between the probability of an event under $$ p $$ and under $$ Q $$.

When $$ P $$ and $$ Q $$ are associated with probability densities $$ p $$ and $$ q $$ respectively, the total variation distance become,

\begin{equation}\label{eq:tv2}
    \text{TV}(P,Q)= \frac{1}{2}\int_{x \in A} |p(x) - q(x)|dx.
\end{equation}

Notice that \eqref{tv2} reveals that TV distance is equivant the $$\ell_1$$ distance between densities.

<h3> Kullback-Leibler (KL) divergence </h3>
Introduced by Solomon Kullback and Richard Leibler, KL divergence (also called relative entropy) is a statistical distance that measure how much a model probability $$P$$ is different from a true probability distribution $$Q$$. For continuous probability distribution $$P$$ and $$Q$$, the KL divergence is given by,

\begin{equation}
    \text{D_{KL}}(P,Q) = \int p(x) \log \left(\dfrac{p(x)}{q(x)}\right)dx.
\end{equation}

For discrete probability distribution $$P$$ and $$Q$$, the KL divergence is given by,

\begin{equation}
    \text{D_{KL}}(P,Q) = \sum_{x} p(x) \log \left(\dfrac{p(x)}{q(x)}\right)dx.
\end{equation}


KL divergence if not symmetric $$\text{D_{KL}}(P,Q) \neq \text{D_{KL}}(Q,P)$$ and does not statisfy the triangle inequality. Consequently, KL divergence is not a metric.

In real application, KL divergence is used when one want to approximation a complex true distribution $$P$$ with a simple approximate $$Q$$ which is most case is Gaussian. This technique is quite used in situation where it is easier to compute, such as expectation-maximazation algorithm (EM) and evidence lower bound (ELBO) computations.

Here we have some properties of KL divergence.

* Consider two multivariate Gaussian distributions $$P_1=\mathcal{N}(\mu_1, \Sigma_1)$$ and $$P_2=\mathcal{N}(\mu_2, \Sigma_2)$$, the KL deivergence between $$P_1$$ and $$P_2$$ has a close form expression given by

\begin{equation}
    \text{D_{KL}}(P_1, P_2) = \frac{1}{2}\left(\text{tr}(\Sigma^{-1}_2\Sigma_1) -d + (\mu_2-\mu_1)^\top\Sigma_2^{-1}(\mu_2-\mu_1) + \ln\left(\dfrac{\text{det}\Sigma_2}{\text{det}\Sigma_1}\right)\right)
\end{equation}

* Consider two uniform distributions $$P_1=\mathcal{U}(A, B)$$ and $$P_2=\mathcal{U}(C,D)$$, the KL deivergence between $$P_1$$ and $$P_2$$ has a close form expression given by

\begin{equation}
    \text{D_{KL}}(P_1, P_2) =\log\left(\dfrac{D-C}{B-A}\right).
\end{equation}
    

<h3> Wasserstein distance </h3>
Named after Leonid Vaserstein, wasserstein distance also named Kantorovich-Rubinstein metric is a distance nction between probability distributions on a given metric spaces $$X$$.

Let condider $$\left(M, d\right)$$ be a metric space. For $$p\in\left[1, +\infty\right]$$, the Wasserstein $$p-$$distance between two probability measures $$\mu$$ and $$\nu$$ on $$M$$ is given by

\begin{equation}
    W_p(\mu,\nu) = \inf_{\gamma \in \Gamma(\mu,\nu)} \left(\mathbb{E}_{x,y \sim \gamma}d(x,y)^p\right)^{\frac{1}{p}},
\end{equation}

where $$\Gamma(\mu,\nu)$$ is the set of couplings (joint probability) of $$\mu$$ (marginal) and $$\nu$$ (marginal).

When $$P$$ and $$Q$$ are empirical distributions with samples $$X_1, \dots,X_n$$ and $$Y_1,\dots,Y_n$$ respectively, the wasserstein $$p-$$distance is given by

\begin{equation}
    W_p(P,Q) = \left(\frac{1}{n}\sum_{i=1}^n||X_i-Y_i||^p\right)^{\frac{1}{p}}.
\end{equation}

In practical application, wesserstein distance is a natural way to compare probability distributions of two random variables $$X$$ and $$Y$$, where one variable is deviated from the other by small, non-uniform pertubations.

<h3> Maximum Mean Discrepancy </h3>

<h3> Jensen-Shannon divergence </h3>

<h3> f-divergence </h3>




--- -->
