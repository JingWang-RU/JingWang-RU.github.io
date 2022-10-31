---
layout: page
title: social recommendation
description: matrix completion
img: assets/img/graph.png
# redirect: https://unsplash.com
importance: 3
category: work
---

    ---
    Online matrix completion for signed link prediction. WSDM'17.
    ---

This work studies the binary matrix completion problem underlying a large body of real-world applications such as signed link prediction and information propagation. That is, each entry of the matrix indicates a binary preference such as "like" or "dislike", "trust" or "distrust". However, the performance of existing matrix completion methods may be hindered owing to three practical challenges: 
* the observed data are with binary label (i.e., not real value); 
* the data are typically sampled non-uniformly (i.e., positive links dominate the negative ones)
* a network may have a huge volume of data (i.e., memory and computational issue).


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/social.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

We propose a novel framework which 
* maximizes the resemblance between predicted and observed matrices as well as penalizing the logistic loss to fit the binary data to produce binary estimates; 
* constrains the matrix max-norm and maximizes the F-score to handle non-uniformness; 
* presents online optimization technique, hence mitigating the memory cost. 

The loss function can be perfectly separated as:
\begin{equation}
L(Z,U,V;\Omega) = \sum_{(i,j)\in\Omega} \log (1+\exp(-Z_{ij}u_iv_i^T)).
\end{equation}

The constraints can be rewritten as:
\begin{equation}
||u_i||_2\leq \lambda, ||v_i||_2\leq \lambda, \forall 1\leq i\leq n.
\end{equation}

The gradients with respect to $$u_i$$ and $$v_j$$ are given by:
\begin{equation}
\dfrac{\partial }{\partial u_i}L(Z, U, V; \Omega) = \frac{-Z_{ij}\exp(-Z_{ij}u_iv_j^T)}{1+\exp(-Z_{ij}u_iv_j^T)}v_j,
\end{equation}
\begin{equation}
\dfrac{\partial }{\partial v_j}L(Z, U, V; \Omega) = \frac{-Z_{ij}\exp(-Z_{ij}u_iv_j^T)}{1+\exp(-Z_{ij}u_iv_j^T)}u_i.
\end{equation}

<b>Memory cost.</b> $$O(dn)$$ instead of $$O(n^2)$$ of SDP (Semi-Definite Program), where $$d$$ is approximated rank of $$Z$$.

<b>Convergence of threshold.</b>The obtained threshold converges asymptotically to the global optimal
value which maximizes the resemblance between $$B$$ and $$Z$$.




