---
layout: page 
title: Research 
permalink: /research/
---

### Current Projects:

Starting to read about a friend's work on Branching Brownian Motion. Planning to animate some of the objects of study using Manim.

### Previous Projects:

**Bressan's conjecture on mixing flows:**
Consider the unit square in $$\mathbb{R}^2$$ with periodic boundary conditions (i.e., the torus) divided down the middle
$$x=1/2$$ line into sets $$R$$, $$B$$ (imagine half as painted red and the other half blue). We say that a flow mixes
$$R$$, $$B$$ up to scale $$\epsilon$$ with mixing factor $$\kappa \in (0,1/2)$$ if every $$\epsilon$$-ball has at
least $$\kappa$$ of its points from $$R$$ and $$\kappa$$ from $$B$$ (where this is defined in terms of the Lebesgue measure). If
we mix the initial condition to scale $$\epsilon$$ with some time-dependent divergence-free vector field $$f$$, how
much "work" is necessary? Here, "work" is measured as

$$\begin{equation*}
    \int_{0}^{T} \int_{\mathbb{T}^2} \lVert \nabla f(x,t) \rVert_{L^1} dxdt.
\end{equation*}$$

Bressan conjectured that this quantity grows at least logarithmically w.r.t. $$1/\epsilon$$. Existing literature has
proven the conjecture for $$L^p$$ norms, $$p > 1$$, but the machinery used in their results does not seem to extend to
the $$p=1$$ case. Alongside the conjecture, Bressan also constructed an example mixer; we will investigate some
numerical approaches to this problem (e.g., machine learning) to develop our intuition as to whether or not his
construction is optimal. I'm working on this project with Professor Tarek M. Elgindi. Fall 2021 independent study report
available [here]({{ site.url }}/assets/Mixing_CraigChen.pdf).

**Learning linear dynamical systems with memory:**
Consider a dynamical system with hidden state $$h_t$$, observable $$y_t$$, and control input $$u_t$$ following the dynamics

$$\begin{align*}
    h_{t+1} &= Ah_t + Bu_t \\
    y_t &= Ch_t + Du_t.
\end{align*}$$

It is known that gradient descent can learn this system (*i.e.,* learn the parameters $$A,B,C,D$$) with polynomially 
(in the dimension) many samples. What happens if we allow for a higher-order system which depends on $$h_t$$ through 
$$h_{t-m}$$? It is possible to linearize this system byconcatenating all of the state vectors, but then the matrices 
to be learned will be rather sparse and this advantage will go to waste. I am working with Professor Andrea Agazzi 
(and some advice from Professor Jianfeng Lu) to try to prove a better sample-complexity bound for the system with memory.

**Close lattice points on circles:**
We are interested in the question of how many lattice points can lie on an arc of length $$R^\theta$$ where $$R$$ is the
radius of a circle centered at the origin and $$\theta \in [0,1)$$. The best bound in current literature blows up as
$$\theta$$ approaches $$1/2$$. In this project, we produced a fully rigorous proof of the current bound as well as some
related lemmas and investigated potential methods to improve the bound. At the moment, it seems like an improvement will
require an entirely different approach. Mentored by Professor Lillian B. Pierce. Spring 2021 independent study report
available [here]({{ site.url }}/assets/Jarnik_CraigChen.pdf).

**Policy gradient methods in the linear-quadratic regulator with nonlinear controls:**
We aim to extend convergence results of existing literature to a wider policy class. As of now, there are still very few
convergence guarantees for policy gradient algorithms in settings with continuous state and action spaces (as opposed to
tabular). We prove that these algorithms converge in the setting of the LQR for policies that can be written as linear
combinations of globally Lipschitz functions; to prove our results we develop a new approach that involves iteratively
updating a discount factor. This project is mentored by Professor Andrea Agazzi. 
[https://arxiv.org/abs/2112.07612](https://arxiv.org/abs/2112.07612)
