---
title: "A stochastic optimisation unadjusted Langevin method for empirical Bayesian estimation in semi-blind image deblurring problems"
collection: publications
permalink: /publication/2023/07/2023-07-01-semi-blindTV
excerpt: 'This paper presents a novel stochastic optimisation methodology to perform empirical Bayesian inference in semi-blind image deconvolution problems. Given a blurred image and a parametric class of possible operators, the proposed optimisation approach automatically calibrates the parameters of the blur model by maximum marginal likelihood estimation, followed by (non-blind) image deconvolution by maximum-a-posteriori estimation conditionally to the estimated model parameters. In addition to the blur model, the proposed approach also automatically calibrates the noise variance as well as any regularisation parameters. The marginal likelihood of the blur, noise variance, and regularisation parameters is generally computationally intractable, as it requires calculating several integrals over the entire solution space. Our approach addresses this difficulty by using a stochastic approximation proximal gradient optimisation scheme, which iteratively solves such integrals by using a Moreau-Yosida regularised unadjusted Langevin Markov chain Monte Carlo algorithm. This optimisation strategy can be easily and efficiently applied to any model that is log-concave, and by using the same gradient and proximal operators that are required to compute the maximum-a-posteriori solution by convex optimisation. We provide convergence guarantees for the proposed optimisation scheme under realistic and easily verifiable conditions and subsequently demonstrate the effectiveness of the approach with a series of deconvolution experiments and comparisons with alternative strategies from the state of the art.'
date: 2023-07-01
venue: 'SIAM'
paperurl: 'http://academicpages.github.io/files/paper1.pdf'
citation: 'C. Kemajou, M. Pereyra, J.F. Giovannelli (2023). &quot;A stochastic optimisation unadjusted Langevin method for empirical Bayesian estimation in semi-blind image deblurring problems.&quot; <i>SIAM</i>.'
index: 20230701
tags:
  - paper
---
<style>
  .hiddentext {
      display: none;
      border: 2px solid #333; /* Set border width and color */
      padding: 10px;
    }
</style>
<div style="margin-left: 20px;">
    <p>
        Recommended citation: {{ post.citation }}
    </p> 
    <p> 
        <a href="http://academicpages.github.io/files/paper1.pdf" style="display:inline-block; padding:10px 20px;   margin:10px; background-color:white; color:rgb(127, 71, 127); text-decoration:none; border-radius:5px;border: 1px solid #333">PDF</a> 
        <a href="charles-kmc/charles-kmc.github.io" style="display:inline-block; padding:10px 20px; margin:10px; background-color:white; color:rgb(127, 71, 127); text-decoration:none; border-radius:5px; border: 1px solid #333">CODE</a>
        <button onclick='toggleText()' style="display:inline-block; padding:10px 20px; margin:10px; background-color:white; color:rgb(127, 71, 127); text-decoration:none; border-radius:5px;border: 1px solid #333">ABS</button>
        <div id= "index" class="hiddentext">
            This paper presents a novel stochastic optimisation methodology to perform empirical Bayesian inference in semi-blind image deconvolution problems. Given a blurred image and a parametric class of possible operators, the proposed optimisation approach automatically calibrates the parameters of the blur model by maximum marginal likelihood estimation, followed by (non-blind) image deconvolution by maximum-a-posteriori estimation conditionally to the estimated model parameters. In addition to the blur model, the proposed approach also automatically calibrates the noise variance as well as any regularisation parameters. The marginal likelihood of the blur, noise variance, and regularisation parameters is generally computationally intractable, as it requires calculating several integrals over the entire solution space. Our approach addresses this difficulty by using a stochastic approximation proximal gradient optimisation scheme, which iteratively solves such integrals by using a Moreau-Yosida regularised unadjusted Langevin Markov chain Monte Carlo algorithm. This optimisation strategy can be easily and efficiently applied to any model that is log-concave, and by using the same gradient and proximal operators that are required to compute the maximum-a-posteriori solution by convex optimisation. We provide convergence guarantees for the proposed optimisation scheme under realistic and easily verifiable conditions and subsequently demonstrate the effectiveness of the approach with a series of deconvolution experiments and comparisons with alternative strategies from the state of the art.
        </div>
    </p>
</div>

<script>
      function toggleText() {
        var textElement = document.getElementById("index");
        if (textElement.style.display === "none") {
          textElement.style.display = "inline-block";
        } else {
          textElement.style.display = "none";
        }
      }
</script>

