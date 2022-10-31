---
layout: page
title: feature selection
description: linear regression, spectral theory
img: assets/img/apple.png
importance: 1
category: research
---

    ---
    Provable Variable Selection for Streaming Features. ICML'18.
    ---

<b>Background.</b> In many machin learning tasks, the samples are fixed and feature can be generated dynamically, for example the features of patients.

The goal of online feature selectionis to make a decision on whether to keep the new fature in real time. For example, the features of patient are collected over time, e.g. history information on day $$t_1$$, the lab Testing results on day $$t_2$$ as shown in the following figure. The task of online feature selection is to select the most important features (in red rectangle) at each time step, and discard the remaining features. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/medical_online.jpeg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<b>Problem setup.</b> Suppose that there are $$n$$ samples, 
  * Each $$ a_i $$ being the feature arrives at $$i$$th time step.
  * Algorithm makes the yes / no decision on whether to keep the feature $$a_i$$.
  * Update the data matrix $$A\in R^{n\times s_i} $$, $$s_i$$ is the number of selected features so far.


<b>Contributions.</b> This work is a simple feature selection algorithm
  * High dimensional regime $$ n\ll d $$.
  * Memory cost $$ O(n^2 log n) $$.
  * Time efficiency $$O(n^3)$$.
  * Theoretical guarantee for $$k$$-means clustering.



<b>Related works.</b> 
    
    ---
    Online Group Feature Selection. IJCAI'13.
    Online Feature Selection with Group Structure Analysis. TKDE'15.
    ---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/diagOnline.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

