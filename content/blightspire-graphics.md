---
title: "Blightspire graphics contributions"
date: 2024-09-25T18:35:46+05:30
params:
  dateLast: Current day
draft: false
description: "Blightspire graphics contributions"
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


---
## Shadows

- Shadows are implemented in the classic shadowmap way using poisson sampling for noisy style.
- Static and dynamic geometry have their own separate shadowmap in order to improve performance.

![Blightspire](/images/projects/blightspire/shadow.png)

---

## Stylized art

- To compensate for the lack of artists in our team I implemented two effects aiming at solving our asset-like look of our game.
- Pixelization:
  - Using the depth buffer in order to determine different pixel levels across different distances, hence compensating for detail loss that other more common pixelization implementations may have.
- Quantized color palette:
  - Snapping the colors towards the closest ones in a color palette, adding a bit of dither and mixing between the original and the new color using the exposed settings.

![Blightspire](/images/projects/blightspire/art.png)

---

## SSAO and FXAA

- SSAO is implemented in a standard fashion using hemispheres to check against geometry.

![Blightspire](/images/projects/blightspire/ssao.png)

- FXAA is implemented as the industry standard in order to fix some of the aliasing problems. 

<img src="/images/projects/blightspire/fxaa2.png" alt="Blightspire FXAA" style="width: 100%">

---

## Procedural sky

- The dynamic sky is creating as a screen space effect using rays from the camera and fractal brownian noise to sample the clouds.
- Implementation based on: https://www.shadertoy.com/view/wslyWs

![Blightspire](/images/projects/blightspire/skygif.gif)

---

## Screen door transparency

- Worked on screen door transparency implementation 
- Used it as enemy death effects

![Blightspire](/images/projects/blightspire/dis.gif)


---

## Debug renderer

- Created a vulkan debug line rendering pipeline.
- We can push 3D lines positions towards this pipeline to render them.
- Jolt Physics pushes its debug lines in our debug renderer too, allowing for collision visualizations, ray casts etc.

![Blightspire](/images/projects/blightspire/lines.png)

---

## Navigate

<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: center; margin-top: 1rem;">



  <a href="/blightspire/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/blightspire/blightspire.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 3rem; border-radius: 8px;">Back to overview</h3></center>
    </div>
  </a>

  <a href="/blightspire-engine/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/blightspire/engine.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 1rem; border-radius: 8px;">Engine & Gameplay Contributions</h3></center>
    </div>
  </a>

</div>

---
