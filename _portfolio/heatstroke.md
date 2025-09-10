---
title: "Heatstroke - Volumetric Renderer"
excerpt: "Real-time volumetric renderer written in JavaScript and WebGL "

order: 6
sort_by: order

header:
  teaser: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/heatstroke/demo.gif

author_profile: true
sidebar: true
nav: true

sidebar:
  # - title: "WebGL, JavaScript"
  #   text: '<a href="https://github.com/rms13/WebGL2-Volumetric-Renderer" class="project-links" target="_blank"><i class="fab fa-github"></i>Repo</a>'
  # - text: '<a href="https://rms13.github.io/WebGL2-Volumetric-Renderer/" class="project-links" target="_blank">Demo</a>'
gallery:
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/heatstroke/demo.gif
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/heatstroke/demo.gif
    alt: "demo"
  - url: https://raw.githubusercontent.com/rms13/WebGL2-Volumetric-Renderer/master/images/Godrays/goddrays.png
    image_path: https://raw.githubusercontent.com/rms13/WebGL2-Volumetric-Renderer/master/images/Godrays/goddrays.png
    alt: "god rays"
  - url: https://raw.githubusercontent.com/rms13/WebGL2-Volumetric-Renderer/master/images/Godrays/heterogenous.PNG
    image_path: https://raw.githubusercontent.com/rms13/WebGL2-Volumetric-Renderer/master/images/Godrays/heterogenous.PNG
    alt: "heterogeneous"
---

<aside class="sidebar__right" style="text-align:right;">
  <header>WebGL, JavaScript</header>
  <header><a href="https://github.com/rms13/WebGL2-Volumetric-Renderer" class="project-links" target="_blank"><i class="fab fa-github"></i>Repo</a> | <a href="https://rms13.github.io/WebGL2-Volumetric-Renderer/" class="project-links" target="_blank">Demo</a></header>
  <header></header>
</aside>

<p class="project-desc">Heatstroke is a real-time physically-based volumetric renderer that is based on EA's Frostbite Engine presented at Siggraph 2014 by Sebastien Hillaire. <a href="https://github.com/rms13" target="_blank" class="project-links">Rishabh Shah</a> and I worked on this as our final project for CIS565: GPU Programming Fall 2017.</p>

<p class="project-desc">WebGL 2.0 offers many features that weren't available in WebGL 1.0 and were indispensible for our implementation, including 3D textures and multiple render targets.</p>

<p class="project-desc">We developed a pipeline that was built from a clustered deferred renderer:
Shadow Mapping, G-Buffer Pass, Volumetric Pass, Final Shading and Tone Mapping.</p>

<p class="project-desc">(You can check out my deferred renderer <a class="project-links" href="https://github.com/AgentLee/ClusteredRenderer" target="_blank">here</a>.)</p>

<p class="project-desc">For more details and an in-depth performance analysis, visit our <a class="project-links" href="https://github.com/rms13/WebGL2-Volumetric-Renderer" target="_blank">repo</a>.
Must have WebGL 2.0 enabled to run the demo!</p>

{% include gallery %}

<style>
.links-row {
  display: flex;
  gap: 1rem;           /* space between links */
}

.sidebar-link {
  text-decoration: none;
  color: inherit;       /* match sidebar text color */
  font-weight: 500;
  transition: color 0.2s;
}

.sidebar-link:hover {
  color: #007acc;       /* optional hover color */
}
</style>