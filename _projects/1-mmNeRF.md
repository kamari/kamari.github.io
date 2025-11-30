---
layout: page
title: mmNeRF
description: View Synthesis and 6DoF Pose Estimation in mmWave Radar Neural Radiance Fields
img: assets/img/mmnerf-datac.jpg
importance: 2
category: work
related_publications: true
---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmnerf-output.jpg" title="mmSV structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    mmNeRF View Synthesis examples
</div> 

Estimating a device's 6DoF pose (i.e., location and orientation) within the environment is a fundamental problem in robotics, and beyond. Millimeter-wave (mmWave) radars have emerged as an attractive alternative to optical sensors (e.g., RGB cameras) in these tasks due to their ability to operate in poor lighting and adverse conditions such as smoke and fog. This paper presents mmNeRF, a view synthesis and 6DoF pose estimation system based on neural radiance fields (NeRF) designed specifically for mmWave radars. mmNeRF requires only radar range-angle heatmaps collected in a given environment to construct its implicit neural representation, ensuring multi-view consistency and producing high-quality view synthesis. It then builds a 6DoF pose estimation framework that queries the neural model with particle filters to perform scan & matching operations to yield an accurate 6DoF pose. We evaluate mmNeRF using over 50K radar frames collected in six different indoor environments on a handheld rig equipped with a radar. Our results show that mmNeRF achieves median translation and rotation errors of 0.34m and 17.15° for single-spectrum 6DoF pose estimation and Absolute Trajectory Error (ATE) of 0.66m and 0.81 radians for continuous 6DoF pose tracking, considerably outperforming state-of-the-art solutions. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmnerf-datac.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmnerf-output1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, Data collection rig. Right, tracking result.
</div>



