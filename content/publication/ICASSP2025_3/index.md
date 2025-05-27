---
title: 'Compressive Imaging Reconstruction via Conditional Diffusion Model With Augmented Measurements'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - emmanuel
  - leon
  - admin
  - roman
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

abstract: Compressive imaging (CI) consists of reconstructing images from incomplete observed data. The reconstruction process involves solving an ill-posed inverse problem which is highly dependent on the number of real measurements, with a greater number of measurements typically leading to more accurate reconstructions. Due to their ability to learn data distributions, diffusion models (DM) have emerged as promising techniques for various inverse problems. Mainly, DMs solve inverse problems by conditioning the generation process to the acquired measurements. In this work, we introduce a new approach to improve this conditioning by exploiting synthetic measurements, which come from a synthetic sensing matrix. Synthetic measurements are estimated from real data via a neural network. The combined real and synthetic measurements form an augmented set, which is input into the conditional DM to enhance reconstruction capacity. Computational experiments demonstrate that augmenting measurements with the conditional DM improves performance compared to using only real measurements.

# Summary. An optional shortened abstract.
summary: "2025 International Conference on Acoustics, Speech, and Signal Processing"



# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/10889114/'
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

![screen reader text](/ICASSP2025_3/results.png "Fig. 1.   Qualitative results. Three validation samples from the MNIST dataset and their reconstructions using the zig-zag and cake-cutting Hadamard Single-Pixel Camera ordering strategies. "Baseline" denotes the conditional DM without the augmentation model. "Pseudoinverse" refers to reconstruction using $[H^\top, S^\top]^\dagger [y^\top, M_\phi^*(y)^\top]^\top$. The "Proposed" method includes both real and synthetic measurements. The green boxes show synthetic measurements with MSE and SAM evaluations.")

