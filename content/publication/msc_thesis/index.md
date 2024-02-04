---
title: "The Killed Mollified Super Brownian Motion and Paracontrolled Wild Sums"
authors:
- admin
date: "29.07.2020"
doi: ""

share: false

# Schedule page publish date (NOT publication's date).
publishDate: "2020-07-29"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["thesis"]

# Publication name and optional abbreviated publication name.
publication: "Mathematisch-Naturwissenschaftliche Fakultät der Rheinischen Friedrich-Wilhelms-Universität Bonn"
publication_short: "University of Bonn"

abstract: The main goal of this work is to construct the killed rough Super Brownian Motion, a superprocess in a white noise environment first introduced by Perkowksi and Rosati. To achieve this, we use a Branching Brownian Motion and a novel intermediate process called the killed mollified Super Brownian Motion. Not only does this simplify the construction of Rosati et al., it may also be more aligned with biological intuition. In order to show the uniqueness of the killed rough Super Brownian Motion, we construct a solution to the associated Evolution Equation, a certain Singular Stochastic Partial Differential Equation with a logistic non-linearity. This construction is carried out by introducing what we shall call Paracontrolled Wild sums, a lightweight tool which also yields the approximability of solutions and differentiability with respect to a small parameter in the initial condition.


# Summary. An optional shortened abstract.
summary: 

tags:
- singular stochastic partial differential equation
- paracontrolled distributions
- superprocesses
- rough super Brownian motion
- parabolic Anderson model
featured: true

links:
url_pdf: ''
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
  caption: 'The birth-death mechanism of a branching Brownian motion in a mollified white noise environment'
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

Let {{< math >}}$L>0${{< /math >}} be the domain size and {{< math >}}$m${{< /math >}} be a mollification parameter. Let {{< math >}}$\tau\in C_{c}^{\infty}(\mathbb{R}^{2},[0,1])${{< /math >}} be even such that {{< math >}}$\tau\equiv1${{< /math >}} in a neighbourhood of {{< math >}}$0${{< /math >}}. We define a mollified white noise with Neumann boundary conditions by 
{{< math >}}\begin{equation*}
\xi_{m}=\sum_{k\in\mathbb{N}_{0}^{2}}\tau((mL)^{-1}k)\mathscr{W}(\mathfrak{n}_{k})\mathfrak{n}_{k},
\end{equation*}{{< /math >}}
where $\mathscr{W}$ denotes a (spatial) white noise and {{< math >}}$(\mathfrak{n}_{k})_{k\in\mathbb{N}_{0}^{2}}${{< /math >}} an orthonormal basis of cosines.

The (Dirichlet) parabolic Anderson model on {{< math >}}$(0,L)^{2}${{< /math >}} needs to be renormalized by a sequence of counter-terms {{< math >}}$(c_{m})_{m\in\mathbb{N}}${{< /math >}} such that {{< math >}}$c_{m}=\frac{1}{2\pi}\log(m)+c_{\tau}${{< /math >}}, where {{< math >}}$c_{\tau}${{< /math >}} depends only on {{< math >}}$\tau${{< /math >}}. With this sequence of counter-terms, it follows that the solutions to the mollified (Dirichlet) parabolic Anderson model
{{< math >}}\begin{equation*}
(\partial_{t}-\Delta)u_{m}=(\xi_{m}-c_{m})u_{m}
\end{equation*}{{< /math >}}
converge as {{< math >}}$m\to\infty${{< /math >}}.

How does the renormalization affect an underlying population? Let {{< math >}}$(X^{m})_{m\in\mathbb{N}}${{< /math >}} be a (killed) super Brownian motion in a mollified white-noise environment, that is, for every {{< math >}}$\phi\in C_{0}((0,L)^{2})${{< /math >}} with {{< math >}}$\Delta\phi\in C_{0}((0,L)^{2})${{< /math >}}, it follows that
{{< math >}}\begin{equation*}
\langle\phi,X^{m}_{t}\rangle-\langle\phi,X^{m}_{0}\rangle-\int_{0}^{t}\langle(\Delta+\xi_{m}-c_{m})\phi,X^{m}_{s}\rangle\mathrm{d}s
\end{equation*}{{< /math >}}
is a continuous, square-integrable martingale with quadratic variation
{{< math >}}\begin{equation*}
\int_{0}^{t}\langle\phi^{2},X^{m}_{s}\rangle\mathrm{d}s.
\end{equation*}{{< /math >}}

