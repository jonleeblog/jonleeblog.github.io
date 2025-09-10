---
layout: single
author_profile: true
sidebar: true
nav: true
classes: wide
---

<h1>Shipped Titles</h1>

<div class="image-text-row">
  <img src="images/D4+X1_logo.png" alt="Image 2">
  <div class="text">
    <div class="h3-row">
        <h3><a class="project-links" href="https://diablo4.blizzard.com/en-us/vessel-of-hatred">Diablo IV: Vessel of Hatred</a></h3>
        <span class="h3-extra">October 2024</span>
    </div>
    <div class="project-desc">
        <p>The first Diablo IV Expansion</p>
    </div>
    <div class="h3-row">
      <h3><a class="project-links" href="https://diablo4.blizzard.com/en-us/">Diablo IV</a></h3>
      <span class="h3-extra">June 2023</span>
    </div>
    <div class="project-desc">
      <p>I collaborated with many art disciplines to deliver key graphics features and workflow improvements:</p>
      <ul>
          <li>Designed a VFX recoloring systlem, in collaboration with gameplay engineers and designers, to optimize power design workflow</li>
          <li>Co-implemented GTAO with another engineer to upgrade our AO system (Read more <a class="project-links" href="https://news.blizzard.com/en-us/article/24077218/hells-beauty-burns-anew-with-ray-tracing">here!</a>)</li>
          <li>Integrated the <a href="https://gpuopen.com/fidelityfx-denoiser/" class="project-links">FidelityFX Shadow Denoiser</a> to boost raytracing performance and quality</li>
      </ul>
    </div>
  </div>
</div>

<div class="image-text-row">
  <img src="images/D2R_logo.png" alt="Image 3">
  <div class="text">
    <div class="h3-row">
      <h3><a class="project-links" href="https://diablo4.blizzard.com/en-us/">Diablo II: Resurrected</a></h3>
      <span class="h3-extra">September 2021</span>
    </div>
    <div class="project-desc">
      <p>
          I collaborated mainly with VFX artists to develop shaders and provide support for the <a href="https://www.popcornfx.com/" class="project-links">PopcornFX editor</a>.
      </p>
      <ul>
          <li>Maintained and integrated the PopcornFX SDK upgrades into the engine</li>
          <li>Optimized various VFX memory and performance</li>
      </ul>
    </div>
  </div>
</div>

<hr>

<section class="portfolio-preview">
  <div class="h2-row">
    <h1>Portfolio</h1>
    <span class="h2-subtext"><a class="project-links" href="/portfolio">View all projects</a></span>
  </div>

  <div class="portfolio-preview-grid">
    {% assign preview_items = site.portfolio | sort: 'date' | reverse %}
    {% for item in preview_items limit:4 %}  <!-- show only 4 items -->
      <div class="portfolio-item">
        <a href="{{ item.url }}" class="project-links">
          <img src="{{ item.header.teaser }}" alt="{{ item.title }}" style="height: 100px">
          <h4>{{ item.title }}</h4>
        </a>
      </div>
    {% endfor %}
  </div>
</section>

<style>
.h2-row {
  display: flex;
  justify-content: space-between; /* left = h2, right = subtext */
  align-items: baseline;          /* align text nicely */
  margin-bottom: 1rem;            /* spacing below the row */
  border-bottom:none;
}

.h2-row h2 {
  margin: 0;
  font-size: 1.5rem;              /* adjust as needed */
  border-bottom:none;
}

.h2-subtext {
  font-size: 1rem;                /* smaller than h2 */
  color: #666;
}

.portfolio-preview-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.portfolio-item img {
  height: 200px;
  width: auto;          /* keeps aspect ratio */
  display: block;
  margin: 0 auto;
  object-fit: cover;    /* fills container nicely */
}

.portfolio-item h4 {
  margin-top: 0.5rem;
  font-size: 1rem;
}

.h3-row {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  gap: 1rem; /* optional spacing */
}

.h3-row h3 {
  margin: 0;
  font-size: 1.25rem;
  font-weight: 600;
  line-height: 1.2;
  flex-shrink: 1;       /* allow h3 to shrink to fit */
  min-width: 0;         /* prevents overflow in flex container */
}

.h3-extra {
  font-size: 0.9rem;
  color: #999;
  white-space: nowrap;   /* keeps extra text on one line */
}

.subheading {
  margin: 0 0 0.5rem 0;
  font-size: 1rem;
  font-weight: 400;
  color: #666;
}

@media (max-width: 768px) {
  .h3-row {
    flex-direction: column;
    align-items: flex-start;
  }

  .h3-extra {
    margin-top: 0.25rem;
    white-space: normal; /* allow wrapping if stacked */
  }
}


.image-text-row {
  display: flex;
  align-items: flex-start;       /* vertically center image and text */
  gap: 1.5rem;               /* space between image and text */
  margin-bottom: 2rem;       /* space between rows */
}

.image-text-row img {
  max-width: 40%;            /* adjust image width */
  height: auto;
  border-radius: 8px;
}

.image-text-row .text {
  flex: 1;                   /* text takes remaining space */
} 
</style>
