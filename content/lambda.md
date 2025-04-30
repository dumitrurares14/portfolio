---
title: "Lambda Engine"
date: 2023-09-25T18:35:46+05:30
params:
  dateLast: January 2024
draft: false
description: "Lambda Engine"
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

![lambda](/images/projects/lambda/lambda.png)

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
            Engine programmer<br>
          </td>
        </tr>
        <tr><td><strong>Duration</strong></td><td>8 weeks</td></tr>
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
        <tr><td><strong>Languages & APIs</strong></td><td>C++, Lua</td></tr>
        <tr><td><strong>Tools</strong></td><td>Visual studio</td></tr>
        <tr><td><strong>Workflow</strong></td><td>Git/GitHub</td></tr>
        <tr><td><strong>Libraries</strong></td><td>ImGUI, Entt, TinyGLTF, SolLua, Cereal, GLM</td></tr>
      </table>
    </div>
  </div>

</div>


---

## Project Overview

Lambda engine is my first in-depth dive at the engine architecture world, where I tried to develop and understand how some of the most important features of an engine work under the hood. Following some design patterns from popular engines such as Unity, I also tried to leave my own touch on certain aspects.

---

## Goals and motivations

- Understand the important features of an engine:
    - How to use an ECS
    - How to create a simple resource manager
    - How to import gltf files
    - How to handle complex hierarchies
    - How to create a simple CPU based particle system
    - How to implement a scripting language
    - How to handle hot reloading
- Have fun with creating tools and UIs for all the systems


---

## Biggest obstacles

- Handling scripting with Lua and play, pause and stop scripting logic
- Grasping resource manager concepts for the first time
- Getting a better understanding of the GLTF spec sheet

---

## Highlights

- Full engine editor using ImGui
- Support for scripting with Lua
- Component based architecture, facilitating entt ECS
- Custom resource manager
- Scene serialization
- CPU based particle system
- Game start, stop, and pause
- Custom in engine console for logging errors, warnings and messages

<center>

![lambda](/images/projects/lambda/run.gif)

</center>

---


