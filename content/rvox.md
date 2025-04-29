---
title: "rVox Engine"
date: 2024-01-25T18:35:46+05:30
params:
  dateLast: March 2024
draft: false
description: "rVox Engine"
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

![rvox](/images/projects/rvox/rvox.png)

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
            Graphics programmer
            Engine programmer<br>
          </td>
        </tr>
        <tr><td><strong>Duration</strong></td><td>8 week</td></tr>
        <tr><td><strong>Platform</strong></td><td>Windows</td></tr>
        <tr><td><strong>Engine</strong></td><td>Custom-built</td></tr>
        <tr><td><strong>Team size</strong></td><td>Solo</td></tr>
      </table>
    </div>
  </div>

  <div style="flex: 1 1 300px; min-width: 280px; text-align: center;">
    <h3>Tools & Technologies</h3>
    <div style="display: inline-block; text-align: left;">
      <table>
        <tr><td><strong>Languages & APIs</strong></td><td>C++, OpenGL, OpenCL, GLSL</td></tr>
        <tr><td><strong>Tools</strong></td><td>CLTracer</td></tr>
        <tr><td><strong>Workflow</strong></td><td>Git/GitHub</td></tr>
        <tr><td><strong>Libraries</strong></td><td>ImGUI, MagicaVoxel loader</td></tr>
      </table>
    </div>
  </div>

</div>


---

## Project Overview

rVox is my first proper dive into the world of ray marching and voxels. Over 8 weeks I learned how to properly raymarch voxels inside a rasterized box and render them using only compute kernels. The most interesting part of this project is that I am not using any normals in the light calculations, admittedly with some artifacts and leaks, the results are looking interesting and quite fast.

---

## Goals and motivations

- Getting a better understanding of ray marching and voxel rendering
- Learning to handle compute kernels. I used OpenCL as a personal choice.
- Understand how to get per voxel lighting for:
    - Cool blocky results
    - Noise free
    - Faster calculations

---

## Biggest obstacles

- Using and debugging OpenCL
- Grasping the concept of ray marching
- Achieving per voxel lighting look

---

## Highlights

- Fixed 64x64x64 scene with MagicaVoxel support
- Lighting and rendering using DDA
- Per voxel look, with no normals usage

<center>

![CTCAGI](/images/projects/rvox/tree.png)

</center>

---


## A more in depth dive?

<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: center; margin-top: 1rem;">

  <a href="https://www.rares-dumitru.dev/Per-Voxel-Lighting-for-Dummies/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/rvox/box.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 3rem; border-radius: 8px;">See blog post</h3></center>
    </div>
  </a>

</div>
