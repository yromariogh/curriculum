---
title: 'Deep Learned Non-Linear Propagation Model Regularizer for Compressive Spectral Imaging'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - bacca
  - profe

# Author notes (optional)
reading_time: false
date: '2024-06-24T00:00:00Z'
doi: '10.1364/COSI.2023.CTh3B.2'

# Schedule page publish date (NOT publication's date).
publishDate: '2024-06-24T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['journal']

# Publication name and optional abbreviated publication name.
publication: "IEEE Transactions on Computational Imaging"
publication_short: "TCI 2024"

abstract: Coded aperture snapshot spectral imager (CASSI), efficiently captures 3D spectral images by sensing 2D projections of the scene. While CASSI offers a substantial reduction in acquisition time, compared to traditional scanning optical systems, it requires a reconstruction post-processing step. Furthermore, to obtain high-quality reconstructions, an accurate propagation model is required. Notably, CASSI exhibits a variant spatio-spectral sensor response, making it difficult to acquire an accurate propagation model. To address these inherent limitations, this work proposes to learn a deep non-linear fully differentiable propagation model that can be used as a regularizer within an optimization-based reconstruction algorithm. The proposed approach trains the non-linear spatially-variant propagation model using paired compressed measurements and spectral images, by employing side information only in the calibration step. From the deep propagation model incorporation into a plug-and-play alternating direction method of multipliers framework, our proposed method outperforms traditional CASSI linear-based models. Extensive simulations and a testbed implementation validate the efficacy of the proposed methodology. 

# Summary. An optional shortened abstract.
summary: "IEEE Transactions on Computational Imaging"



# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://opg.optica.org/abstract.cfm?uri=COSI-2023-CTh3B.2'
url_code: 'https://github.com/yromariogh/DNL2'
url_dataset: 'https://github.com/hdspgroup/datasets'
url_poster: 'https://drive.google.com/file/d/1U6cVhdxNf7-2HU_67_hu58cWoxDE-fu7/view?usp=sharing'
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
projects: [calibration]
show_breadcrumb: true

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

### Quantitative results
![screen reader text](/TCI2024/LAB.png "Influence of the proposed regularizer in the reconstructions' quality")


