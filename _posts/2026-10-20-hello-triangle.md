---
layout: post
title: Hello, triangle
date: 2026-10-20 09:00
hero: /assets/img/triangle.svg
hero_alt: First software-rendered triangle
---
This first post doubles as a template: it shows every thing you can put in a
post. Copy it, change the file name to `YYYY-MM-DD-your-title.md`, and push.

Here is a normal inline image too:

![a triangle](/assets/img/triangle.svg)

And here is some code. Fenced blocks highlight automatically (rouge):

```c
typedef struct { float x, y, z; } vec3;

static float dot(vec3 a, vec3 b) {
    return a.x * b.x + a.y * b.y + a.z * b.z;
}
```

Uncomment the block below once you commit a clip to `assets/video/`:

<!--
<video controls preload="metadata" poster="/assets/img/triangle.svg">
  <source src="/assets/video/spinning-triangle.mp4" type="video/mp4">
</video>
-->

Delete this text, keep the structure, and happy rendering.
