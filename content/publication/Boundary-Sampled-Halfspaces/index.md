---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Boundary-Sampled Halfspaces: A New Representation for Constructive Solid Modeling"
authors: ["Xingyi Du", "Qingnan Zhou", "Nathan Carr", "Tao Ju"]
date: 2021-05-21T17:23:54-05:00
doi: "10.1145/3450626.3459870"

# Schedule page publish date (NOT publication's date).
publishDate: 2021-05-21T17:23:54-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Graphics (Proc. SIGGRAPH 2021)"
publication_short: ""

abstract: "We present a novel representation of solid models for shape design. Like Constructive Solid Geometry (CSG), the solid shape is constructed from a set of halfspaces without the need for an explicit boundary structure. Instead of using Boolean expressions as in CSG, the shape is defined by sparsely placed samples on the boundary of each halfspace. This representation, called Boundary-Sampled Halfspaces (BSH), affords greater agility and expressiveness than CSG while simplifying the reverse engineering process. We discuss theoretical properties of the representation and present practical algorithms for boundary extraction and conversion from other representations. Our algorithms are demonstrated on both 2D and 3D examples."

# Summary. An optional shortened abstract.
summary: "A novel representation for solid models to facilitate intuitive shape design and straightforward reverse engineering"

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
  url: Boundary-Sampled-Halfspaces-low-res.pdf

url_pdf:
url_code: https://github.com/duxingyi-charles/Boundary_Sampled_Halfspaces
url_dataset:
url_poster:
url_project:
url_slides: "BSH_Slides.pdf"
url_source:
url_video: https://youtu.be/rCKh39pEdrg

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

{{<figure alt="featured" src="/img/BSH/fig1.png" title="Figure 1. A segmented shape (a) is converted into our representation (b), which consists of halfspaces associated with sparse samples (colored spheres). Each halfspace is either a simple primitive (e.g., plane, sphere, etc.) or a free-form implicit surface (one is shown in transparency). The representation can be easily edited by modifying the halfspaces and/or their samples (c).">}}



### **Abstract**

We present a novel representation of solid models for shape design. Like Constructive Solid Geometry (CSG), the solid shape is constructed from a set of halfspaces without the need for an explicit boundary structure. Instead of using Boolean expressions as in CSG, the shape is defined by sparsely placed samples on the boundary of each halfspace. This representation, called Boundary-Sampled Halfspaces (BSH), affords greater agility and expressiveness than CSG while simplifying the reverse engineering process. We discuss theoretical properties of the representation and present practical algorithms for boundary extraction and conversion from other representations. Our algorithms are demonstrated on both 2D and 3D examples.

### **Video**

#### Fast Forward

{{< youtube ujd4t9skJ_Y >}}

#### Quick Summary

{{< youtube rCKh39pEdrg >}}

#### Full Presentation

{{< youtube -lKQAQhfX3I >}}

#### Software Demo

We demonstrate the modeling process of various examples using Boundary-Sampled Halfspaces.

{{< youtube BRO36bIMXxI >}}




## **2D Shape Design**

{{<figure alt="fig-gallery-2D" src="/img/BSH/fig-gallery-2D.png" title="Figure 2. Several 2D shapes modeled by BSH. Halfspaces for the last two shapes are not shown due to their complexity.">}}

## **3D Shape Design**

{{<figure alt="fig-beads" src="/img/BSH/fig-beads.png" title="Figure 3. Various BSH shapes created from one torus and several spheres. By choosing which segment of the torus has a sample, different segments can be kept or deleted while the shape remains a solid.">}}

{{<figure alt="fig-gallery-3D" src="/img/BSH/fig-gallery-3D.png" title="Figure 4. Shape modeled by BSH that cannot be represented by CSG without additional halfspaces. For the first two shapes, input halfspaces are on the left and the final shapes are on the right. The last shape (“Heart”) is shown in two views, and the second view shows a halfspace represented as a VIPSS implicit surface interpolating a sparse set of control points (red spheres).">}}

## **Converted from other representations**

{{<figure alt="fig-gallery-reverse" src="/img/BSH/fig-gallery-reverse.png" title="Figure 5. Free-form BSH shapes (Elk, Flower, Boat, and Chair) converted from meshes and undergone editing of the halfspaces and/or their samples. Top: each row shows the input segmented mesh, the converted BSH, and result after editing. Selected halfspaces before and after editing are shown with transparency. Bottom: each row shows the converted BSH and two editing results.">}}


{{<figure alt="fig-cad" src="/img/BSH/fig-cad.png" title="Figure 6. A CAD mesh segmented and fitted by primitives (a; showing two views), the converted BSH shape (b; showing two views), and two edited shapes with altered structure (e.g., fewer rings and a missing shelf) (c) and modified primitive geometry (d).">}}



<!-- ### **Acknowledgments**

This work is supported in part by NSF grant RI-1618685, NIH grant U2C CA233303-1, and Simons Math+X Investigators Award 400837. We would like to thank authors of several papers for providing code, data, and help with comparisons, and especially Hanxiao Shen, Ofir Weber, Alon Bright, Zohar Levi, and Xiao-Ming Fu. -->
