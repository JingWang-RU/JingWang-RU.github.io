---
layout: page
title: feature selection
description: sparse linear regression and graph spectral theory
img: assets/img/apple.jpg
importance: 1
category: work
---

<b>Background</b> In many machin learning tasks, the samples are fixed and feature can be generated dynamically, for example the features of patients.

The goal of online feature selectionis to make a decision on whether to keep the new fature in real time. For example, the features of patient are collected over time, e.g. history information on day $t_1$, the lab Testing results on day $t_2$ as shown in the following figure. The task of online feature selection is to select the most important features (in red rectangle) at each time step, and discard the remaining features. 

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/medical_online.jpeg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<b>Problem setup.</b> Suppose that there are n samples, the features 
<ul>
  <li>Each a_i being the ith feature</li>
  <li>Make the yes / no decision on whether to keep the feature</li>
  <li>Update the observation matrix </li>
</ul> 


<b>Contributions.</b> This work is a simple feature selection algorithm
<ul>
  <li>High dimensional regime n<< d</li>
  <li>Memory cost O(n^2 log n)</li>
  <li>Time efficiency O(n^3) </li>
  <li>Theoretical guarantee for k-means clustering</li>
</ul>


<b>Experiments</b>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>


You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
