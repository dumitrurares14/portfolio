---
title: "Blightspire engine contributions"
date: 2024-09-25T18:35:46+05:30
params:
  dateLast: Current day
draft: false
description: "Blightspire engine contributions"
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
# ENGINE & TOOLS


## Jolt Physics integration

- I implemented Jolt Physics library in our engine as a solution for collision and ray casting.

![Blightspire](/images/projects/blightspire/jolt.gif)

- Designed a system to sync the rigid bodies transforms with our transform component in order to keep the more complex models within expectations when moving or simulating them.

![Blightspire](/images/projects/blightspire/physics_sync.png)

---

## Tooling for all the features I made

- For each graphics feature I implemented, I also created tools for the editor to allow everyone in the team to tweak everything as they desire.
- The tools are simple and made with ImGuI in a settings like manner, that facilitate accessibility

<center>

![Blightspire](/images/projects/blightspire/s1.png)

<br>

![Blightspire](/images/projects/blightspire/s2.png)

<br>

![Blightspire](/images/projects/blightspire/s3.png)

<br>

![Blightspire](/images/projects/blightspire/s4.png)

<br>

![Blightspire](/images/projects/blightspire/s5.png)

</center>



---
# GAMEPLAY


## Quake style movement

- I implemented a fast paced movement style similar to the one in quake and guided by <a href="https://github.com/id-Software/Quake/tree/master/"><strong>their original code base</strong></a>
- Features
  - Sliding
  - Jumping and double jumping
  - Dashing
  - Assisted bunny hopping
  - Ramp leaping
  - Fully integrated with Jolt's rigid bodies
- Fully implemented in Wren

<video controls width="100%" >
  <source src="/images/projects/blightspire/movement.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## Enemy bone effects

- Implemented bone effects for our skeleton enemies
  - Sound effects
  - Particle effects (Made using our custom particle system)

<video controls width="100%" >
  <source src="/images/projects/blightspire/bones.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


---

## Pistol effects

- Added polish and feel to our main gun in the game
  - Sound effects
  - Bullet trail
  - Bullet hole smoke
  - Reload bullets based on player's velocity


<video controls width="100%" >
  <source src="/images/projects/blightspire/revolver.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


## Ranged enemy

- Worked on the ranged enemy idle and attack behavior

<video controls width="100%" >
  <source src="/images/projects/blightspire/eye.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## Navigate

<div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center; align-items: center; margin-top: 1rem;">



  <a href="/blightspire/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/blightspire/blightspire.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 3rem; border-radius: 8px;">Back to overview</h3></center>
    </div>
  </a>

  <a href="/blightspire-graphics/" style="text-decoration: none;">
    <div style="width: 300px; height: 180px; background-image: url('/images/projects/blightspire/graphics.png'); background-size: cover; background-position: center; border-radius: 12px; box-shadow: 0 4px 20px rgba(0,0,0,0.4); display: flex; align-items: center; justify-content: center;">
      <center><h3 style="color: white; background: rgba(0, 0, 0, 0.6); padding: 0.5rem 1rem; border-radius: 8px;">Graphics Contributions</h3></center>
    </div>
  </a>

</div>