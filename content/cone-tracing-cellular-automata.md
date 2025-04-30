---
title: "Cone tracing cellular automata GI"
date: 2024-04-25T18:35:46+05:30
draft: false
description: "Cone tracing cellular automata GI"
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

![CTCAGI](/images/projects/ctcagi/ctcagi.png)

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
          </td>
        </tr>
        <tr><td><strong>Duration</strong></td><td>~4 weeks</td></tr>
        <tr><td><strong>Platform</strong></td><td>Windows</td></tr>
        <tr><td><strong>Engine</strong></td><td>Custom-built during Block C in Year 2 as a team project</td></tr>
        <tr><td><strong>Team size</strong></td><td>Solo</td></tr>
      </table>
    </div>
  </div>

  <div style="flex: 1 1 300px; min-width: 280px; text-align: center;">
    <h3>Tools & Technologies</h3>
    <div style="display: inline-block; text-align: left;">
      <table>
        <tr><td><strong>Languages & APIs</strong></td><td>C++, OpenGL, GLSL</td></tr>
        <tr><td><strong>Tools</strong></td><td>RenderDoc, Nsight Graphics</td></tr>
        <tr><td><strong>Workflow</strong></td><td>Git/GitHub</td></tr>
        <tr><td><strong>Libraries</strong></td><td>ImGUI, MagicaVoxel loader</td></tr>
      </table>
    </div>
  </div>

</div>


---

## Project Overview

During Block C in year 2 at Breda University of Applied Sciences I had the chance to work in a team on a voxel project. Since we were working with voxels it was a great opportunity for me to dive into global illumination research and prototypes and decided on trying cone tracing guided by the <a href="https://research.nvidia.com/sites/default/files/publications/GIVoxels-pg2011-authors.pdf">**famous nvidia paper from 2011**</a>.

---

## Goals and motivations

- Getting a **better understanding of global illumination** principles
- First time trying the interesting idea of **cellular automata for light propagation**
- Extra: I **love the slow propagation** of light volumes

---

## Biggest obstacles

- Overcoming workflow of **cone tracing** for the first time
- Hiding **light leaking** problems, especially when lights are close to walls
- Balancing light propagation speed and **performance**

---

## Highlights

- Cellular automata is used for direct light propagation
- Cone tracing for indirect calculation and direct sampling for volumetric effects as well as for specular

<center>

![CTCAGI](/images/projects/ctcagi/p.png)

</center>

---


## Presented at GPC 2024

<div style="position: relative; padding-top: 56.25%; /* 16:9 ratio */ height: 0; overflow: hidden; border-radius: 1rem; margin: 2rem auto;">
  <iframe
    src="https://www.youtube.com/embed/MONs5wMy6Rw?start=1213"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 1rem;">
  </iframe>
</div>

---
