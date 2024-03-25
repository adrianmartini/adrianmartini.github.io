---
title: "An Additive Noise Approximation to Keller-Segel-Dean-Kawasaki Dynamics Part I: Local Well-Posedness of Paracontrolled Solutions"
authors:
- admin
- Avi Mayorcas
date: "22.09.2022"
doi: "10.48550/arXiv.2207.10711"

share: false

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
- linear fluctuating hydrodynamics
- parabolic-elliptic Keller–Segel model
- Dean–Kawasaki equation
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
  caption: 'Simulation of the Keller–Segel–Dean Kawasaki equation'
  focal_point: "Center"
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

# Description

We are interested in the fluctuating hydrodynamics of the Keller–Segel model of chemotaxis, the so-called Keller–Segel–Dean–Kawasaki (KSDK) equation:

{{< math >}}
\begin{equation*}
\begin{cases}
  (\partial_{t}-\Delta)\rho &= -\nabla\cdot(\rho\nabla c)-\nabla\cdot(\sqrt{\rho}\boldsymbol{\xi}),\\
  -\Delta c &= \rho,
\end{cases}
\end{equation*}
{{< /math >}}

where {{< math >}}$\boldsymbol{\xi}${{< /math >}} denotes a vector-valued space-time white noise.

This equation is a mesoscopic model for the dynamics of a finite population in which particles disperse a chemical {{< math >}}$c${{< /math >}}, to which other particles react by moving up the chemical gradient. Due to the non-linear noise, we do not expect KSDK to be well-posed[^1].

[^1]: V. Konarovskyi. T. Lehmann. M.-K. von Renesse. Electron. Commun. Probab. 24, 2019

 Instead, we consider an additive-noise approximation on the two-dimensional torus {{< math >}}$\mathbb{T}^{2}=\mathbb{R}^{2}/\mathbb{Z}^{2}${{< /math >}} and establish its well-posedness with the theory of paracontrolled calculus[^2].
 
 Let {{< math >}}$\sigma\in C_{T}\mathcal{H}^{2}${{< /math >}} be a space-time inhomogeneity, {{< math >}}$\delta>0${{< /math >}} be the correlation length and {{< math >}}$\boldsymbol{\xi}^{\delta}${{< /math >}} be a mollified space-time white noise. We show that there exists a sequence of deterministic functions {{< math >}}$(f^{\delta})_{\delta>0}${{< /math >}} such that the solutions {{< math >}}$\rho^{\delta}${{< /math >}} to
{{< math >}}
\begin{equation*}
\begin{cases}
  (\partial_{t}-\Delta)\rho &= \nabla\cdot(\rho\nabla\Phi_{\rho}-f^{\delta})+\nabla\cdot(\sigma\boldsymbol{\xi}^{\delta}),\\
  -\Delta \Phi_{\rho} &= \rho-\langle1,\rho\rangle_{L^{2}(\mathbb{T}^{2})},
\end{cases}
\end{equation*}
{{< /math >}}
converge as {{< math >}}$\delta\to0${{< /math >}} to a unique limit {{< math >}}$\rho${{< /math >}}.

The sequence of counter-terms {{< math >}}$(f^{\delta})_{\delta>0}${{< /math >}} diverges at most logarithmically as {{< math >}}$\delta\to0${{< /math >}}, whereas naïve power counting would suggest a divergence of order {{< math >}}$\delta^{-1}${{< /math >}}. This improvement is due to non-trivial symmetries in the Fourier multiplier {{< math >}}$\Phi${{< /math >}}. Furthermore by the same argument, {{< math >}}$(f^{\delta})_{\delta>0}${{< /math >}} is identically equal to {{< math >}}$0${{< /math >}} if {{< math >}}$\sigma\equiv1${{< /math >}}, which shows that inhomogeneities may induce divergences that need to be renormalised by fields rather than constants.
 
 [^2]: M. Gubinelli, P. Imkeller, N. Perkowski. *Forum Math. Pi*, 3, 2015, Article e6.

