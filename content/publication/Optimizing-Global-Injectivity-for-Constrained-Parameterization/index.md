---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Optimizing Global Injectivity for Constrained Parameterization"
authors: ["Xingyi Du", "Danny M. Kaufman", "Qingnan Zhou", "Shahar Z. Kovalsky", "Yajie Yan", "Noam Aigerman", "Tao Ju"]
date: 2021-09-18T17:23:54-05:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-09-18T17:23:54-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Graphics (Proc. SIGGRAPH Asia 2021)"
publication_short: ""

abstract: "Injective parameterizations of triangulated meshes are critical across applications but remain challenging to compute. Existing algorithms to find injectivity either require initialization from an injective starting state, which is currently only possible without positional constraints, or else can only prevent triangle inversion, which is insufficient to ensure injectivity. Here we present, to our knowledge, the first algorithm for recovering a globally injective parameterization from an arbitrary non-injective initial mesh subject to stationary constraints. These initial meshes can be inverted, wound about interior vertices and/or overlapping. Our algorithm in turn enables globally injective mapping for meshes with arbitrary positional constraints. Our key contribution is a new energy, called smooth excess area (SEA), that measures non-injectivity in a map. This energy is well-defined across both injective and non-injective maps and is smooth almost everywhere, making it readily minimizable using standard gradient-based solvers starting from a non-injective initial state. Importantly, we show that maps minimizing SEA are guaranteed to be locally injective and almost globally injective, in the sense that the overlapping area can be made arbitrarily small. Analyzing SEA’s behavior over a new benchmark set designed to test injective mapping, we find that optimizing SEA successfully recovers globally injective maps for 85% of the benchmark and obtains locally injective maps for 90%. In contrast, state-of-the-art methods for removing triangle inversion obtain locally injective maps for less than 6% of the benchmark, and achieve global injectivity (largely by chance as prior methods are not designed to recover it) on less than 4%."

# Summary. An optional shortened abstract.
summary: "A method for globally injectively mapping a triangle mesh to plane while satisfying positional constraints"

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
url_dataset: https://doi.org/10.5281/zenodo.5547887
url_poster:
url_project:
url_slides:
url_source:
url_video: https://youtu.be/XvewOf-U7Gw

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

{{<figure alt="featured" src="/img/SEA/fig1.jpeg" title="Figure 1. Given a non-injective initial parameterization of a surface mesh (left) with inverted triangles (red), boundary intersections (orange dots), and overwound vertices (magenta dots), our method recovers a globally injective map (right) while keeping the constraints (blue points) in place. The inserts zoom in on one region in the initial map with many boundary intersections and inverted triangles (green box) and another region with an overwound vertex (cyan box).">}}



### **Abstract**

Injective parameterizations of triangulated meshes are critical across applications but remain challenging to compute. Existing algorithms to find injectivity either require initialization from an injective starting state, which is currently only possible without positional constraints, or else can only prevent triangle inversion, which is insufficient to ensure injectivity. Here we present, to our knowledge, the first algorithm for recovering a globally injective parameterization from an arbitrary non-injective initial mesh subject to stationary constraints. These initial meshes can be inverted, wound about interior vertices and/or overlapping. Our algorithm in turn enables globally injective mapping for meshes with arbitrary positional constraints. Our key contribution is a new energy, called smooth excess area (SEA), that measures non-injectivity in a map. This energy is well-defined across both injective and non-injective maps and is smooth almost everywhere, making it readily minimizable using standard gradient-based solvers starting from a non-injective initial state. Importantly, we show that maps minimizing SEA are guaranteed to be locally injective and almost globally injective, in the sense that the overlapping area can be made arbitrarily small. Analyzing SEA’s behavior over a new benchmark set designed to test injective mapping, we find that optimizing SEA successfully recovers globally injective maps for 85% of the benchmark and obtains locally injective maps for 90%. In contrast, state-of-the-art methods for removing triangle inversion obtain locally injective maps for less than 6% of the benchmark, and achieve global injectivity (largely by chance as prior methods are not designed to recover it) on less than 4%.

## **Video** 

### **Fast Forward**

{{< youtube XvewOf-U7Gw >}}

### **Optimization Process**

The process of optimizing SEA (smooth excess area) on the examples presented in the paper.

{{< youtube JXtlrBec4Rs >}}

## **Dataset**

We create a benchmark dataset for evaluating various methods' capability to recover an injective mapping from a non-injective initial mapping while keeping a group of positional constraints in place.

The dataset includes 1791 triangular mesh examples. Each example contains
- `input.obj`: rest mesh and initial mesh (as UV coordinates)
- `handles.txt`: list of indices of the fixed vertices
- `groundTruth.obj`: globally injective mesh satisfying positional constraints

We also provide the result of our method for each example.

[`Download Dataset`](https://doi.org/10.5281/zenodo.5547887)

## **Code**

Code will be released soon.


## **Figures**

{{<figure alt="fig-success" src="/img/SEA/fig-success.png" title="Figure 2. Three successful examples from the benchmark: initial maps (first column), maps produced by our method (second column), which are all globally injective, and maps produced by LBD (third column) and SA (last column), none of which are locally or globally injective.">}}

{{<figure alt="fig-toys" src="/img/SEA/fig-toys.png" title="Figure 3. From left to right: input meshes (with one or two boundaries), non-injective initial maps, globally injective maps produced by our method (SEA), and results of LBD and SA. Both LBD and SA have removed most or all inverted triangles, but the results are neither locally or globally injective due to overwound vertices and boundary intersections.">}}

{{<figure alt="fig-overwound-1-rings" src="/img/SEA/fig-overwound-1-rings.png" title="Figure 4. Two initial maps with overwound vertices (top) and the injective maps produced by our method (bottom).">}}





<!-- ### **Acknowledgments**

This work is supported in part by NSF grant RI-1618685, NIH grant U2C CA233303-1, and Simons Math+X Investigators Award 400837. We would like to thank authors of several papers for providing code, data, and help with comparisons, and especially Hanxiao Shen, Ofir Weber, Alon Bright, Zohar Levi, and Xiao-Ming Fu. -->