Let {{< math >}}$T^{m}\phi${{< /math >}} denote the solution of the mollified parabolic Anderson model with initial data {{< math >}}$\phi${{< /math >}}. We can then identify linear moments of {{< math >}}$X^{m}${{< /math >}}:
{{< math >}}\begin{equation*}
\mathbb{E}(\langle\phi,X^{m}_{t}\rangle)=\mathbb{E}(\langle T^{m}_{t}\phi,X^{m}_{0}\rangle).
\end{equation*}{{< /math >}}
Hence, to find a natural interpretation for the renormalization of the parabolic Anderson model, it suffices to find an individual-based model for the (killed) super Brownian motion in a mollified white-noise environment. A natural choice is a branching Brownian motion in an environment determined by mollified white noise.

Fix a finite population size {{< math >}}$n${{< /math >}}. We define for {{< math >}}$x\in(0,L)^{2}${{< /math >}},
{{< math >}}\begin{equation*}
\zeta_{n,m}^{+1}(x)=\frac{1}{2}\Big(1+\frac{\xi_{m}(x)-c_{m}}{n}\Big),\quad\zeta_{n,m}^{-1}(x)=\frac{1}{2}\Big(1-\frac{\xi_{m}(x)-c_{m}}{n}\Big).
\end{equation*}{{< /math >}}
It follows that {{< math >}}$\zeta_{n,m}^{+1}(x)+\zeta_{n,m}^{-1}(x)=1${{< /math >}} and, for {{< math >}}$m${{< /math >}} sufficiently large, that {{< math >}}$\zeta_{n,m}^{+1}(x),\zeta_{n,m}^{-1}(x)\in[0,1]${{< /math >}} uniformly in {{< math >}}$x\in(0,L)^{2}${{< /math >}}. Hence, we can interpret those quantities as probabilities.

Let {{< math >}}$Y^{n,m}${{< /math >}} be a branching Brownian motion such that:

* particles evolve as variance-{{< math >}}$2/n${{< /math >}}-Brownian motions until they are killed upon reaching {{< math >}}$\partial(0,L)^{2}${{< /math >}};
* branching events occur with rate {{< math >}}$1${{< /math >}} at which a particle at position {{< math >}}$x\in(0,L)^{2}${{< /math >}} either gives birth with probability {{< math >}}$\zeta_{n,m}^{+1}(x)${{< /math >}} or dies with probability {{< math >}}$\zeta_{n,m}^{-1}(x)${{< /math >}};
* particles are born at the location {{< math >}}$x${{< /math >}} of their parent and evolve independently of them.

It then follows that {{< math >}}$X^{n,m}_{t}=\frac{1}{n}Y^{n,m}_{nt}${{< /math >}} converges in distribution as {{< math >}}$n\to\infty${{< /math >}} to {{< math >}}$X^{m}_{t}${{< /math >}}, the killed super Brownian motion in a mollified white-noise environment. Hence, the renormalization {{< math >}}$(c_{m})_{m\in\mathbb{N}}${{< /math >}} affects the underlying particle dynamics through the branching probabilities {{< math >}}$\zeta_{n,m}^{+1}(x),\zeta_{n,m}^{-1}(x)${{< /math >}} by introducing an asymptotically small perturbation of order {{< math >}}$\log(m)/m${{< /math >}}.


## Highlights

* Identified an intermediate process, the killed mollified super Brownian motion, in the universality class of N. Perkowski and T. Rosati’s killed rough super Brownian motion [T.C. Rosati, N. Perkowski, *Ann. Probab. 49(2)*, 2021; T.C. Rosati, *Electron. Commun. Probab.* 25, 2020]

* Developed a novel construction of singular stochastic PDEs with multiplicative noise and quadratic reaction terms based on Wild sums


