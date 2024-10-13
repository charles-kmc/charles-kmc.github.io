---
layout: post
title: a step by step diffusion models
date: 2024-10-09 17:39:00
description:
# tags: formatting math
categories: generative_models
# related_posts: false
---

<h3> Introduction </h3>
Diffusion model ...
$$
\sum_{k=1}^\infty |\langle x, e_k \rangle|^2 \leq \|x\|^2
$$

$$
\begin{equation}\label{eq: test}
\sum_{k=1}^\infty |\langle x, e_k \rangle|^2 \leq \|x\|^2
\end{equation}
$$

You \eqref{eq: test} can also use `\begin{equation}...\end{equation}` instead of `$$` for display mode math.
MathJax will automatically number equations:

\begin{equation}
\label{eq:cauchy-schwarz}
\left( \sum*{k=1}^n a_k b_k \right)^2 \leq \left( \sum*{k=1}^n a*k^2 \right) \left( \sum*{k=1}^n b_k^2 \right)
\end{equation}

and by adding `\label{...}` inside the equation environment, we can now refer to the equation using `\eqref`.

Note that MathJax 3 is [a major re-write of MathJax](https://docs.mathjax.org/en/latest/upgrading/whats-new-3.0.html) that brought a significant improvement to the loading and rendering speed, which is now [on par with KaTeX](http://www.intmath.com/cg5/katex-mathjax-comparison.php).
