---
title: 'NPN: Non-Linear Projections of the Null-Space for Imaging Inverse Problems'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - roman
  - admin
  - leon
  - profe

# Author notes (optional)
reading_time: false
date: '2025-12-01'
doi: '10.48550/arXiv.2510.01608'

# Schedule page publish date (NOT publication's date).
publishDate: '2025-12-01'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['conference']

# Publication name and optional abbreviated publication name.
publication: "Neural Information Processing Systems 2025"
publication_short: "Neurips 2025"

abstract: Imaging inverse problems aim to recover high-dimensional signals from undersampled, noisy measurements, a fundamentally ill-posed task with infinite solutions in the null-space of the sensing operator. To resolve this ambiguity, prior information is typically incorporated through handcrafted regularizers or learned models that constrain the solution space. However, these priors typically ignore the task-specific structure of that null-space. In this work, we propose \textit{Non-Linear Projections of the Null-Space} (NPN), a novel class of regularization that, instead of enforcing structural constraints in the image domain, promotes solutions that lie in a low-dimensional projection of the sensing matrix’s null-space with a neural network. Our approach has two key advantages. (1) Interpretability. by focusing on the structure of the null-space, we design sensing-matrix-specific priors that capture information orthogonal to the signal components that are fundamentally blind to the sensing process. (2) Flexibility. NPN is adaptable to various inverse problems, compatible with existing reconstruction frameworks, and complementary to conventional image-domain priors. We provide theoretical guarantees on convergence and reconstruction accuracy when used within plug-and-play methods. Empirical results across diverse sensing matrices demonstrate that NPN priors consistently enhance reconstruction fidelity in various imaging inverse problems, such as compressive sensing, deblurring, super-resolution, computed tomography, and magnetic resonance imaging, with plug-and-play methods, unrolling networks, deep image prior, and diffusion models. 

# Summary. An optional shortened abstract.
summary: "Neural Information Processing Systems 2025"



# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2510.01608'
url_code: 'https://github.com/yromariogh/NPN'
# url_dataset: ''
url_poster: 'https://drive.google.com/file/d/16RnQku3sUIMAqnIYE2HcFrsB2e2M-gSD/view?usp=sharing'
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []
show_breadcrumb: true

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

### NPN: Non-Linear Projections of the Null-Space for High-Fidelity Imaging 
Inverse imaging problems—such as **deblurring, denoising, and compressive sensing** (CS)—are notoriously challenging because they rely on reconstructing a single high-quality image from incomplete or corrupted measurements. This fundamental ambiguity is encapsulated in the null-space of the measurement process.
Our paper, NPN (Non-Linear Projections of the Null-Space), introduces a novel deep learning framework to explicitly address this ambiguity, leading to state-of-the-art reconstruction quality across various tasks.

### Solving Ambiguity with the Null-Space
Traditional image reconstruction methods, such as Plug-and-Play (PnP) and diffusion models, typically enforce image priors directly in the signal domain, limiting their ability to fully resolve the ambiguities introduced by the measurement matrix (especially in low-sampling scenarios like compressive sensing).
The NPN framework overcomes this by introducing a new component: a non-linear projection operator (S) that focuses specifically on mapping information within the null-space.
By explicitly modeling the ambiguity and projecting it into a meaningful, learned subspace, NPN successfully:
- Decomposes the image space into the signal range (data fidelity) and the null-space (ambiguity).
- Learns a powerful non-linear projector (S) that effectively filters out unwanted null-space components, dramatically improving reconstruction quality.
This approach significantly enhances the performance of existing denoisers and diffusion-based image priors, pushing the boundaries of what is possible in various imaging applications. We demonstrate superior reconstruction fidelity for problems including image deblurring, denoising, and compressive sensing.

![screen reader text](/Neurips2025/featured.png "**Figure 1: Conceptual Overview of NPN**. The proposed Non-Linear Projections of the Null-Space (NPN) framework, explicitly modeling the null-space ambiguity to enable higher fidelity image reconstruction.")

![screen reader text](/Neurips2025/DIFF_REC-1.png "**Figure 2: Qualitative Results for Image Reconstruction.** A comparison of NPN's performance (right) against state-of-the-art techniques for a challenging imaging inverse problem (e.g., low-rate compressive sensing), showing superior detail preservation and artifact suppression.")