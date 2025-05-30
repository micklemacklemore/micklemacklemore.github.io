---
title: CUDA Stream Compaction
date: 2024-12-11 12:29:00 -0500
toc: true
description: <span class="highlighter">CUDA, C++</span>. I implement GPU stream compaction algorithms, and compare their performance.  
media_subpath: /assets/img/
---

In this project, I implemented a GPU stream compaction algorithm using CUDA, with the goal of removing zeros from an array of integers.

Stream compaction is a critical technique in GPU programming, widely applicable in various scenarios (i.e. path tracing where terminated rays are compacted out of the working set).

This project involved both CPU and GPU implementations of the *all-prefix-sums* (or simply scan) algorithm as a foundation for the compaction process.

I used [Chapter 39 from GPU Gems 3](https://developer.nvidia.com/gpugems/gpugems3/part-vi-gpu-computing/chapter-39-parallel-prefix-sum-scan-cuda) as the basis for the GPU implementations.

### [See my GitHub Repo...](https://github.com/micklemacklemore/CUDA-Stream-Compaction)