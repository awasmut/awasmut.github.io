---
layout: post
title: Hello, triangle
date: 2026-10-20 09:00
---
All supported post elements, in one file. Copy it, rename it, write over it.

Image and video are commented out; uncomment them once the files are
committed:

<!--
![caption](/assets/img/cover.png)

<video controls preload="metadata">
  <source src="/assets/video/clip.mp4" type="video/mp4">
</video>
-->

Code fences highlight automatically:

```c
typedef struct { float x, y, z; } vec3;

static float dot(vec3 a, vec3 b) {
    return a.x * b.x + a.y * b.y + a.z * b.z;
}
```
