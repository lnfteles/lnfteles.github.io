---
title: 'Neumann Series'
date: 2023-09-27
permalink: /posts/2023/09/Neumann-series/
tags:
  - Spectral Theory
  - Functional Analysis
  - Banach Spaces
---

Neumann series are series of bounded linear operators of the form 

$$\sum_{k=0}^\infty T^k = I + T + T^2 + ...$$

where $\|T\|< 1$, $T:X\to X$ and $X$ is a Banach space. When these conditions are met, we get that the operator $\sum{}_{k=0}^{\infty} T^k$ not only is well-defined and bounded but also has a bounded inverse of the form $(I-T)$. It's inverse gives us a hint at how this concept might be useful for Spectral Theory, that studies operators of the form $T-\lambda I$.

But first, why are these properties true? The convergence (and boundedness) of the series is guaranteed by the convergence of it's real counterpart $\sum{}_{k=0}^\infty\|T\|^k$ and the completeness of the space. It follows simply from the linearity of $T$ that the series behaves as a linear operator. 

The fact that it acts as the inverse for $I-T$ is a consequence of how the operator $I-T$, when composed with a power of $T$, computes the diference between that and the next power $(T^k-T^{k+1})$ and the sum of such differences ends up as the difference between the first and "last" iterations:
$$(I-T)\sum_{k=0}^n T^k = I -T + T -T^2 + T^2 +... - T^{n+1} = I-T^{n+1}$$
As $\|T^n\| \to 0$, with $n \to \infty$, we have $(I-T)\sum{}_{k=0}^\infty T^k = I$, because they comute we verify they are in fact the inverse of one another.

At first such a theorem may seem too niche, dealing only with operators with norms $\|T\|<1$. However, it is a very flexible tool that gives us a lot of fundamental results in Spectral Theory. Two examples of its usefulness are the following:
1. We may simply consider $(T-\lambda I)$, for $\lambda > \|T\|$ to be $\lambda(\frac{1}{\lambda}T - I)$ where clearly the operator $S = \frac{1}{\lambda}T$ has norm $\|S\| < 1$, guaranteeing that it, and $T-\lambda I$, are invertible.
2. Having determined that $T-\lambda_0 I$ has an inverse $R_{\lambda_0}$, we can rewrite $T-\lambda I$ as a further pertubation $-(\lambda-\lambda_0)I$ of the already known $T-\lambda_0I$:
$$T-\lambda = (T-\lambda_0I-(\lambda-\lambda_0)I) = (T-\lambda_0)(I-(\lambda-\lambda_0)R_{\lambda_0}).$$

In this form we see that for $\lambda$ sufficiently close to $\lambda_0$ there is no way of avoiding that $T-\lambda$ also be invertible ($\|(\lambda - \lambda_0)R_{\lambda_0}\|<1$).

These two results can be used as part of the proofs for why the spectrum is contained in the ball of radius $\|T\|$ and why the spectrum is closed, respectively.

(Please note that we are still working with the assumptions of the previous post, namely that $T \in B(X,X)$ and that $X$ is Banach).
