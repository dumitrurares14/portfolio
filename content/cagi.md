---
title: "Cellular Automata Global Illumination"
date: 2024-09-25T18:35:46+05:30
params:
  dateLast: Current day
draft: false
description: "Cellular Automata Global Illumination"
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

![CAGI](/images/projects/cagi/cagi.png)

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
            Engine programmer<br>
          </td>
        </tr>
        <tr><td><strong>Duration</strong></td><td>~1 Year in my spare time~</td></tr>
        <tr><td><strong>Platform</strong></td><td>Windows</td></tr>
        <tr><td><strong>Engine</strong></td><td>Custom-built from scratch</td></tr>
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

CAGI (Cellular Automata Global Illumination) is a technique that is aiming at computing approximations of diffuse light bounces into the scene by only using cellular automata. I have been working and researching this method in my spare time as well as during the self study hours during my university course.

---

## Goals and motivations

- Achieving a **high performance** global illumination solution that will enable good looking lighting on **lower end devices**
- This technique was never properly documented anywhere, and I wish to proceed further with my studies **doing a master with researching and applying CAGI**
- Trying to prove that **the overly used ray tracing** methods and probe methods are **not the only solutions** out there
- Aiming at getting an ideal **"infinite bounces"** feel in a **noise free** environment

---

## Biggest obstacles

- Managing memory efficiently since cellular automata ideally requires dense grids in order to compute
- Managing light directionality and shadow propagation
- Balancing light propagation speed and performance

---

## End Goal

- The end goal with this research is to have a working pipeline that will voxelize the scene in real time around the player in a 3D world, use CAGI to compute the nearby light calculations and sample the volume to shade the rendered meshes.

---


## My progress so far

<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: center; margin-top: 1rem;">



  <a href="/cagi-2d/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/cagi/cagi-2d.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 1rem; border-radius: 8px;">CAGI in 2D</h3></center>
    </div>
  </a>

  <a href="/cagi-3d/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/cagi/cagi-3d.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 1rem; border-radius: 8px;">CAGI in 3D</h3></center>
    </div>
  </a>

</div>

---

## Links

- [2D Youtube Showcase](https://youtu.be/V0-yVUaaWog)
- [3D Youtube Showcase](https://youtu.be/_Vm_Wg44h88)

