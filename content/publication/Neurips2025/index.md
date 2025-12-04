---
title: 'NPN: Non-Linear Projections of the Null-Space for Imaging Inverse Problems'
authors:
  - roman
  - admin
  - leon
  - profe
reading_time: false
date: '2025-12-01'
doi: '10.48550/arXiv.2510.01608'
publishDate: '2025-12-01'
publication_types: ['conference']
publication: "Neural Information Processing Systems 2025"
publication_short: "Neurips 2025"
abstract: Imaging inverse problems aim to recover high-dimensional signals from undersampled, noisy measurements, a fundamentally ill-posed task with infinite solutions in the null-space of the sensing operator. To resolve this ambiguity, prior information is typically incorporated through handcrafted regularizers or learned models that constrain the solution space. However, these priors typically ignore the task-specific structure of that null-space. In this work, we propose Non-Linear Projections of the Null-Space (NPN), a regularization that promotes solutions lying in a learned, low-dimensional projection of the sensing matrix’s null-space. This yields interpretable, operator-aware priors and complements existing reconstruction frameworks. Empirically, NPN improves reconstruction fidelity across compressive sensing, deblurring, super-resolution, CT, and MRI with plug-and-play methods, unrolling networks, deep image prior, and diffusion models.
summary: "Null-space–aware prior that plugs into PnP, unrolling, DIP, and diffusion solvers to boost reconstructions across CS, MRI, CT, and deblurring."
featured: true
url_pdf: 'https://openreview.net/pdf?id=G67ZNmeWJ5'
url_code: 'https://github.com/yromariogh/NPN'
url_poster: 'https://drive.google.com/file/d/16RnQku3sUIMAqnIYE2HcFrsB2e2M-gSD/view?usp=sharing'
projects: []
show_breadcrumb: true
slides: ""
---

## Key idea
Learn a low-dimensional projection matrix S whose rows lie in Null(H), and train a network G(y) to predict Sx. Enforce consistency during reconstruction.
![](/Neurips2025/method1.png)

## Why NPN? 
Adds model-aware, p-dimensional structure in Null(H); complementary to image-domain priors and integrates into PnP, Unrolling, DIP, and DMs.
![](/Neurips2025/method2.png "Figure 1: Geometric comparison of subspace–prior learning.")

## Results
- Faster Plug-and-Play convergence across noise levels and acceleration factors.
- Higher PSNR/SSIM for CS, MRI, Super-Resolution, CT, and Deblurring; complementary to Diffusion solvers (DPS, DiffPIR).
- Robust to projection dimension choices and sampling strategies.

![](/Neurips2025/figure2.png "Figure 2: PnP-FISTA convergence analysis in CS.")
![](/Neurips2025/figure3.png "Figure 3: Convergence for σ ∈ {2,5,10} and AF ∈ {4,8,12}.")
![](/Neurips2025/figure4.png "Figure 4: Deblurring and MRI results for PnP and PnP-NPN.")
![](/Neurips2025/figure5.png "Figure 5: Effect of p/n and S design.")
![](/Neurips2025/figure6.png "Figure 6: DIP in Deblurring.")

![](/Neurips2025/table11.png "Table 1: Dataset generalization. Each S, G, and Unrolling were optimized with CIFAR-10, and tested with the CIFAR-10 and STL10.")
![](/Neurips2025/table22.png "Table 2: Comparison of metrics under different sampling strategies.")
![](/Neurips2025/table33.png "Table 3: State-of-the-art comparison for CS, MRI, and Deblurring.")
![](/Neurips2025/table44.png "Table 4: γ-ablation for DPS and DiffPIR.")