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

<div style="position: relative; padding-top: 56.25%; /* 16:9 ratio */ height: 0; overflow: hidden; border-radius: 1rem; margin: 2rem auto;">
  <iframe
    src="https://www.youtube.com/embed/V0-yVUaaWog"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 1rem;">
  </iframe>
</div>

## Highlights

- Double buffering pipeline to compute one step per frame in order to achieve high performance results
- Fully ran by cellular automata rules in GLSL compute shaders. No ray tracing, no tricks.
- Not tied up by the number of lights.
  - All lights are being computed at once in the same simulation in the same volume, more lights won't affect performance or memory.


## Navigate

<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: center; margin-top: 1rem;">



  <a href="/cagi/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/cagi/cagi.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 1rem; border-radius: 8px;">Back to overview</h3></center>
    </div>
  </a>

  <a href="/cagi-3d/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/cagi/cagi-3d.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 1rem; border-radius: 8px;">CAGI in 3D</h3></center>
    </div>
  </a>

</div>

---
