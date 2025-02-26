---
layout: post
title: Machine learning resources
date: 2025-02-06 17:39:00
description:
# tags: formatting math
# categories: generative-models
# related_posts: false
---

<h3> Introduction </h3>
In this post, I will work you through some technical tools to effectively prepare a succesful Machine learning interview role!

<h3> Computer Vison </h3>
Challenges in computer vison

- **Domain shifts**: Domain shifts occur when there is a discrepancy between the statistical distribution of data in the training environment (source domain) and the real-world deployment setting (target domain). This mismatch can arise due to variations in factors such as lighting conditions, sensor noise, data collection methods, or demographic differences. As a result, models trained on the source domain may struggle to generalize effectively to the target domain, leading to degraded performance.

- **Inbalance data**: Imbalanced data occur when some classes have significantly fewer samples compared to others, Leading to bias model performance. Specifically, machine learning models tend to focus on the majority calss, as it dominates the training data while under representing or misclassifying the minority class. This problem can severely impact model generalisation, prcticulary in application such as anomaly detection and medical diagnosis.

<h2>Definitions</h2>

- **Overfitting**: Overfitting occurs when a model is too complex and fits the training. This means that the model performs very well of training data but poorly on unseen data because it has learned specific patterns that do not generalise to new data. 
- **Underfitting**: Underfitting occurs when a model is too simple and fails to capture important paterns. 

- **Bias**: In machine learning in general, bias refers to a systematic error introduced during the modelling process, which significantly affects the model's ability to generalise well on unseen data. bias can takes different meanings:
    * **Model bias**: In the context of machine learning models, bias referes to the error introduced by approximating a real-world problem by a simplified model. A model with high bias makes strong assumptions about data and may fail to capture important patterns, leading to overfitting. 
    * **Data bias**: Bias can also occur if the training data is not representative of the real-world situation. This can leads to baised oucomes for certains groups. 
    * **Bias as parameter**:  In deep learning, bias is often used as an additional parameter in neurons. This allows the neural network to shift the output up or down and helps the model learn more complex patterns. 

- **Variance**: Variance referes to how much the model's predictions change when trained on different subsets of data. 
    * **High variance**: High variance often occurs when a the model is too complex relative to the amunt of training data available. A model with high variance will fit well the training data, but when exposed to new, unseen data, it may perform poorly because it has memorised rather that generalised patterns.
    * **Low variance**. A models with low variance doesn't change much when trained on different subsets of data. It tends the make stable prdictions, bay may struggle to capture complex patterns, leading to underfitting.
- **Bias-Variance tradeoff**. This is a fundamental concept in machine learning when we try to balance two competing factors: *bais* and *variance*. 
    * **Low bias, high variance**. The model is complex and can captures many details, including noise, leading to overfitting. The prediction can 


- **Regularization**: Regularization is a technique used to prevent overfitting by adding a penalty
- **Hyperparameter tuning**: Hyperparameter tuning is the process of selecting the best
- **Cross-validation**: Cross-validation is a technique used to evaluate a model's performance
- **Resampling**: Resampling is a technique used to create multiple versions of a dataset
- **Ensemble methods**: Ensemble methods are a technique used to combine the predictions
- **Gradient boosting**: Gradient boosting is a type of ensemble method that combines
- **Random forest**: Random forest is a type of ensemble method that combines
- **Support vector machines**: Support vector machines are a type of supervised learning
- **K-nearest neighbors**: K-nearest neighbors is a type of supervised learning
- **Decision trees**: Decision trees are a type of supervised learning
- **Neural networks**: Neural networks are a type of supervised learning
- **Reinforcement learning**: Reinforcement learning is a type of unsupervised learning
- **Unsupervised learning**: Unsupervised learning is a type of learning where the model
- **Supervised learning**: Supervised learning is a type of learning where the model
- **Semi-supervised learning**: Semi-supervised learning is a type of learning where the model
- **Active learning**: Active learning is a type of learning where the model
- **Transfer learning**: Transfer learning is a type of learning where a model
- **Deep learning**: Deep learning is a type of machine learning that uses
- **Natural language processing**: Natural language processing is a type of machine learning
- **Computer vision**: Computer vision is a type of machine learning that deals
- **Vision Transformer**: 


<!--
<h3> Computer Vison </h3>
Challenges in computer vison

- **Domain shifts**:Domain shifts occur when there is a discrepancy between the statistical distribution of data in the training environment (source domain) and the real-world deployment setting (target domain). This mismatch can arise due to variations in factors such as lighting conditions, sensor noise, data collection methods, or demographic differences. As a result, models trained on the source domain may struggle to generalize effectively to the target domain, leading to degraded performance. Addressing domain shifts often involves techniques such as domain adaptation, domain generalization, or self-supervised learning to enhance model robustness across different environments.
- **Inbalance data**: Imbalanced data occur when some classes have significantly fewer samples compared to others, Leading to bias model performance. Specifically, machine learning models tend to focus on the majority calss, as it dominates the training data while under representing or misclassifying the minority class. This problem can severely impact model generalisation, prcticulary in application such as anomaly detection and medical diagnosis.  

$$
\begin{equation}\label{eq: test}
\sum_{k=1}^\infty |\langle x, e_k \rangle|^2 \leq \|x\|^2
\end{equation}
$$ -->

<!-- **Pixel-wise classification**:
**Instant classification**:
**edge detection**:
**Convolution**:
**Activation function**:
**ResNet**:
**VGG**:
**Skip-connection**:
**Vision transformer**:

--- -->
