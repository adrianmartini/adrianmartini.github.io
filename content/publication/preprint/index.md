---
title: "An Additive Noise Approximation to Keller-Segel-Dean-Kawasaki Dynamics Part I: Local Well-Posedness of Paracontrolled Solutions"
authors:
- admin
- Avi Mayorcas
date: "22.09.2022"
doi: "10.48550/arXiv.2207.10711"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-09-22"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: "Submitted"
publication_short: ""

abstract: Using the method of paracontrolled distributions, we show the local well-posedness of an additive noise approximation to the fluctuating hydrodynamics of the Keller-Segel model on the two-dimensional torus. Our approximation is a non-linear, non-local, parabolic-elliptic stochastic PDE with an irregular, heterogeneous space-time noise. As a consequence of the irregularity and heterogeneity, solutions to this equation must be renormalised by a sequence of diverging fields. Using the symmetry of the elliptic Green's function, which appears in our non-local term, we establish that the renormalisation diverges at most logarithmically, an improvement over the linear divergence one would expect by power counting. Similar cancellations also serve to reduce the number of diverging counterterms.

# Summary. An optional shortened abstract.
summary: 

tags:
- singular stochastic partial differential equation
- paracontrolled distributions
- linear fluctuating hy- drodynamics
- parabolic-elliptic Keller–Segel model
- Dean–Kawasaki equation;
featured: true

links:
- name: ArXiv Link
  url: https://arxiv.org/abs/2207.10711
url_pdf: https://arxiv.org/pdf/2207.10711.pdf
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
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.

projects: []

#projects:
#- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.

slides: ""
#slides: example
---

We are interested in the fluctuating hydrodynamics of the Keller–Segel model of chemotaxis, the so-called Keller–Segel–Dean–Kawasaki (KSDK) equation:

{{< math >}}
$$
\begin{cases}
  (\partial_{t}-\Delta)\rho = -\nabla\cdot(\rho\nabla c)-\sqrt{\eps}\nabla\cdot(\sqrt{\rho}\boldsymbol{\xi}),\\
  -\Delta c = \rho.
\end{cases}
$$
{{< /math >}}

This equation is a mesoscopic model for the dynamics of a finite population in which particles disperse a chemical

{{< math >}}
$c$
{{< \math >}},

to which other particles react by moving up the chemical gradient. For a survey on the rôle of chemotaxis in biology, see [K. J. Painter. *J. Theor. Biol.* 481, 2019].

Due to the non-linear noise, we do not expect KSDK to be well-posed. Instead, we consider an additive-noise approximation and establish its well-posedness with the theory of paracontrolled calculus [M. Gubinelli, P. Imkeller, N. Perkowski. *Forum Math. Pi*, 3, 2015, Article e6]

