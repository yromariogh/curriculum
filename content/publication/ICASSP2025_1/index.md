---
title: 'Learning to Reconstruct Signals With Inexact Sensing Operator via Knowledge Distillation'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - roman
  - leon
  - admin
  - luis_gonzalez
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

abstract: In computational optical imaging and wireless communications, signals are acquired through linear coded and noisy projections, which are recovered through computational algorithms. Deep model-based approaches, i.e., neural networks incorporating the sensing operators, are the state-of-the-art for signal recovery. However, these methods require exact knowledge of the sensing operator, which is often unavailable in practice, leading to performance degradation. Consequently, we propose a new recovery paradigm based on knowledge distillation. A teacher model, trained with full or almost exact knowledge of a synthetic sensing operator, guides a student model with an inexact real sensing operator. The teacher is interpreted as a relaxation of the student since it solves a problem with fewer constraints, which can guide the student to achieve higher performance. We demonstrate the improvement of signal reconstruction in computational optical imaging for single-pixel imaging with miscalibrated coded apertures systems and multiple-input multiple-output symbols detection with inexact channel matrix.

# Summary. An optional shortened abstract.
summary: "2025 International Conference on Acoustics, Speech, and Signal Processing"



# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10887652'
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

![screen reader text](/ICASSP2025_1/fig3.png "Fig. 3.   Recovery performance in the SPC system. (a) Quantitative results for different values of $\sigma_t$ and $\sigma$. (b) Visual reconstruction for the best-performing configuration of the method and the baseline.")

![screen reader text](/ICASSP2025_1/fig4.png "Fig. 4.   Detection performance in MIMO systems for different values of the proposed method $\sigma_t$ and $\sigma$ and varying the SNR.")

