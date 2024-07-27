---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Adaptive Grid Generation for Discretizing Implicit Complexes"
authors: ["Yiwen Ju", "Xingyi Du", "Qingnan Zhou", "Nathan Carr", "Tao Ju"]
date: 2024-07-27T17:23:54-05:00
doi: "10.1145/3658215"

# Schedule page publish date (NOT publication's date).
publishDate: 2024-07-19T17:23:54-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Graphics (Proc. SIGGRAPH 2024)"
publication_short: ""

abstract: "We present a method for generating a simplicial (e.g., triangular or tetrahedral) grid to enable adaptive discretization of implicit shapes defined by a vector function. Such shapes, which we call implicit complexes, are generalizations of implicit surfaces and useful for representing non-smooth and non-manifold structures. While adaptive grid generation has been extensively studied for polygonizing implicit surfaces, few methods are designed for implicit complexes. Our method can generate adaptive grids for several implicit complexes, including arrangements of implicit surfaces, CSG shapes, material interfaces, and curve networks. Importantly, our method adapts the grid to the geometry of not only the implicit surfaces but also their lower-dimensional intersections. We demonstrate how our method enables efficient and detail-preserving discretization of non-trivial implicit shapes."

# Summary. An optional shortened abstract.
summary: "An adaptive grid generation method that captures fine geometric details for implicit surfaces including their intersection curves and joint points"

tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

links:

url_pdf: https://jurwen.github.io/Adaptive-grid-for-implicit-complexes/static/pdfs/Adaptive%20grid%20generation%20for%20discretizing%20implicit%20complexes.pdf
url_code: https://github.com/Jurwen/Adaptive-grid-generation
url_dataset:
url_poster:
url_project: https://jurwen.github.io/Adaptive-grid-for-implicit-complexes/
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

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

header:
  image: ""
  placement: 
  caption: ""

---
