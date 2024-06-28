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
url_dataset: ''
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

### Proposed algorithm
![screen reader text](/TCI2024/ALGORITHM.png "")

### Simulation results

![screen reader text](/TCI2024/Ys_by_deg_level_white+Mx.png "Fig. 3.   Simulated measurement $\mathbf{y}_i$ for each degradation level $D_i$. (b) Absolute error of each simulated measurement with respect to the non-degradation scenario $\mathbf{y}_0=\mathbf{Hx}$. (c) Improved measurement obtained with the $\text{DNL}^2$ model. (d) Absolute error of each simulated measurement with respect to the improved measurement. The evident reduction in error across degradation levels underscores its robustness and independence.")

![screen reader text](/TCI2024/ARAD_METRICS_NL+SNR.png "Fig. 4.   (a) Simulation results and ablation studies of $\lambda_1$ under each degradation level in the ARAD dataset. Note the improvement in the different metrics by increasing the proposed regularizer influence through the coefficient $\lambda_1$, with $\lambda_1=0$ as the baseline PnP with the linear propagation model. (b) Average results of different testing images evaluating the impact of additional noise at the highest degradation level $D_4$ from the ARAD dataset.")

![screen reader text](/TCI2024/TABLE_IV.png ".")

### Hardware experiments

![screen reader text](/TCI2024/PSNRvsPSNR+Convergence+Split_Results.png "Fig. 5.   (a) Average PSNR of the estimated measurements with $\text{DNL}^2$ model through iterations. (b) Comparison between the $\text{DNL}^2$ measurement performance and reconstruction quality using $\lambda=1$. (c) Convergence of the $\text{DNL}^2$ recovery loss. (d-f) Reconstruction quality with real data and ablation studies of the proposed regularizer influence, $\lambda_1$. The quality of the reconstructions shows a significant improvement, with an increase of nearly 3 dB in PSNR compared to the simple propagation model (i.e., $\lambda_1=0$).")

![screen reader text](/TCI2024/4x6-LABands.png "Fig. 6.   Some recovered spectral bands for an acquired testing spectral image. Note the visual and metric improvement in the false RGB representation and across the spectral bands using the $\text{DNL}^2$ model, i.e., $\lambda_1=1$.")

![screen reader text](/TCI2024/X_and_morePSfs.png "Fig. 7.   The input of the $\text{DNL}^2$ model is the spectral image in (a) resulting in a set of spatio-spectrally variant PSFs within the domain of the compressed measurements, which are spectrally plotted in (b) and two of them are zoomed in (d). The linear propagation model PSF is shown in (c).")

### State-of-the-art comparison

![screen reader text](/TCI2024/TABLE_VI.png ".")

![screen reader text](/TCI2024/LAB.png "Fig. 8.   Experimental reconstructions comparison as false RGB and corresponding signatures between Song et al.'s [22] and DNL² propagation model. Note the visual and quantitative improvement for the three testing images and in the corresponding spectral signatures at points A, B, and C.")


### Supplementary material

![screen reader text](/TCI2024/Sup_ALGORITHM.png ".")

![screen reader text](/TCI2024/METRICS_PRIOR.png "Fig. 1. Results and ablation studies of $\lambda_1$ using a Fixed~\cite{dabov2007image} and Learned prior~\cite{zhang2021plug} with experimental data.")

![screen reader text](/TCI2024/LAB_PRIOR.png "Fig. 2. Experimental reconstructions comparison as false RGB and corresponding signatures between Song et al.'s~\cite{song2022high} and $\text{DNL}^2$ propagation model with a fixed \cite{dabov2007image} or learned prior \cite{zhang2021plug}.")

![screen reader text](/TCI2024/Table_Sup1.png "")


