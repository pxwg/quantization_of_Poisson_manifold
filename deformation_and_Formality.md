# Deformation Quantization: Motivate to Formality Conjecture

Consider the algebra $(\mathcal{A}, m)$ where $m$ is associative, which is equivalent to the condition
$$a\cdot (b \cdot c) = m(a,m(b,c))$$
$$(a \cdot b) \cdot c = m(m(a,b), c)$$
thus $a \cdot b \cdot c = m(a,m(b,c)) = m(m(a,b),c)$
which is similar to
$[m,m] = 0$
is an element of dg-Lie algebra. Consider the deformation of $m$, which could be written formally as $m + \hbar m_1 + \hbar^2 m_2 + \cdots$ i.e. $m + \gamma$ where $\gamma \in \hbar \mathcal{A}[[\hbar]]$, thus the Maurer-Cartan equation could be written as $[m+\gamma,m+\gamma] = 0$. Consider the Hoshchild cohomology operator $d \equiv [m, \cdot]$, we could rewrite the equation above as
$d_{m} \gamma + \frac{1}{2} [\gamma,\gamma] = 0$, which is the standard form of Maurer-Cartan equation. 

Note the Maurer-Cartan equation is gauge redundancy under the gauge transformation
$$\gamma \rightarrow \gamma + d_{m} a$$
where $a \in \mathfrak{g}^{1}$ is an element of order $1$ dg-Lie algebra, thus the deformation of assosiative multiplication $m$ could be identified to the moduli space of flat connections over the dg-Lie algebra $\mathfrak{g}^{2}$ i.e the space
$$\mathcal{M}_{m} = \left\{ \gamma \in \mathfrak{g}^{2}[[\hbar]] ;\  d_{m}\gamma + \frac{1}{2}\hbar[\gamma,\gamma] = 0 \right\}/\exp (\mathfrak{g}^{1})$$
At the usual quantization problem, we would focused on the Poisson Manifold $(\mathcal{M},\alpha)$ where $\alpha$ is the (degenerated) Poisson structure. The algebra $\mathcal{A}$ could be defined as the smooth function ring $C^{\infty }(\mathcal{M})$ where the multiplication is defined as the pointwise multiplication $m(f,g) = fg$. The (formal) deformation (which respect to the associativity) could induce star-product on the algebra $\mathcal{A}[[\hbar]] $, where the formal path between $m$ and $\star$ could be written as
$$\star : \mathcal{A}[[\hbar]] \otimes \mathcal{A}[[\hbar]] \rightarrow \mathcal{A}[[\hbar]] $$
where $\star : f \otimes g \mapsto fg + {f,g} \hbar + B_{2}(f,g)\hbar^{2}+\cdots $ i.e. the tangent of the formal path gives Poisson bracket over the manifold $\mathcal{M}$.

At the another side, the deformation of Poisson structure could be identified to the moduli space of flat connections on the dg-Lie algebra $\mathfrak{g}^{1}$. First, we can consider the standard Poisson structure $\alpha$ on the manifold $\mathcal{M}$, which could be written as an bi-verctor filed $\alpha = \alpha^{ij} \partial _{i} \wedge \partial _{j}$. The Poisson structure could used to define the Poisson bracket $\{f,g\} = \alpha^{ij} \partial _{i}f \partial _{j}g$ where $f,g \in C^{\infty}(\mathcal{M})$. According to the Jacobi identity, the Poisson structure is satisfied
$$\left[ \alpha , \alpha \right]_{\mathrm{SN}} = 0$$
where $\left[ \cdot , \cdot \right]_{\mathrm{SN}}$ is the Schouten-Nijenhuis bracket of poly vector space $\mathrm{PV}^{\cdot}(\mathcal{M})$, which is the Maurer-Cartan equation with Schouten-Nijenhuis bracket.

The deformation of Poisson structure could be written as $\alpha + \hbar \alpha_{1} + \hbar^{2} \alpha_{2} + \cdots$ where $\alpha_{i} \in \mathfrak{g}^{1}$. Thus the deformation $\alpha \mapsto \alpha+\gamma$ could be written as 
$$b_{\alpha}\gamma + \frac{1}{2}[\gamma,\gamma]_{\mathrm{SN}} = 0$$
which is the Maurer-Cartan equation with $b_{\alpha} : \gamma \mapsto [\alpha,\gamma]_{\mathrm{SN}}$ i.e. the  Lichnerowicz differential.

Based on the same idea, the moduli space of flat connections on the dg-Lie algebra $\mathfrak{g}^{1} = \mathrm{PV}^{1}(\mathcal{M}) = \Gamma(\Sigma_{\mathrm{dR}}; \bigwedge T^{\star } \mathcal{M}[1]$ could be written as 
$$\mathcal{M}_{\alpha} = \left\{ \gamma \in \mathfrak{g}^{1}[[\hbar]] ;\ b_{\alpha} \gamma + \frac{1}{2} \hbar [\gamma,\gamma] \right\}/\exp (\mathrm{Vect}(\mathcal{M}))$$
where $\mathrm{Vect}(\mathcal{M})$ could be viewed as the $1$ order bi-verctor field on the manifold $\mathcal{M}$.

Moreover, the unique non-trivial deformation of Poisson structure could be obtained by $\gamma(\hbar) = \hbar \alpha$, thus the formal path is simply a ray. ( 这句话是错误的，这只在 leading order 成立，换言之，when Poisson structure induces a communicative algebra, it's always zero which implies a trivial multiplication $m : f \otimes g \mapsto fg = gf$ over smooth function ring. The deformation of $m$ comes from a trivial multiplication over $\mathcal{A} = C^{\infty }(\mathcal{M})$, which is similar to the original point of Poisson structure which is simply $0$. So under the deformation quantization, the leading order of Poisson structure is $\gamma(\hbar) \in \hbar \mathrm{PV}^{2}(\mathcal{M})[[\hbar]]$. )

The discussion above gives us a non-trivial intuition between quantization and *Formality*. The formality is the existence of quasi-isomorphism between two DGLAs. If the formality is held between two DGLAs, there would be an 1-1 correspondence between the solutions of Maurer-Carton equation over both two DGLAs.

Under the language of moduli space, the formality is equivalent to the quasi-isomorphism between two moduli space.

Kontsevich's non-trivial observation is that, if the formality between $(\mathrm{PV}(\mathcal{M}), b_{\alpha})$ and $(C(C^{\infty }(\mathcal{M}),m), d_{\alpha})$ is satisfied, the quantization of smooth manifold is possible.

The observation could be understood with the way below. Consider a deformation path from original point over $\mathrm{PV}[[\hbar]]$, the formality tells us there exists a formal path over $\mathcal{A}[[\hbar]]$, which is a deformation quantization we were looking for. However, HKR theorem shows that
$$HH^{\cdot} (\mathcal{A},\mathcal{A}) \cong \bigwedge T\mathcal{M} \cong \mathrm{PV}^{\cdot}(\mathcal{M})$$
which helps us to rewrite the quantization-possible condition to 

> **Kontsevich's Formality Conjecture**  
> *The Hoshchild complex $C^{\cdot}(\mathcal{A}, \mathcal{A})$ is quasi-isomorphism as a DGLA to it's cohomology $HH^{\cdot}(\mathcal{A};\mathcal{A})$.*
