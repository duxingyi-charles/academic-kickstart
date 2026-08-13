---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "DreamUV: Unwrap Artist-like UV by End-to-End Flow Matching"
authors: ["Quanyuan Ruan", "Jiabao Lei", "Xingyi Du", "Xifeng Gao"]
date: 2026-06-21T00:00:00-07:00
doi: "10.48550/arXiv.2606.22445"

# Schedule page publish date (NOT publication's date).
publishDate: 2026-06-21T00:00:00-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types:

# Publication name and optional abbreviated publication name.
publication: "arXiv preprint arXiv:2606.22445, 2026"
publication_short: ""

abstract: "UV parameterization is a fundamental step in 3D content creation, yet producing production-ready UV layouts remains challenging due to the gap between geometric distortion objectives and the stylistic preferences of professional artists. While classical methods optimize handcrafted energy functions, artist-authored UVs exhibit structural patterns such as straightened seams, axis-aligned islands, and flexible interior deformation, properties that are difficult to explicitly formulate. We present DreamUV, an end-to-end learning framework that formulates UV unwrapping as a generative Flow Matching problem. Rather than predicting a single optimal parameterization, DreamUV learns a mesh-conditioned transport process that maps noise samples to a distribution of artist-like UV layouts. A boundary-aware training strategy prioritizes seam geometry, while Model-in-the-Loop Finetuning explicitly accounts for discretization errors during sampling and stabilizes transport dynamics under heterogeneous supervision. Experiments demonstrate significantly straighter boundaries and tighter axis-aligned islands than classical and learning-based baselines while maintaining competitive distortion metrics."

# Summary. An optional shortened abstract.
summary: "An end-to-end Flow Matching framework for generating artist-like UV layouts from meshes"

tags: []
categories: []
featured: false

links:

url_pdf: https://arxiv.org/pdf/2606.22445
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source: https://arxiv.org/abs/2606.22445
url_video:

# Featured image
image:
  caption: ""
  focal_point: ""
  preview_only: true

projects: []
slides: ""

header:
  image: ""
  placement:
  caption: ""

---
