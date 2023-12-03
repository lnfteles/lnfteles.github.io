---
title: 'Compact operators and the unit ball'
date: 2023-11-27
permalink: /posts/2023/11/compact-operators-and-the-unit-ball/
tags:
  - Spectral Theory
  - Functional Analysis
  - Banach Spaces
---

One famous fact in functional analysis is that the closed unit ball $B_X$ of a normed space $X$ is compact if, and only if, the space $X$ is finite dimensional.
As if paying homage to that, compact linear operators (operators that map bounded sets $A$ to relatively compact sets $T(A)$, where $\overline{T(A)}$ is compact), allude to both notions of compactness and finite-dimensionality.

As a consequence of the compactness of the unit ball, for operators between finite-dimensional spaces, this relationship is clear as all linear operators are compact.

In a more general case, compact operators $T:X \to X$ have very similar spectral properties to those of linear operators between finite-dimensional spaces. In particular, one finds all non-zero spectral values to be eigenvalues, all with finite dimensional eigenspaces and only finitely many of such outside of any given ball around the origin of the complex plane. 

One may also find several similarities between the generalized eigenspaces of any given eigenvalue and the rank-nullity theorem, e.g. if $\lambda\neq 0$ there exists $r \in \mathbb{N}$ such that:
$$X= \ker(T_\lambda^r)\oplus T_\lambda^r(X).$$

As a final remark, for spaces with a little more structure (especifically the Approximation Property) such as Hilbert spaces, every compact operator can be seen as the limit of finite-rank operators, so that the class of compact operators can be defined alternatively as the closure of the set of finite-rank operators in the norm topology.
