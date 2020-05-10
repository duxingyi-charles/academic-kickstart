---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Field-Aligned Isotropic Surface Remeshing"
authors: ["Xingyi Du", "Xiaohan Liu", "Dong-Ming Yan", "Caigui Jiang", "Juntao Ye", "Hui Zhang"]
date: 2018-02-28T00:00:00-00:00
doi: "10.1111/cgf.13329"

# Schedule page publish date (NOT publication's date).
publishDate: 2020-05-09T17:23:54-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "Computer Graphics Forum (Proc. Eurographics 2018)"
publication_short: ""

abstract: "We present a novel isotropic surface remeshing algorithm that automatically aligns the mesh edges with an underlying directional field. The alignment is achieved by minimizing an energy function that combines both centroidal Voronoi tessellation and the penalty enforced by a six-way rotational symmetry (6-RoSy) field. The CVT term ensures the uniform distribution of thevertices and the high remeshing quality, while the field constraint enforces the directional alignment of the edges. Experimental results show that the proposed approach has the advantages of both isotropic remeshing and field-aligned remeshing. We demonstrate that our algorithm is superior to the representative state-of-the-art approaches in various aspects."

# Summary. An optional shortened abstract.
summary: ""

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

url_pdf:
url_code: https://github.com/duxingyi-charles/CVTRemesh
url_dataset:
url_poster:
url_project:
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
  placement: 1
  caption: ""

---


{{<figure alt="overview of algorithm" src="/img/fcvt-cylinder.png" title="Figure 1. Given a user-defined directional field (left), our method aligns the mesh edges with the field direction (middle left). The result is a high quality remeshing with less singular vertices (right).">}}