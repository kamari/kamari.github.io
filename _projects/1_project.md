---
layout: page
title: project 1
description: with background image
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmsv-structure.jpg" title="mmSV structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of mmSV
</div>

As we move towards a future of connected and autonomous vehicles, high-speed and low-latency connectivity between vehicles is becoming increasingly important. This paper investigates enabling high data rate mmWave links in vehicle-to-vehicle (V2V) scenarios using street view images. We find that mmWave V2V links in urban settings suffer from frequent and prolonged blockages, resulting in unreliable connection and high beamforming overhead. Our work proposes mmSV, a system that creates 3D reflection profiles from street view images to assist vehicles in findingmmWave reflections from the environment in real-time. mmSV consists of two key components: material identification which identifies materials from street view images to determine their reflectivity and create 3D reflection map, and environment-driven raytracing and beamsearching which finds a high-SNR beam using predicted 3D material maps. Our extensive experimental results on the mmWave testbed show that mmSV can provide highly reliable V2V mmWave connectivity with low beamforming overhead. This work was presented in MobCom '23.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmsv-3dmap01.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmsv-3dmap02.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mmsv-3dmap03.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, Projection of material map on 3D buildings. Middle, Example of final generated 3D material map. Right, mmWave testbed.
</div>


