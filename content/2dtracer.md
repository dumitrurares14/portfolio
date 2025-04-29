---
title: "2D Ray Tracer"
date: 2024-04-25T18:35:46+05:30
draft: false
description: "2D Ray Tracer"
layout: "single"
# galleryImages:
#  - src: https://iso.500px.com/wp-content/uploads/2016/03/stock-photo-142984111-1500x1000.jpg
#  - src: https://img.etimg.com/thumb/msid-68721417,width-650,imgsize-1016106,,resizemode-4,quality-100/nature1_gettyimages.jpg
#  - src: https://thumbs.dreamstime.com/b/team-ants-council-collective-decision-work-17037482.jpg
#  - src: https://thumbs.dreamstime.com/b/summer-day-smiling-women-relax-wearing-red-dress-fashion-standing-wooden-bridge-over-sea-blue-sky-background-summer-107411998.jpg
#  - src: https://thumbs.dreamstime.com/b/young-woman-playing-dog-pet-beach-sunrise-sunset-girl-dog-having-fun-seasid-seaside-cute-neglected-stay-66480218.jpg
#  - src: https://thumbs.dreamstime.com/b/funny-picture-taken-sunrise-frozen-lake-perspective-rider-retro-bicycle-sunrise-personal-211066044.jpg 
# viewer : true
# viewerOptions : {
#     title: false
#     # you can add more options here. refer https://github.com/fengyuanchen/viewerjs?tab=readme-ov-file#options
# }
toc: 
---

<center>

![2dtracer](/images/projects/2dtracer/2dtracer.png)

</center>

---
<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: flex-start;">

  <div style="flex: 1 1 300px; min-width: 280px; text-align: center;">
    <h3>Overview</h3>
    <div style="display: inline-block; text-align: left;">
      <table>
        <tr>
          <td><strong>Roles</strong></td>
          <td>
            Graphics programmer<br>
            Gameplay programmer
          </td>
        </tr>
        <tr><td><strong>Duration</strong></td><td>~8 week</td></tr>
        <tr><td><strong>Platform</strong></td><td>Windows</td></tr>
        <tr><td><strong>Engine</strong></td><td>Custom engine template - <a href="https://github.com/jbikker/tmpl8">Jacco Bikker</a></td></tr>
        <tr><td><strong>Team size</strong></td><td>Solo</td></tr>
      </table>
    </div>
  </div>

  <div style="flex: 1 1 300px; min-width: 280px; text-align: center;">
    <h3>Tools & Technologies</h3>
    <div style="display: inline-block; text-align: left;">
      <table>
        <tr><td><strong>Languages & APIs</strong></td><td>C++</td></tr>
        <tr><td><strong>Tools</strong></td><td>Visual studio, Very sleepy</td></tr>
        <tr><td><strong>Workflow</strong></td><td>Perforce</td></tr>
        <tr><td><strong>Libraries</strong></td><td>GLM, OpenMP</td></tr>
      </table>
    </div>
  </div>

</div>


---

## Project Overview

This 2D Ray Tracer was developed as a course project at BUAS during Block C of Year 1. The entire rendering pipeline runs on the CPU using C++, modifying a continuous pixel buffer that gets displayed at the end of each frame. To demonstrate the dynamic lighting capabilities, I made a small snake spinoff on top of the engine. 



---

## Goals and motivations

- Explore fundamental ray-tracing concepts such as intersection checks, shadows, lighting.
- Gain experience on CPU based renderers while improving C++ skills.
- Get a basic understanding of optimization techniques in ray tracing

---

## Biggest obstacles

- Grasping ray tracing concepts for the first time
- Optimizing such project to run on the CPU

---

## Highlights


- Support for point lights & spotlights
- Soft shadows and hard shadows settings, with different level of graphics fidelity to choose from
- Ray tracing intersection against basic shapes: Box, Circles, Lines
- Various optimizations tricks
- Denoising with last frame information
- Temporal accumulation denoise
- Snake game to showoff the rendering capabilities

<center>
<video controls width="100%" >
  <source src="/images/projects/2dtracer/stress.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
</center>

---


## Gameplay using this renderer

- Note: This gameplay is using the best settings in order to achieve ~60 FPS during gameplay in that scene on my laptop CPU
    - AMD Ryzen 7 6800H

<center>

![2dtracer](/images/projects/2dtracer/snake.gif)

</center>

