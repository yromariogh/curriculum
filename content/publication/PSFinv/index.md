---
title: 'Learning Point Spread Function Invertibility Assessment for Image Deconvolution'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Roman Jacome
  - Sergio Urrea
  - profe
  - Luis Gonzalez

# Author notes (optional)
author_notes:
reading_time: false

date: '2024-05-25T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-05-25T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['conference-paper']

# Publication name and optional abbreviated publication name.
publication: European Signal Processing Conference 2024
publication_short: In EUPSIPCO 2024
show_breadcrumb: true
abstract: Deep-learning (DL)-based image deconvolution (ID) has exhibited remarkable recovery performance, surpassing traditional linear methods. However, unlike traditional ID approaches that rely on analytical properties of the point spread function (PSF) to achieve high recovery performance—such as specific spectrum properties or small conditional numbers in the convolution matrix—DL techniques lack quantifiable metrics for evaluating PSF suitability for DL-assisted recovery. Aiming to enhance deconvolution quality, we propose a metric that employs a non-linear approach to learn the invertibility of an arbitrary PSF using a neural network by mapping it to a unit impulse. A lower discrepancy between the mapped PSF and a unit impulse indicates a higher likelihood of successful inversion by a DL network. Our findings reveal that this metric correlates with high recovery performance in  DL and traditional methods, thereby serving as an effective regularizer in deconvolution tasks.  This approach reduces the computational complexity over conventional condition number assessments and is a differentiable process. These useful properties allow its application in designing diffractive optical elements through end-to-end (E2E) optimization, achieving invertible PSFs, and outperforming the E2E baseline framework.

# Summary. An optional shortened abstract.
summary: EUPSIPCO 2024



# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2405.16343v1'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  placement: 3
  focal_point: 'center'
  preview_only: false



# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""

---

### Results with Gaussian filters
![screen reader text](/PSFinv/results1.png "")

### Results for a Variety of PSFs
![screen reader text](/PSFinv/results2.png "")

### Results for DOE design
![screen reader text](/PSFinv/results3.png "Comparative results illustrating the impact of incorporating the proposed invertibility metric into the E2E optimization loss function for ID.")
