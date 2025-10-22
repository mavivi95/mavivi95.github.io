---
title: "Reducing overfitting in ResNet with Adaptive Lipschitz regularization"
authors:
  - Manuela Chacon-Chamorro
  - Fernando A. Gallego b 
  - J.C. Riano-Rojas
date: "2025-01-01"
publication_types: ["article-journal"]
publication: "Journal of Computational and Applied Mathematics"


tags: ["Neural Networks", "Lipschitz continuity", "Regularization", "Overfitting"]
featured: true

links:
- type: custom
  label: Site
  url: "https://doi.org/10.1016/j.cam.2025.116747"
- type: preprint
  provider: arxiv
  id: 2409.13187

image:
  preview_only: true
---

**Abstract.** This paper introduces Adaptive Lipschitz Bound Regularization with Random Constraints (LBA Regularization), a method designed to mitigate overfitting in residual neural networks by dynamically adjusting the regularization parameter based on the spectral norm of randomly selected layers. Unlike traditional regularization techniques such as L1, L2, Dropout, Early Stopping, and Batch Normalization, LBA leverages an adaptive approach that effectively constrains the Lipschitz bound while maintaining flexibility in deep learning architectures. To substantiate this method, an analysis of the Lipschitz properties in ResNet architectures was performed, offering theoretical insights into their impact on model stability and generalization. The method was evaluated in various neural architectures and datasets, including MNIST, CIFAR-10, and tabular data sets. The results demonstrate that LBA significantly reduces the gap between training and validation accuracy, leading to improved generalization performance. Furthermore, an adversarial robustness analysis against FGSM and PGD attacks confirmed that LBA maintains model stability under adversarial perturbations.