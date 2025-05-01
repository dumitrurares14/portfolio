---
title: "Owlet"
date: 2024-04-25T18:35:46+05:30
draft: false
description: "Owlet"
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


## Particle system

- CPU based particle system ran with the ECS
- Particles have simple depth sorting and rendered separately from the other drawable.
- Emitter editor is complex and has most of the functionality of a modern emitter editor in an engine.

<small>
Note: Showcase video is from mid development; Depth sorting was not implemented at that point
</small>

<video controls width="100%" >
  <source src="/images/projects/owlet/Media1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## Procedural sky

- The dynamic sky is creating as a screen space effect using rays from the camera and fractal brownian noise to sample the clouds.
- Great to visualize the directional light
- Implementation based on: https://www.shadertoy.com/view/wslyWs

<center>

![Owlet](/images/projects/owlet/sky.png)

</center>

---

## Grass system

- ECS based to render a modest amount of foliage
- Different pipeline to render it, to account for wind and different coloring proprieties
- Wind shader simulates a global wind with noise by displacing vertex data for each grass card

<video controls width="100%" >
  <source src="/images/projects/owlet/Media2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## Post processing

- Post processing effects such as: 
  - color correction, vignette, film grain, screen space fog.

<video controls width="100%" >
  <source src="/images/projects/owlet/Media3.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


---

## Material system

- Engine and tools integration of our PBR renderer
- Real-time hot reloading textures for materials
- Textures preview

<center>

![Owlet](/images/projects/owlet/mat.png)

</center>

---

## Navigate

<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: center; margin-top: 1rem;">

  <a href="/owlet/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/owlet/owlet.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 3rem; border-radius: 8px;">Back to overview</h3></center>
    </div>
  </a>

</div>

