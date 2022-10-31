---
layout: page
title: computer vision
description: object detection, face recognition
img: assets/img/vision.png
importance: 1
category: research
---

    ---
    Object Proposal with Kernelized Partial Ranking. PR'17.
    ---

Given an input image, our system obtains the proposals which are produced by some previous proposal algorithm such as Selective Search, then splits the set of
candidates into the top-$$k$$ subset and the last n-k subset according to the IoU to the ground truth, (4)
computes features for each proposal followed by Consistent Weighted Sampling (CWS), and then (6) learns the
partial ranking model based on the output of CWS.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/proposal.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

    ---
    Visual data Denoising with a Unified Schatten-p norm and Lq norm regularized Principal Component Pursuit. PR'15.
    ---


The clear object is with low-rank structure, the noise is sparse.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/denoise_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">

</div>

Given the video, the background is with low rank structure and the front object is sparse.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/backfront.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    
</div>


    ---
    Robust Face Recognition via Adaptive Sparse Representation. IEEE Trans Cybern'15.
    ---

 Comparison recognition rates based on $$t$$ images of each subject for training on the AR database (A. Martinez'98).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/facerec.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
