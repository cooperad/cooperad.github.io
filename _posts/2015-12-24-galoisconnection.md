---
layout: post
title: test2
--- 

<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

Let $$P,S$$ be posets, with maps going back and forth $$\varphi: P\to S$$ and $$\psi:S\to P$$. Viewing the posets as categories and the maps as functors, an adjunction $$\varphi \dashv \psi$$ simply states that

$$\varphi (p) \leq s \Leftrightarrow p \leq \psi (s).$$


This follows from the fact that in this setup, a hom-set consists of at most one element, expressing an inequality. The naturality condition of the adjunction is trivial, a direct consequence of monotonicity of poset maps and transitivity of order.

An adjunction between posets goes by another name: a Galois connection (the fundamental theorem of Galois theory relates the lattices of certain subgroups and field extensions in this way). Let’s see a simpler example, from set theory.

Consider a set map $$f:X\to Y$$. It induces poset maps on the powersets: direct image $$f_*: 2^X\to 2^Y$$ and inverse image $$f^*:2^Y\to 2^X$$. Recall that for any subset $$A\subseteq X$$, we have the inclusion

$$A\subseteq f^*f_*A,$$

which I try to remember by the slogan « push-pull inflates » accompanied by suitable hand gestures. Dually, « pull-push deflates »:

$$ f_*f^*B \subseteq B$$

for any $$B\subseteq Y$$.

These observations show that there is a Galois connection $$f_* \dashv f^*$$:

$$ f_* A \subseteq  B \Leftrightarrow A \subseteq f^* B$$.
