---
title: Mini-Minecraft
date: 2024-12-11 12:29:00 -0500
toc: true
description: <span class="highlighter">OpenGL, C++, Qt</span>. Minecraft from scratch. Multi-threaded voxel rendering. Super Mario 64 integration!
media_subpath: /assets/img/
image:
    path: mario.png
---

A three week group project. This is Minecraft built from scratch using C++. I created a multi-threaded rendering backend using OpenGL, with draw call optimizations via grouping minecraft blocks into 128x128 mesh "chunks".

I also intergrated Mario 64 using libraries based on the [decompiled Super Mario 64 source code!](https://github.com/libsm64/libsm64)