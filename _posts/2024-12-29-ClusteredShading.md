---
title: WebGPU Clustered Deferred Renderer
date: 2024-12-11 12:29:00 -0500
toc: true
description: <span class="highlighter">WebGPU, TypeScript</span>. Fast real-time lighting in the browser. And an educational read-me!
media_subpath: /assets/img/
image:
    path: sponza.png
---

### [See my GitHub Repo...](https://github.com/micklemacklemore/WebGPU-Deferred-Renderer)

This is a *[clustered deferred renderer](https://www.aortiz.me/2018/12/21/CG.html)* implemented in [WebGPU](https://github.com/gpuweb/gpuweb), an explicit GPU API for the web.   

The goal of this 1.5-week project was to:

* Learn the ***WebGPU API*** and develop a better understanding of explicit APIs.
* Understand ***clustered shading***, which involves splitting up the camera frustum into bounding "clusters", and assign the lights from the scene to them.
* Understand ***deferred shading***, which involves splitting rendering in to a "G-Buffer" render pass and a "Full-screen" lighting render pass.
  + ***"G-Buffer" geometry pass:*** process the geometry data and output seperate position, normal and albedo framebuffers
  + ***"Full-screen" Lighting pass:*** using the framebuffers from the last pass, calculate the lighting for each pixel.