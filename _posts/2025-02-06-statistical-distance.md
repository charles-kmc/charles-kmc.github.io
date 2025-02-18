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
In this block, we explore key distances and metrics between distributions that are essential in statistics. Evaluating distance between two distributions has become ubiqutous task in various research fields and applications. For instance, in generative adversarial network (GAN), the primary objective is to minimize the distance between the training distribution and the generated distribution. Another example is independence testing, where we are given samples $$(X_1, Y_1), \dots, (X_n, Y_n) \sim P_{XY}$$ and we want test the distance between the joint distribution $$P_{XY}$$ and the product of marginal distributions $$P_XP_Y$$. We discuss several important measures including total variation, KL divergence, maximum mean discrepancy, f-divergence and wasserstein distance.

Before delving into the details, let's first consider a measurable space $$ \mathcal{M}=\left(\Omega, \mathcal{F}\right) $$ and two probability distributions $$P$$ and $$ Q $$ defined of $$\mathcal{M}$$. We say $$ Q $$ dominate $$ P  $$ when the following statement hold: If $$ Q(A)=0 $$ for some set $$ A $$ then it has to be the case that $$ P(A) $$ is also $$ 0 $$.

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

Notice that \eqref{eq:tv2} reveals that TV distance is equivant the $$\ell_1$$ distance between densities.

<h3> Kullback-Leibler (KL) divergence </h3>
Introduced by Solomon Kullback and Richard Leibler, KL divergence (also called relative entropy) is a statistical distance that measure how much a model probability $$P$$ is different from a true probability distribution $$Q$$. For continuous probability distribution $$P$$ and $$Q$$, the KL divergence is given by,

\begin{equation}
    \text{D}_{KL}(P,Q) = \int p(x) \log \left(\dfrac{p(x)}{q(x)}\right)dx.
\end{equation}

For discrete probability distribution $$P$$ and $$Q$$, the KL divergence is given by,

\begin{equation}
    \text{D}_{KL}(P,Q) = \sum_{x} p(x) \log \left(\dfrac{p(x)}{q(x)}\right)dx.
\end{equation}


KL divergence if not symmetric $$\text{D}_{KL}(P,Q) \neq \text{D}_{KL}(Q,P)$$ and does not statisfy the triangle inequality. Consequently, KL divergence is not a metric.

In real application, KL divergence is used when one want to approximation a complex true distribution $$P$$ with a simple approximate $$Q$$ which is most case is Gaussian. This technique is quite used in situation where it is easier to compute, such as expectation-maximazation algorithm (EM) and evidence lower bound (ELBO) computations.

Here we have some properties of KL divergence.

* Consider two multivariate Gaussian distributions $$P_1=\mathcal{N}(\mu_1, \Sigma_1)$$ and $$P_2=\mathcal{N}(\mu_2, \Sigma_2)$$, the KL deivergence between $$P_1$$ and $$P_2$$ has a close form expression given by

\begin{equation}
    \text{D}_{KL}(P_1, P_2) = \frac{1}{2}\left(\text{tr}(\Sigma^{-1}_2\Sigma_1) -d + (\mu_2-\mu_1)^\top\Sigma_2^{-1}(\mu_2-\mu_1) + \ln\left(\dfrac{\text{det}\Sigma_2}{\text{det}\Sigma_1}\right)\right)
\end{equation}

* Consider two uniform distributions $$P_1=\mathcal{U}(A, B)$$ and $$P_2=\mathcal{U}(C,D)$$, the KL deivergence between $$P_1$$ and $$P_2$$ has a close form expression given by

\begin{equation}
    \text{D}_{KL}(P_1, P_2) =\log\left(\dfrac{D-C}{B-A}\right).
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

<h3> Maximum Mean Discrepancy (MMD) </h3>
MMD is a distance on the space of probability measures which has found numerous applications in machine learning and non-parametric testing. The distance is based on the notion of embedding probabilities in a reproducing kernel hilbert space (RKHS). This means each probability distribution is represented as an element of th RKHS. The key point is to embedded probability distributions into an infinite-dimensional features spaces, while allowing one to compare and manipulate distributions using Hilbert space operations such as inner products, distances, projections, linear transformations, and spectral analysis. 

Let $$\mathcal{F}_k$$ to be a unit ball in a reproducing kernel hilbert space, where $$k$$ is a kernel measuring similarity. The MMD between $$P$$ and $$Q$$ is defened as follows:

\begin{equation}
    \text{MMD}(P,Q) = \sup_{f\in\mathcal{F}_k}|\mathbb{E}_{X\sim P}\left[f(X)\right] - \mathbb{E}_{Y\sim Q}\left[f(Y)\right]|.
\end{equation}

This distance can be rewritten as follows

\begin{equation}
    \text{MMD}(P,Q) = \mathbb{E}_{X,X'\sim P}k(X,X') - 2\mathbb{E}_{Y\sim Q, X\sim P}k(X,Y)+ \mathbb{E}_{Y,Y'\sim P}k(Y,Y').
\end{equation}

In practical application, the MMD measure is quite used because it is simple to evaluate. Notice that MMD measure consist of expectation values for which wa can use empirical expectation.  
<h3> Jensen-Shannon divergence </h3>

<h3> f-divergence </h3>




--- -->
