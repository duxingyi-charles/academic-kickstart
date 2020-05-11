---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Lifting Simplices to Find Injectivity"
authors: ["Xingyi Du", "Noam Aigerman", "Qingnan Zhou", "Shahar Z. Kovalsky", "Yajie Yan", "Danny M. Kaufman", "Tao Ju"]
date: 2020-05-04T17:23:54-05:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2020-05-04T17:23:54-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Graphics (Proc. SIGGRAPH 2020)"
publication_short: ""

abstract: "Mapping a source mesh into a target domain while preserving local injectivity is an important but highly non-trivial task. Existing methods either require an already-injective starting configuration, which is often not available, or rely on sophisticated solving schemes. We propose a novel energy form, called Total Lifted Content (TLC), that is equipped with theoretical properties desirable for injectivity optimization. By lifting the simplices of the mesh into a higher dimension and measuring their contents (2D area or 3D volume) there, TLC is smooth over the entire embedding space and its global minima are always injective. The energy is simple to minimize using standard gradient-based solvers. Our method achieved 100% success rate on an extensive benchmark of embedding problems for triangular and tetrahedral meshes, on which existing methods only have varied success."

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

links:
- name: PDF (Low Res)
  url: Lifting-Simplices-to-Find-Injectivity-low-res.pdf

url_pdf:
url_code: https://github.com/duxingyi-charles/lifted-nlopt
url_dataset: https://wustl.box.com/v/InjectiveMappingBenchmark
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

{{<figure alt="fig1" src="/img/TLC/fig1.png" title="Figure 1. Injectively mapping a complex surface mesh (Lucy, 48K vertices) to a non-convex boundary (letter “G”, with zoom-ins), on the left, and mapping a tetrahedral mesh (Armadillo, 6K vertices) to a highly deformed target surface, on the right, as a result of minimizing our novel energy. These two examples are part of our new benchmark data set.">}}

### **Abstract**

Mapping a source mesh into a target domain while preserving local injectivity is an important but highly non-trivial task. Existing methods either require an already-injective starting configuration, which is often not available, or rely on sophisticated solving schemes. We propose a novel energy form, called Total Lifted Content (**TLC**), that is equipped with theoretical properties desirable for injectivity optimization. By lifting the simplices of the mesh into a higher dimension and measuring their contents (2D area or 3D volume) there, TLC is smooth over the entire embedding space and its global minima are always injective. The energy is simple to minimize using standard gradient-based solvers. Our method achieved _100_% success rate on an extensive benchmark of embedding problems for triangular and tetrahedral meshes, on which existing methods only have varied success.

### **Video**

This video demonstrates the process of **TLC** optimization on a complex example. The initial mapping has _3115_ inverted triangles (colored red). Our method computes an injective mapping within _120_ iterations. 

{{<video src="lucy_G.mp4" controls="yes" >}}

### **Dataset**

We release the large benchmark dataset of 2D/3D meshes used to compare with previous methods. The dataset includes _10743_ triangular mesh examples and _904_ tetrahedral mesh examples. The dateset is divided into 3 categories, 2D parameterization, 3D parameterization and 3D deformation.

#### 2D Parameterization

{{<figure alt="2D Parameterization" src="/img/TLC/2D-Param.png" title="Figure 2. Four examples in the 2D parameterization category derived from [Liu et al. 2018], where methods FF and LBD failed to find injective embeddings. Inverted triangles are colored in red, and the numbers of inversion are marked in red.">}}

#### 3D Parameterization

{{<figure alt="3D Parameterization" src="/img/TLC/3D-Param.png" title="Figure 3. Three examples from the 3D parameterization category, each mapping a rest tetrahedral mesh into a sphere (top), smooth surface (middle), and a polycube (bottom). Each example is a failure case for one of the three methods, FF, LBD and SA. Inverted tetrahedra are colored in red, and the numbers of inversion are marked in red.">}}

#### 3D Deformation

{{<figure alt="3D Deformation" src="/img/TLC/3D-Deform.png" title="Figure 4. Three example in the 3D deformation category (a twisting armadillo) where FF, SA and LBD all failed to reach injectivity. The graph in the top-right shows the number of inverted tetrahedra for each of the 600+ frames of the deformation sequence (ellipses indicate the frames from which the three examples were taken).">}}

#### Dataset Organization

Each triangular mesh example contains
- `input.obj`: rest mesh and initial mesh (as uv coordinates)
- `handles.txt`: list of indices of the fixed vertices
- `result.obj`: result of our method

Each tetrahedral mesh example contains
- `rest.msh`: rest mesh
- `init.msh`: initial mesh
- `handles.txt`: list of indices of the fixed vertices
- `result.msh`: result of our method



[`Download Dataset`](https://wustl.box.com/v/InjectiveMappingBenchmark)
(Code and dataset will be released soon. Thanks for your patience.)



