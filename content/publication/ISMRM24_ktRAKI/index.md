---
title: 'ISMRM24: A (k,t)-RAKI Method for Interpolating Sparse Data in Accelerated MRSI Acquisitions'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Ruiyang Zhao
  - Zepeng Wang

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2023-11-08T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-11-08T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: A (k,t)-RAKI Method for Interpolating Sparse Data in Accelerated MRSI Acquisitions
publication_short:  A (k,t)-RAKI Method for Interpolating Sparse Data in Accelerated MRSI Acquisitions

abstract: Parallel imaging has been used to accelerate the slow MRSI acquisition [1]. The commonly used linear methods, such as SENSE [2] and GRAPPA [3] based methods, still produce residual aliasing of water/lipid signals which are significant enough to disrupt spatiospectral processing for metabolite reconstruction. Nonlinear k-space interpolation methods have demonstrated success in parallel MRI [4]. RAKI (Robust Artificial neural networks for k‐space Interpolation) [5][6] has been designed to calibrate CNN from autocalibration signal (ACS) data which can later be employed on the whole undersampled k-space. However, RAKI has thus far been applied exclusively to MRI data. Formerly, MRSI reconstruction has also seen the integration of neural networks [7]. Nevertheless, these approaches focused on nonlinear relationships within the k-space domain, overlooking valuable information in the temporal dimension.

In this work, we adapted and extended the self-supervised learning-based RAKI method by incorporating the FID dimension into a 3D, complex-valued convolutional network, for MRSI reconstruction. We improved the design by training a single network to handle multi-coil data simultaneously instead of the coil-by-coil interpolation in the original RAKI method. We demonstrate reduced aliasing by the proposed method and consequently improved spatiospectral processing results, using in vivo 1H-MRSI data. 


# Summary. An optional shortened abstract.
summary: In this work, we proposed a self-supervised learning-based (k,t)-space interpolation method, (k,t)-RAKI, that is useful for further accelerating MRSI acquisition, in combination with subspace methods.

tags: [Biomedical Imaging, MR Spectroscopy Reconstruction, Deep Learning]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
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
  caption: ''
  focal_point: ''
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - summer intern-uiuc

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/).
