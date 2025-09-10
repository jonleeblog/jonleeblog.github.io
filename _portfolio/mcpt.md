---
title: "Monte Carlo Path Tracer"
excerpt: Physically-based renderer written in C++

order: 2
sort_by: order

header:
  teaser: https://leejon.net/img/thumbs/thumb_dragon.png

author_profile: true
sidebar: true
nav: true

# sidebar:
#   - title: "C++, Qt"
#     text: '<a href="https://github.com/agentlee/pathtracer" class="project-links" target="_blank"><i class="fab fa-github"></i>Repo</a>'
gallery:
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/dragon_32_5.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/dragon_32_5.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/stanford.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/stanford.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/goldendragon_32_8.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/goldendragon_32_8.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/lucy_20_8.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/lucy_20_8.png
    alt: "placeholder image 1"
    title: "Volumetric Rendering"
    caption: "Volumetric Rendering"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/csg_sphere_diff.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/csg_sphere_diff.png
    alt: "placeholder image 1"
    title: "Constructive Solid Geometry"
    caption: "Constructive Solid Geometry"
  - url: https://raw.githubusercontent.com/AgentLee/PathTracer/refs/heads/master/images/extra%20images/veach_32_8.png
    image_path: https://raw.githubusercontent.com/AgentLee/PathTracer/refs/heads/master/images/extra%20images/veach_32_8.png
    alt: "placeholder image 1"
gallery2:
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/variance/highvar.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/variance/highvar.png
    title: "High Variance"
    caption: "High Variance"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/variance/lowvar.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/mcpt/variance/lowvar.png
    title: "Low Variance"
    caption: "Low Variance"
---

<aside class="sidebar__right" style="text-align:right;">
  <header>C++, Qt</header>
  <header><a href="https://github.com/agentlee/pathtracer" class="project-links" target="_blank"><i class="fab fa-github"></i>Repo</a></header>
</aside>

<div class="project-desc">
  <p>Path Tracing is a rendering technique to generate images from 3D scenes as realistically as possible. Path tracing utilizes an estimation method called Monte Carlo estimation to approximate the light energy for a point from an arbitrary amount of samples. This will allow the light contribution to converge towards a solution that solves the Light Transport Equation.</p>

  <p>My path tracer supports multiple importance sampling, global illumination, volumetric rendering, and BVH acceleration</p>
</div>

{% include gallery %}

### Adaptive Sampling

<div class="project-desc">
  <p>I've also written an adaptive sampling feature where the variance gets calculated for each pixel and if the variance is outside a certain threshold, the pixel gets resampled. This led to faster render times (less samples per pixel) and less noisy renders.</a>
</div>

{% include gallery id="gallery2" %}
