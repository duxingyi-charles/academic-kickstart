---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Robust Computation of Implicit Surface Networks for Piecewise Linear Functions"
authors: ["Xingyi Du", "Qingnan Zhou", "Nathan Carr", "Tao Ju"]
date: 2022-04-28T17:23:54-05:00
doi: "10.1145/3528223.3530176"

# Schedule page publish date (NOT publication's date).
publishDate: 2022-04-28T17:23:54-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Graphics (Proc. SIGGRAPH 2022)"
publication_short: ""

abstract: "Implicit surface networks, such as arrangements of implicit surfaces and materials interfaces, are used for modeling piecewise smooth or partitioned shapes. However, accurate and numerically robust algorithms for discretizing either structure on a grid are still lacking. We present a unified approach for computing both types of surface networks for piecewise linear functions defined on a tetrahedral grid. Both algorithms are guaranteed to produce a correct combinatorial structure for any number of functions. Our main contribution is an exact and efficient method for partitioning a tetrahedron using the level sets of linear functions defined by barycentric interpolation. To further improve performance, we designed look-up tables to speed up processing of tetrahedra involving few functions and introduced an efficient algorithm for identifying nested 3D regions. "

# Summary. An optional shortened abstract.
summary: "A robust method for computing implicit surface netwroks (e.g. arrangements and material interfaces) on a tetrahedron grid"

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
- name: PDF (Low Res)
  url: Optimizing-Global-Injectivity-for-Constrained-Parameterization-low-res.pdf

url_pdf:
url_code: 
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
  placement: 
  caption: ""

---

{{<figure alt="featured" src="/img/Implicit_network/fig-teaser.jpg" title="Figure 1. Implicit surface networks, such as implicit arrangement (left, obtained for primitive geometry defining a CAD object) and material interfaces (right, the Voronoi diagram of rotating 3D lines), produced by our robust algorithms. Each example is visualized by its surface patches, non-manifold curve network as well as the 3D regions partitioned by the surface network.">}}



### **Abstract**

Implicit surface networks, such as arrangements of implicit surfaces and materials interfaces, are used for modeling piecewise smooth or partitioned shapes. However, accurate and numerically robust algorithms for discretizing either structure on a grid are still lacking. We present a unified approach for computing both types of surface networks for piecewise linear functions defined on a tetrahedral grid. Both algorithms are guaranteed to produce a correct combinatorial structure for any number of functions. Our main contribution is an exact and efficient method for partitioning a tetrahedron using the level sets of linear functions defined by barycentric interpolation. To further improve performance, we designed look-up tables to speed up processing of tetrahedra involving few functions and introduced an efficient algorithm for identifying nested 3D regions. 


## **Code**

Source code will be released soon.

## **Figures**

<!-- {{<figure alt="fig-success" src="/img/SEA/fig-success.png" title="Figure 2. Three successful examples from the benchmark: initial maps (first column), maps produced by our method (second column), which are all globally injective, and maps produced by LBD (third column) and SA (last column), none of which are locally or globally injective.">}} -->


