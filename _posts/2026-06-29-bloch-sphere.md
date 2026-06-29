---
title: Understanding the Bloch Sphere
subtitle: I try to explain how one can represent a quantum state (specifically, a qubit) in a way that is visualisable using the Bloch Sphere
layout: default
date: 2026-06-29
keywords: quantum computing, quantum information theory
published: true
---
I've started a project recently that's going to involve a good amount of quantum computing, which naturally requires a good understanding of the basics. One of the concepts that I found really difficult to understand when trying to learn the basics of QC was the idea of the Bloch Sphere, which is a way of visualising the characteristics of a qubit using a polar coordinates system. Here, I'll try to outline the way a qubit state is changed from its basic "cartesian" form to its "polar", and discuss some things that left me puzzled for a little while.

## Motivation: Qubit states

We can write any qubit state {% katexmm %}$\ket{\psi}${% endkatexmm %} as a linear combination of the two basis states {% katexmm %}$\ket{0}${% endkatexmm %} and {% katexmm %}$\ket{1}${% endkatexmm %}

{% katexmm %}
$$
\ket{\psi} = \alpha \ket{0} + \beta \ket{1}    
$$
{% endkatexmm %}
{% katexmm %}
$$
\ket{0} = (1, 0)^{\top},\quad \\
\ket{1} = (0, 1)^{\top} 
$${% endkatexmm %}
and,
{% katexmm %}
$$
\alpha, \beta \in \mathbb{C}
$${% endkatexmm %}

Already it can be quite troublesome trying to visualise what a qubit state might look like, or where its position might be. When we usually take a linear combination of two orthogonal vectors, we have an object with two degrees of freedom, but here, we scale our basis states with constants {% katexmm %}$\alpha${% endkatexmm %} and {% katexmm %}$\beta${% endkatexmm %} which live in the realm of complex numbers, which they themselves have two degrees of freedom. In total, we have a quantum state which takes on 4 degrees of freedom. 



We can write any qubit {% katexmm %}$\ket{\psi}${% endkatexmm %} as
$$
\ket{\psi} = \cos(\theta/2)\ket{0} + e^{i \varphi}\sin(\theta/2)\ket{1} \tag{1}
$$
where {% katexmm %}$0 \leq \theta \leq \pi${% endkatexmm %} and {% katexmm %}$0 \leq \psi \lt 2\pi${% endkatexmm %}

