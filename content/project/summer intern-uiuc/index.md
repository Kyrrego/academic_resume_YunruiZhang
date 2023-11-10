---
title:  RAKI on MRSI - A deep learning approach to reconstructing high-dimensional MRSI data
summary: Proposed a novel deep learning-based method for magnetic resonance spectroscopic imaging (MRSI) reconstruction, which can achieve high-quality MRSI reconstruction from highly undersampled parallel imaging brain data.

tags:
  - Deep Learning
  - Biomedical Imaging
date: '2023-07-17T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: 'network design from: Akçakaya M, Moeller S, Weingärtner S, Uğurbil K. Scan-specific robust artificial-neural-networks for k-space interpolation (RAKI) reconstruction: Database-free deep learning for fast imaging. Magn Reson Med. 2019;81(1):439-453. doi:10.1002/mrm.27420'
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# 11/10/2023: test pdf embedding (https://github.com/anvithks/hugo-embed-pdf-shortcode)
{{< embed-pdf url="./ISMRM24_ktRAKI_final.pdf" >}}

---

Parallel imaging has been used to accelerate the slow MRSI acquisition [1]. The commonly used linear methods, such as SENSE [2] and GRAPPA [3] based methods, still produce residual aliasing of water/lipid signals which are significant enough to disrupt spatiospectral processing for metabolite reconstruction. Nonlinear k-space interpolation methods have demonstrated success in parallel MRI [4]. RAKI (Robust Artificial neural networks for k-space Interpolation) [5][6] has been designed to calibrate CNN from autocalibration signal (ACS) data which can later be employed on the whole undersampled k-space. However, RAKI has thus far been applied exclusively to MRI data. Formerly, MRSI reconstruction
has also seen the integration of neural networks [7]. Nevertheless, these approaches focused on nonlinear relationships within the k-space domain, overlooking valuable information in the temporal dimension.
In this work, we adapted and extended the self-supervised learning-based RAKI method by incorporating the FID dimension into a 3D, complex-valued convolutional network, for MRSI reconstruction. We improved the design by training a single network to handle multi-coil data simultaneously instead of the coil-by-coil interpolation in the original RAKI method. We demonstrate reduced aliasing by the proposed method and consequently improved spatiospectral processing results, using in vivo H-MRSI data.

Source code available at: https://github.com/Kyrrego/k_t_RAKI




