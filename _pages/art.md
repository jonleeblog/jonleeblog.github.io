---
title: Art
layout: collection       # Minimal Mistakes collection layout
permalink: /art/
collection: art    # tells the page which collection to display
entries_layout: grid     # options: grid, list, cards
author_profile: true
sidebar: true
nav: true
sort_by: order
classes: wide            # optional: make page wider

gallery-typography:
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-stitch.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-stitch.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-oswald.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-oswald.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-darth.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-darth.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-mike.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-mike.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-flynn.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-flynn.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-ariel.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/master/images/typography/thumb-ariel.png
    alt: "placeholder image 1"

gallery-3dmodel:
  - url: https://agentlee.github.io/images/Buzz/Dash.png
    image_path: https://agentlee.github.io/images/Buzz/Dash.png
    alt: "placeholder image 1"
  - url: https://agentlee.github.io/images/Buzz/Laser.png
    image_path: https://agentlee.github.io/images/Buzz/Laser.png
    alt: "placeholder image 1"
  - url: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/refs/heads/master/images/buzz/thumb-profile.png
    image_path: https://raw.githubusercontent.com/AgentLee/agentlee.github.io/refs/heads/master/images/buzz/thumb-profile.png
    alt: "placeholder image 1"
---

<h2>Typography</h2>
<div class="project-desc">
<p>Created in Adobe Illustrator</p>
</div>
{% include gallery id="gallery-typography" %}


## Videos
<div class="project-desc">
<p>Edited in Adobe Premiere and After Effects</p>
</div>
<div class="video-row">
  <div class="project-desc">
    <p style="text-align:left;">This was my final project for a film directing course I took at Rutgers.</p>
  </div>
  <iframe src="https://www.youtube.com/embed/zslfnvbApaQ?si=bM9EYr4n5itQH2IG" title="YouTube video 1" frameborder="0" allowfullscreen></iframe>

  <div class="project-desc">
    <p style="text-align:left;">This was a montage I put together reminiscing over my Disney College Program Internship.</p>
  </div>
  <iframe src="https://www.youtube.com/embed/5vj80s6MkAc?si=DINyz8iNDySCamq8" title="YouTube video 2" frameborder="0" allowfullscreen></iframe>
</div>

<style>
.video-row {
  display: flex;
  gap: 1rem;
  /* justify-content: center; */
  flex-wrap: wrap; /* stack on very small screens */
}

.video-wrapper {
  flex: 1 1 300px;        /* allows shrinking */
  max-width: 560px;       /* maximum width of iframe */
  aspect-ratio: 16 / 9;   /* keeps height proportional */
}

.video-wrapper iframe {
  width: 100%;
  height: 100%;
  border: none;
  display: block;
}
</style>

## 3D Modeling
<div class="project-desc">
<p>Maya + Mental Ray (2016)</p>
</div>
{% include gallery id="gallery-3dmodel" %}
