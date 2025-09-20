---
title: "Refining Ramsey's theorem with ultrafilters"
date: 2025-09-19
permalink: /posts/2025/09/refining-ramseys-theorem-with-ultrafilters/
tags:
  - Set Theory
  - Ramsey Theory
---

Ramsey's theorem (in its infinite version) states that given any 2-coloring $\pi:[\omega]^2 \to 2$ of a 
countably infinite set say, $\omega$, there is an infinite subset $X \subseteq \omega$ such that $\pi([X]^2)$ is constant, in which case we say that $X$ is homogeneous for $\pi$.
In other words, for any coloring of the edges of a graph with countable vertices, there is some infinite subset of vertices whose edges are all of the same color. 

Ramsey's theorem influenced much of modern mathematics, in set theory, for instance, there are various areas of research which draw inspiration from Ramsey-type results
(see for instance Halbeisen's book \[2\]), the one which I'd like to discuss today tackles how one might reduce the class of sets which holds an infinite
homogeneous subset for any choice of $2$-coloring of $[\omega]^2$ from $\{X \subseteq \omega: X \text{ is infinte}\}$ to something "smaller". For our purposes we shall look for
a [non-principal ultrafilter](https://en.wikipedia.org/wiki/Ultrafilter#Ultrafilter_on_the_power_set_of_a_set) on $\omega$ which satisfies this condition. Formally speaking:

**Definition**: Let $\mathcal{U}$ be a non-principal ultrafilter on $\omega$. 

The existence of a Ramsey ultrafilter is independent of ZFC, but we can prove it under ZFC+CH or some weaker conditions, such as $\mathfrak{p}=\mathfrak{c}$ (c.f \[2\]). I'm 
interested in presenting a direct proof of the existence of a Ramsey ultrafilter from [Martin's Axiom](en.wikipedia.org/wiki/Martin's_axiom), following the arguments of 
Booth in his 1970 paper \[1\].

**Theorem**(ZFC+MA): There exists a Ramsey ultrafilter.

**Proof**: 


\[1\] Booth, D., _Ultrafilters on a countable set_, Annals of Mathematical Logic, Vol. 2 (1), 1-24, 1970.

\[2\] Halbeisen, L. J., _Combinatorial Set Theory With A Gentle Introduction to Forcing_, Springer-Verlag, 2012.
