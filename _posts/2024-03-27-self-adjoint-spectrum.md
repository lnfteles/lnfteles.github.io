---
title: 'The spectrum and bounded self-adjointness'
date: 2024-03-27
permalink: /posts/2024/03/the-spectrum-of-bounded-self-adjoint-operators/
tags:
  - Spectral Theory
  - Functional Analysis
---

The spectrum $\sigma(T)$ of operators $T$ helps us them, and many of the problems spectral theorists face involve restraining this set $\sigma(T)$.

In complex Hilbert spaces $H$ an important class of bounded operators is well-suited to the task of reducing what values $\sigma(T) \subseteq \mathbb{C}$ can take, those are the self-adjoint bounded linear operators. Bounded linear operators ${T:H \to H}$ such that

$$\langle Tx,y\rangle = \langle x, Ty\rangle, \qquad \forall x,y \in H.$$

This kind of simmetry that defines the self-adjointness of $T$ brings about some nice consequences, for one it bounds the spectrum of these operators to the real line. One way of seeing how this may come to happen is looking at the case for the point spectrum $\sigma_p(T)$. If $\lambda \in \sigma_p(T)$, $Tx_0 = \lambda x_0$ for some $x_0 \in H$, using the sesquilinearity of the inner product we have that:

$$\lambda \langle x_0, x_0\rangle  = \langle Tx_0,x_0 \rangle = \langle x_0, Tx_0\rangle = \overline{\lambda} \langle x_0, x_0\rangle,$$

and so $\lambda = \overline{\lambda} \implies \sigma_p(T) \subseteq \mathbb{R}$.

To go even further, we may consider another set of complex values that is helpful in this context, that is ${\\{\langle Tx,x\rangle: x \in H\\}}$. Besides being related to self-adjointness itself \[1\], these values allow us to confine $\sigma(T)$ to a closed interval $\[m,M\]$ given by:

$$\sigma(T) \subseteq [\inf_{\|x\|=1} \langle Tx,x\rangle, \sup_{\|x\|=1} \langle Tx,x\rangle] =: [m,M].$$

This fact may be complemented by noting that $m$ and $M$ themselves end up being spectral values, so it turns out that $\[m,M\]$ is in fact the smallest interval containing $\sigma(T)$. Thus bringing about not only a significant reduction to the possibilities of spectral values, but enabling the use of the compactness of closed intervals in the real line, a fact taken advantage of in the Spectral Theorem.

\[1\] <https://math.stackexchange.com/questions/1277876/show-langle-tx-x-rangle-in-bbb-r-forall-x-in-h-implies-t-is-self-adj>
