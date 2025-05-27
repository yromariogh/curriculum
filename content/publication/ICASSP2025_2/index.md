---
title: 'Improving Compressive Imaging Recovery via Measurement Augmentation'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - roman
  - leon
  - emmanuel
  - profe

# Author notes (optional)
reading_time: false
date: '2025-01-27T00:00:00Z'


# Schedule page publish date (NOT publication's date).
publishDate: '2024-07-05T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['conference']

# Publication name and optional abbreviated publication name.
publication: "International Conference on Acoustics, Speech, and Signal Processing"
publication_short: "ICASSP 2025"

abstract: In compressive imaging systems, the scene is acquired via linear coded noisy projections, known as measurements, requiring a recovery process to estimate the underlying signal. This recovery is inherently ill-posed, posing a challenge for accurate signal recovery. Existing methods that employ prior information about the signal often fail in practical scenarios. In this work, instead of developing a new prior over the signal, we exploit the structure of the low-dimensional measurements to synthesize an augmented measurement set that can be used in various recovery methods to improve its performance. We used a deep neural network to generate the synthetic measurements from the acquired data. We show the benefits of this approach in two schemes, deep learning-based recovery and the plug-and-play (PnP) algorithm. Particularly, our method is interpreted as a non-linear preconditioning technique for the PnP algorithm. We show improved performance for different sensing matrices.

# Summary. An optional shortened abstract.
summary: "2025 International Conference on Acoustics, Speech, and Signal Processing"



# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10888734'
# url_code: 'https://github.com/yromariogh/DNL2'
# url_dataset: ''
# url_poster: 'https://drive.google.com/file/d/1U6cVhdxNf7-2HU_67_hu58cWoxDE-fu7/view?usp=sharing'
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

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

### Simulation results

![screen reader text](/ICASSP2025_2/convergence.png "Fig. 1.   Convergence metrics for Augmented PnP-ADMM using the DCT sensing matrix with $m/n = 0.1$. The losses are normalized with respect to the ground-truth signal $x$.")

![screen reader text](/ICASSP2025_2/heatmaps.png "Fig. 2.   Measurement augmentation performance in terms of peak signal-to-noise ratio (PSNR) using a DNN for signal recovery with binary sensing matrices: (a) Hadamard and (b) Cake-Cutting ordered Hadamard; and real-valued sensing matrices: (c) DCT and (d) Gaussian. The best recovery PSNR for each $\gamma$ experiment is highlighted in bold if it surpasses the baseline in the corresponding $m/n$. Blank zones indicate $m/n + d/n > 1.0$.")

