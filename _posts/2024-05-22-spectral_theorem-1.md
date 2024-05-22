---
title: 'Hilbert, Schmidt and the Spectral Theorem'
date: 2024-05-22
permalink: /posts/2024/05/the-spectral-theorem-1/
tags:
  - Spectral Theory
  - Functional Analysis
---

The Spectral Theorem comes in many flavors, one might encounter it first in it's finite dimensional case, for $\mathbb{C}^n$. If $T:\mathbb{C}^n \to \mathbb{C}^n$ is a self-adjoint linear map then there is a basis $\{x_1, ..., x_n\}$ of $\mathbb{C}^n$ consisting of eigenvectors of $T$ with which we have:
$$Tx= \sum_{i=1}^n \lambda_i \langle x, x_i\rangle x_i.$$
As its name suggests, it falls to Spectral Theory to extend this result into infinite dimensional spaces. As it's usually the case, this brings forth considerable difficulties. One way of easing these difficulties is to retain some notion of finitude, in this case compactness. 

Specifically, if we now concern ourselves with a complex Hilbert Space $H$ and a compact self-adjoint linear operator $T:H \to H$ we find that $T$ has at most a countable number of eigenvalues $\{\lambda_i: i \in J\}$ and we verify the following decomposition
$$T= \sum_{i \in J} \lambda_i P_i,$$
where $P_i$ is the orthogonal projection of $H$ onto the eigenspace $\ker(T-\lambda_i I)$.

To go even further we need to overcome in some way  consequences of infinite-dimensionality. For this, we deal with the spectrum instead of just the eigenvalues of an operator ${T:H \to H}$, now only assumed to be bounded and self-adjoint. As I discussed in a previous post, studying the spectrum of bounded self-adjoint operators we find that it lies in a compact interval $[a,b]$ of the real line.

In the case of a discrete spectrum we can  use a series to represent the self-adjoint operator. In the general case this is not  possible and we look for the standard continuous alternative to summation: Integrals! 

In the integration of real-valued functions over the real line we combine real numbers in proportion to the size of the partition of the domain that they represent, now we need to combine projections. To do this we define a spectral measure \(E\) that maps the Borel sets on the real line to the space of orthogonal projections and from this derive the theory of Spectral Integration. With which we get the result that for any given bounded self-adjoint operator $T:H \to H$ we have a spectral measure $E$ such that we may write
$$\boxed{T = \int_a^b \lambda dE(\lambda).}$$
Although more intricate, this version of the Spectral Theorem still holds the essence of the original theorem: The decomposition of a self-adjoint operator into a "sum" of multiples of  orthogonal projections. 

P.S: There is still a notion of uniqueness for the spectral measure $E$: If there was any spectral measure on $\mathcal{B}(\mathbb{R})$ satisfying the decomposition above for the operator $T$ we would have $E(M\cap [a,b]) = F(M)$ for all $M \in \mathcal{B}(\mathbb{R})$.

These posts are motivated by a poster I recently presented in an event at my university. Said poster may be found (in portuguese) here: [O Teorema de Hilbert-Schmidt](https://lnfteles.github.io/talks/1semanadapura)
