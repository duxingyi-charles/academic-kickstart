---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Isometric Energies for Recovering Injectivity in Constrained Mapping"
authors: ["Xingyi Du", "Danny M. Kaufman", "Qingnan Zhou", "Shahar Z. Kovalsky", "Yajie Yan", "Noam Aigerman", "Tao Ju"]
date: 2022-10-09T17:23:54-06:00
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: 2022-10-09T17:23:54-06:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: 

# Publication name and optional abbreviated publication name.
publication: "SIGGRAPH Conference Proceedings (Proc. SIGGRAPH Asia 2022)"
publication_short: ""

abstract: "Computing injective maps with low distortions is a long-standing problem in computer graphics. Such maps are particularly challenging to obtain in the presence of positional constraints, because an injective initial map is often not available. Recently, several energies were proposed and shown to be highly successful in optimizing injectivity from non-injective initial maps while satisfying positional constraints. However, minimizing these energies tends to produce elements with significant isometric distortions. This paper presents simple variants of these energies that retain their desirable traits while promoting isometry. While our method is not guaranteed to provide an injective map, we observe that, on large-scale 2D and 3D data sets, minimizing the proposed isometric variants results in a similar level of success in recovering injectivity as the original energies but a significantly lower isometric distortion."

# Summary. An optional shortened abstract.
summary: "A method for computing injective and low-distortion maps with positional constraints"

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
  url: Isometric-Energies-for-Recovering-Injectivity-in-Constrained-Mapping-low-res.pdf

url_pdf:
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video: https://youtu.be/6Utp5YR28Mg

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

{{<figure alt="featured" src="/img/Iso_TLC_SEA/teaser.png" title="Figure 1. When used to parameterize meshes into the 2D plane, our isometric variants of injectivity energies empirically tend to yield injective results with low isometric distortion. Left: an initial map of Lucy into letter S, which contains many inverted triangles (red), is optimized while holding its boundary fixed, using the TLC energy [Du et al. 2020], the Fold-Free Mapping (FFM) method of [Garanzha et al. 2021], and our energy - IsoTLC. Right: an initial map, which contains inverted triangles (red), overwinding vertices (purple) and global overlaps (boxed), is optimized while fixing only a set of sparse positional constraints (blue) without constraining the boundary, by minimizing either the SEA energy of [Du et al. 2020] or our energy, IsoSEA. In both cases, our method leads to the injective map with the lowest isometric distortion (max(𝜎1, 1/𝜎2)) of the triangles, as shown by the histograms and the color map on the mesh.">}}



### **Abstract**

Computing injective maps with low distortions is a long-standing problem in computer graphics. Such maps are particularly challenging to obtain in the presence of positional constraints, because an injective initial map is often not available. Recently, several energies were proposed and shown to be highly successful in optimizing injectivity from non-injective initial maps while satisfying positional constraints. However, minimizing these energies tends to produce elements with significant isometric distortions. This paper presents simple variants of these energies that retain their desirable traits while promoting isometry. While our method is not guaranteed to provide an injective map, we observe that, on large-scale 2D and 3D data sets, minimizing the proposed isometric variants results in a similar level of success in recovering injectivity as the original energies but a significantly lower isometric distortion.

## **Video** 

{{< youtube 6Utp5YR28Mg >}}

## **Code**

Coming soon.


<!-- ## **Figures**

{{<figure alt="fig-success" src="/img/SEA/fig-success.png" title="Figure 2. Three successful examples from the benchmark: initial maps (first column), maps produced by our method (second column), which are all globally injective, and maps produced by LBD (third column) and SA (last column), none of which are locally or globally injective.">}}

{{<figure alt="fig-toys" src="/img/SEA/fig-toys.png" title="Figure 3. From left to right: input meshes (with one or two boundaries), non-injective initial maps, globally injective maps produced by our method (SEA), and results of LBD and SA. Both LBD and SA have removed most or all inverted triangles, but the results are neither locally or globally injective due to overwound vertices and boundary intersections.">}}

{{<figure alt="fig-overwound-1-rings" src="/img/SEA/fig-overwound-1-rings.png" title="Figure 4. Two initial maps with overwound vertices (top) and the injective maps produced by our method (bottom).">}} -->





<!-- ### **Acknowledgments**

This work is supported in part by NSF grant RI-1618685, NIH grant U2C CA233303-1, and Simons Math+X Investigators Award 400837. We would like to thank authors of several papers for providing code, data, and help with comparisons, and especially Hanxiao Shen, Ofir Weber, Alon Bright, Zohar Levi, and Xiao-Ming Fu. -->
