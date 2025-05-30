---
title: CUDA Path Tracer
date: 2024-12-11 12:29:00 -0500
toc: true
description: <span class="highlighter">C++, CUDA</span>. Interactive path tracer. Supports glTF scenes, PBR textures and integrates Open Image Denoiser. 
media_subpath: /assets/img/
image:
    path: hero.png
---

### [See my GitHub Repo...](https://github.com/micklemacklemore/CUDA-Path-Tracer)

A two week solo project. 

This is a Path Tracing Renderer (i.e. Arnold, RenderMan, V-Ray) written in C++ and CUDA which utilizes GPU hardware. This is an interactive renderer! It supports basic materials and scene handling, including glTF support, color & normal textures, and more!

### Supported Features

* glTF File Format
* Albedo Maps
* Normal Maps
* Depth of field
* Open Image Denoiser intergration
* Physically-Based Materials (BxDFs)
  * Matte (Perfect Diffuse BRDF)
  * Mirror (Perfect Specular BRDF)
  * Glass (Specular Reflection BRDF + Specular Transmission BTDF, mixed by fresnel)
  * Brushed Metal (Torrance-Sparrow Microfacet BRDF Model with a Trowbridge-Reitz Distribution)

Part of my Computer Graphics graduate program at University of Pennsylvania: CIS 5650: GPU Programming.

